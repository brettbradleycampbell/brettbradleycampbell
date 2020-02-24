---
layout: page
title: payment canceled
permalink: /canceled
---


<div class="homepage-about grid">
	<div class="grid__item medium-up--three-quarters">
		<h2 class="about-large">We build websites</h2>
    
    <!-- Load Stripe.js on your website. -->
<script src="https://js.stripe.com/v3"></script>

<!-- Create a button that your customers click to complete their purchase. Customize the styling to suit your branding. -->
<button
  style="background-color:#6772E5;color:#FFF;padding:8px 12px;border:0;border-radius:4px;font-size:1em"
  id="checkout-button-plan_GnPbs3xDcpI2qR"
  role="link"
>
  Checkout
</button>

<div id="error-message"></div>

<script>
(function() {
  var stripe = Stripe('pk_live_n8vDqxwCL1XGMJiGnu5qscXG');

  var checkoutButton = document.getElementById('checkout-button-plan_GnPbs3xDcpI2qR');
  checkoutButton.addEventListener('click', function () {
    // When the customer clicks on the button, redirect
    // them to Checkout.
    stripe.redirectToCheckout({
      items: [{plan: 'plan_GnPbs3xDcpI2qR', quantity: 1}],

      // Do not rely on the redirect to the successUrl for fulfilling
      // purchases, customers may not always reach the success_url after
      // a successful payment.
      // Instead use one of the strategies described in
      // https://stripe.com/docs/payments/checkout/fulfillment
      successUrl: window.location.protocol + '//brettbradleycampbell.com/success',
      cancelUrl: window.location.protocol + '//brettbradleycampbell.com/canceled',
    })
    .then(function (result) {
      if (result.error) {
        // If `redirectToCheckout` fails due to a browser or network
        // error, display the localized error message to your customer.
        var displayError = document.getElementById('error-message');
        displayError.textContent = result.error.message;
      }
    });
  });
})();
</script>
    
	</div>
</div>



<!--<div class="homepage-about grid">
	<div class="grid__item medium-up--three-quarters">
		<h2 class="about-large">We're your friendly neighborhood creative studio. We make brands, websites, videos, and marketing strategies. </h2>
		<p>Email us at <a href="mailto:brettbradleycampbell@gmail.com" class="underline-link">info@saintmaverick.co</a> or use our amazing <a href="{{ site.baseurl }}/contact" class="underline-link">contact form.</a></p>
	</div>
</div>-->
