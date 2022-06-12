<template>
  <div id="app">
    <HeaderWeatherApp v-bind:propsdata="currentData"></HeaderWeatherApp>
    <BodyWeatherApp></BodyWeatherApp>
    <FooterWeatherApp></FooterWeatherApp>
    <button v-on:click="getWeatherData">ddd</button>
  </div>
</template>

<script>
import HeaderWeatherApp from "./components/HeaderWeatherApp.vue"
import BodyWeatherApp from "./components/BodyWeatherApp.vue"
import FooterWeatherApp from "./components/FooterWeatherApp.vue"

export default {
  data() {
    return {
      currentData: {
        currentTemp: 10,
        minTemp: 5,
        maxTemp: 15,
        location: "서울",
        weatherDesc: "구름이 많이 낍니다."
      }
    }
  },
  components: {
    'HeaderWeatherApp': HeaderWeatherApp,
    'BodyWeatherApp': BodyWeatherApp,
    'FooterWeatherApp': FooterWeatherApp
  },
  methods: {
  }
}
</script>

<style>
body {
  text-align: center;
  background-color: #62626a;
  color: white;
}

</style>
