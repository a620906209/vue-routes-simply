<template>
  <div id="app">
    <headder></headder>
    <img src="./assets/logo.png">
    <div class="">  
      <ul>
        <li>
          <router-link to="/">Home</router-link>
        </li>
        <li>
          <router-link to="/firstroute/Peter">FirstRoute</router-link>
        </li>
        <li>
          <router-link to="/firstroute/Peter/child">FirstRouteChild</router-link>
        </li>
      </ul>
    </div>

    <router-view/>
    <foot></foot>

  </div>
</template>

<script>
import foot from "@/components/footer"
import headder from "@/components/header"

export default {
  name: 'App', 
  components:{
    'foot': foot,
    'headder': headder
  }
}
</script>

<style>
#app {
  text-align: center;
  color: #2c3e50;
}
</style>
