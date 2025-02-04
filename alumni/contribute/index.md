---
layout: single
title: Contribute
type: page
parent_id: '0'
published: true
password: ''
status: publish
categories: []
tags: []
---
Running the Ross Mathematics Program is expensive.

For many years, major funding for the Ross Program was provided by the National Science Foundation, 
and later by Ohio State University and the Clay Math Institute.  In 2015 the CMI moved its funding elsewhere, 
and in 2018 the Ross Program separated from OSU.  Scholarship funding is currently provided by the 
American Mathematical Society's [Epsilon Fund](http://www.ams.org/programs/edu-support/epsilon/emp-epsilon), 
and by [Jane Street](https://www.janestreet.com).  But most Ross funding now arises from student fees, 
enhanced by gifts from generous donors and by income from the Program's Endowment Funds. 
Please consider joining our effort to build those _Endowment Funds_. <br>
&nbsp; With your support the Ross Program will continue to thrive.

A wonderful start was made by the [Jacob Lurie](http://en.wikipedia.org/wiki/Jacob_Lurie)’s gift of $100,000 to the Ross Endowment Fund. Lurie was a student and counselor in the Ross Program in the 1990s, has been a professor at Harvard, and is now at the [Institute for Advanced Study](https://www.ias.edu/scholars/lurie).  He was recognized for his world-class mathematical research with both 
a [Breakthrough Prize](http://en.wikipedia.org/wiki/Breakthrough_Prize_in_Mathematics) and 
a [MacArthur Fellowship](http://www.macfound.org/fellows/class/class-2014/).

We ask you to follow Jacob Lurie’s lead by helping to build the Ross Endowment Fund. We still receive the income generated by the OSU Endowment Fund, 
but since 2019 all other Ross funds have been processed through the _Ross Mathematics Foundation_ 
a tax-exempt, 501(c)(3) corporation, with federal Tax ID (EIN) 83-1928343.  <br>
&nbsp; Your contribution is important, and will be greatly appreciated. 

For any method of contributing, please [send us a short email](mailto:ross@rossprogram.org) 
to make sure that we know about your donation. We will reply with a tax receipt. 

## How to Contribute

### By check

Please make out the check to the _Ross Mathematics Foundation_ with “Ross Endowment Fund” in the memo, and mail it to:

> Ross Mathematics Foundation  
> 1644 Andover Rd.  
> Columbus, OH 43212

### Online

Credit card contributions can be made online.

<script src="https://js.stripe.com/v3/"></script>

<section class="container">
            <button
              data-checkout-mode="payment"
              data-price-id="sku_If7ZrcBWCq94uo"
            >
              Donate $50.00 once
            </button><br/>
            <button
              data-checkout-mode="payment"
              data-price-id="sku_If7ZnOt6T0Glqv"
            >
              Donate $100.00 once
            </button><br/>
            <button
              data-checkout-mode="payment"
              data-price-id="sku_If7a7ZTEGdGwl0"
            >
              Donate $250.00 once
            </button><br/>
            <button
              data-checkout-mode="payment"
              data-price-id="sku_If7at30yUCHmK3"
            >
              Donate $500.00 once
            </button><br/>
            <button
              data-checkout-mode="payment"
              data-price-id="sku_If7ahu3GxrQTrv"
            >
              Donate $1000.00 once
            </button><br/>  
          </section>
<div id="error-message"></div>		  

<script>
      // Replace with your own publishable key: https://dashboard.stripe.com/test/apikeys
      var PUBLISHABLE_KEY = 'pk_live_EVv0HE4EnEnGBfjY2iBzPnuS003Q0UNubO';
      // Replace with the domain you want your users to be redirected back to after payment
      var DOMAIN = location.href.replace(/[^/]*$/, '');

      if (PUBLISHABLE_KEY === 'pk_test_Tr8olTkdFnnJVywwhNPHwnHK00HkHV4tnP') {
        console.log(
          'Replace the hardcoded publishable key with your own publishable key: https://dashboard.stripe.com/test/apikeys'
        );
      }

      var stripe = Stripe(PUBLISHABLE_KEY);

      // Handle any errors from Checkout
      var handleResult = function (result) {
        if (result.error) {
          var displayError = document.getElementById('error-message');
          displayError.textContent = result.error.message;
        }
      };

      document.querySelectorAll('button').forEach(function (button) {
        button.addEventListener('click', function (e) {
          var mode = e.target.dataset.checkoutMode;
          var priceId = e.target.dataset.priceId;
          var items = [{ price: priceId, quantity: 1 }];

          // Make the call to Stripe.js to redirect to the checkout page
          // with the sku or plan ID.
          stripe
            .redirectToCheckout({
              mode: mode,
              lineItems: items,
              successUrl:
                DOMAIN + 'success/?session_id={CHECKOUT_SESSION_ID}',
              cancelUrl:
                DOMAIN + 'canceled/?session_id={CHECKOUT_SESSION_ID}',
            })
            .then(handleResult);
        });
      });
</script>



### Corporate matching gifts

Many companies have giving plans that match their employees’ charitable contributions. 
Your employer’s Human Resources department can tell you whether such plans are in place.

### Alternative forms of support

We can work with you to accommodate contributions of various kinds, 
including stocks, bonds, mutual funds, or publicly traded securities. 
Many donors prefer to contribute appreciated securities in order to 
take advantage of federal income tax deductions. A tax accountant or 
financial planner can provide advice on which options are best for you. 
Please contact us at [ross@rossprogram.org](mailto:ross@rossprogram.org) to discuss possibilities.

### Private and corporate donors

Do you know of a foundation or corporation that might support the educational mission 
of the Ross Program? If so, please [send us](mailto:ross@rossprogram.org) your suggestions.

## Thank you

Thanks for your support. Your generosity is appreciated.
