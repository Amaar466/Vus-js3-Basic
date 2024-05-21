<template>
    <h1   :class="{green:true}">Css Dynamic Binding</h1>
    <h1 class="otherClass"  :class="{green:colorFul}">Css Dynamic Binding</h1>
    <button v-on:click="colorFul=!colorFul">Apply Style</button>
</template>

<script>
export default{
    data() {
        return {
            colorFul:true
        }
    },
}
</script>

<style scoped>
  .green{
    background-color: green;
  }
</style>