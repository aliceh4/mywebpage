<template>
  <div class="events">
    <br>
    <h1>Upcoming Events</h1>

    <!-- CHANGE THE EVENT PICTURE HERE:
         - add the jpg or png file into src/assets folder
         - change the code below accordingly so the file path is for your desired photo
         - adjust the size and name of the picture accordingly -->
    <img alt="Event picture" src="../assets/eventflyer.png" width=250px>

    <p>
        <br>
        <!-- CHANGE THE EVENT DESCRIPTION HERE:
             NOTE: make sure to add line breaks (<br>) accordingly to match the style
             of the webpage -->
        Insert event description here. <br>
        
        <br> 
        Many PCE club events are free of cost, so we would greatly <br>
        appreciate it if you could take the time to make a donation <br>
        for our group! If not, just press the register button to get <br>
        access to our meeting right away.
    </p>
    <div class="event-buttons">
        <b-button pill variant="outline-primary" class="btn" @click="register">Register</b-button>
        <b-button pill variant="outline-success" class="btn" @click="donate">Donate</b-button>
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

