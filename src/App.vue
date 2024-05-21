<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Vue.js App"/>
  <homeComponentdetail />
  <methodParams />
  <eventClick />
  <TowWaybinding />
  <getInput />
  <checkBox />
  <conditionIfelse />
  <loopsAll />
  <parentCompenent />
  <reuseComponent />
  <HtmlBinding />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import homeComponentdetail from './components/homeComponentdetail.vue'
import methodParams from './components/methodParams.vue';
import eventClick from './components/eventClick.vue';
import TowWaybinding from './components/towWaybinding.vue';
import getInput from './components/getInput.vue';
import checkBox from './components/checkBox.vue';
import conditionIfelse from './components/conditionIfelse.vue';
import loopsAll from './components/loopsAll.vue';
import parentCompenent from './components/parentCompenent.vue';
import reuseComponent from './components/reuseComponent.vue';
import HtmlBinding from './components/htmlBinding.vue';


export default {
  name: 'App',
  components: {
    HelloWorld,
    homeComponentdetail,
    methodParams,
    eventClick,
    TowWaybinding,
    getInput,
    checkBox,
    conditionIfelse,
    loopsAll,
    parentCompenent,
    reuseComponent,
    HtmlBinding
}
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
