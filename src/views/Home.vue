<template>
  <div class="home">
    <br>
    <img alt="PCE logo" src="../assets/pce_logo.gif">
    <HelloWorld msg="Welcome!"/>
    
  </div>
  
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HomePage.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>
