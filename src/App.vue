<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Vue.js App" />
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
  <DynamicBinding />
  <PropsComponent />
  <RefComponent />
  <FormComponent />
  <ModifierComponent />
  <nonProps />
  <selectButton />
  <computedProperty />
  <watchComponent />
  <homeSlot />
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
import DynamicBinding from './components/dynamicBinding.vue';
import PropsComponent from './components/propsComponent.vue';
import RefComponent from './components/refComponent.vue';
import FormComponent from './components/formComponent.vue';
import ModifierComponent from './components/modifierComponent.vue';
import nonProps from './components/nonProps.vue';
import selectButton from './components/selectButton.vue';
import computedProperty from './components/computedProperty.vue';
import watchComponent from './components/watchComponent.vue';
import homeSlot from './components/homeSlot.vue';


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
    HtmlBinding,
    DynamicBinding,
    PropsComponent,
    RefComponent,
    FormComponent,
    ModifierComponent,
    nonProps,
    selectButton,
    computedProperty,
    watchComponent,
  homeSlot
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
