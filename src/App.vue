<template>
  <div id="app">
    <!-- <router-view/> -->
      <!-- <slotTest :id="9">
        <h1 >GGG</h1>
      </slotTest> -->
      <!-- <slotTest>
        <template v-slot:jojo>
          <h1>Here might be a page title</h1>
        </template>
      </slotTest> -->
  <layout>
    <p slot="header">
      <headder></headder>
    </p>
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
    <router-view></router-view>
    <p slot="footer">
      <foot></foot>
    </p>
  </layout>
    <!-- <foot></foot> -->

  </div>
</template>

<script>
import foot from '@/components/footer'
import headder from '@/components/header'
import slotTest from '@/components/slotTest'
import layout from '@/components/layout'

export default {
  name: 'App',
  components: {
    'foot': foot,
    'headder': headder,
    'slotTest': slotTest,
    'layout': layout
  }
}
</script>

<style>
#app {
  text-align: center;
  color: #2c3e50;
}
</style>
