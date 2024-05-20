<template>
    <h1 v-if="show">If Condition</h1>
    <h2 v-else>Else Condition</h2>
    <button v-on:click="show=!show">Toggle</button>

</template>

<script>
 export default{
   name:'conditionIfelse',
   data() {
    return {
        show:true 
    }
   }, 
 }
 
 </script>