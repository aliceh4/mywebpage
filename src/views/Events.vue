<template>
  <div class="events">
    <h1>Events</h1>
    <div class="event-buttons">
        <b-button variant="primary" class="btn" @click="register">Register</b-button>
        <b-button variant="success" class="btn" @click="donate">Donate</b-button>
    </div>
    <form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_top">
        <input type="hidden" name="cmd" value="_donations" />
        <input type="hidden" name="business" value="RZB5U8H8AL9S8" />
        <input type="hidden" name="currency_code" value="USD" />
        <input type="image" src="https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif" border="0" name="submit" title="PayPal - The safer, easier way to pay online!" alt="Donate with PayPal button" />
        <img alt="" border="0" src="https://www.paypal.com/en_US/i/scr/pixel.gif" width="1" height="1" />
    </form>
  </div>
</template>

<!--  button click functions -->
<script>
export default {
    name: 'events',

    methods: {
        register() {
            this.$router.push({ name: "Register" })
        },
        donate () {
            this.$router.push({ name: "Donate" })
        },
    }
}
</script>

<!-- fix style for the buttons -->
<style>
.event-buttons {
    padding: 10px;
}
.btn {
    margin-left: 80px;
    margin-right: 80px;
}

</style>

