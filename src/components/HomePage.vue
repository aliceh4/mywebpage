<template>
  <div class="homepage">
    <h1>{{ msg }}</h1>

    <p>
      We are the Parents and Children Education Club.<br>
      Check out
      <a href="http://pceclub.org/portal/index.php" target="_blank" rel="noopener">our website</a> 
      for more information.
    </p>

    <h3>Meetings</h3>
    <p>
      With COVID-19 preventing in-person events, meetings <br>
      for the PCE Club will be held virtually through zoom. <br>
      Please navigate to the events section of this page <br>
      for more information.
    </p>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>