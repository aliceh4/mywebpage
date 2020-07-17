<template>
  <div class="events">
    <h1>Events</h1>
    <img alt="Event picture" src="../assets/eventpage.jpg" width=400px>
    <p>
      Many PCE club events are free of cost, so we would greatly <br>
      appreciate it if you could take the time to make a donation <br>
      to our group! If not, just press the register button to get <br>
      access to our meeting right away.
    </p>
    <div class="event-buttons">
        <b-button variant="primary" class="btn" @click="register">Register</b-button>
        <b-button variant="success" class="btn" @click="donate">Donate</b-button>
    </div>
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

