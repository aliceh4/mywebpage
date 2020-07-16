<template>
  <div class="events">
    <h1>Events</h1>
    <div class="event-buttons">
        <b-button variant="primary" class="btn" @click="register">Register</b-button>
        <b-button variant="success" class="btn" @click="donate">Donate</b-button>
    </div>

    <div ref="paypal"></div>
  </div>
</template>

<!--  button click functions -->
<script>
export default {
    name: 'events',

    methods: {
        register() {
            this.$router.push("register")
        },
        donate () {
            this.$router.push("donate")
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

