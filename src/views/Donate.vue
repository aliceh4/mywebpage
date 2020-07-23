<template>
  <div class="donate">
    <br>
    <h1>Donations</h1>
    <img alt="Giving picture" src="../assets/hearts.jpg" width=100px>
    <br>
    <p>
      Thank you so much for choosing to make a donation! Click <br>
      the donate button to be redirected to paypal.
    </p>

    <form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_blank">
      <input type="hidden" name="cmd" value="_s-xclick" />
      <input type="hidden" name="hosted_button_id" value="ZVQ7LDV49V5M2" />
      <input type="image" src="https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif" border="0" name="submit" title="PayPal - The safer, easier way to pay online!" alt="Donate with PayPal button" />
      <img alt="" border="0" src="https://www.paypal.com/en_US/i/scr/pixel.gif" width="1" height="1" />
    </form>

  </div>
  
</template>