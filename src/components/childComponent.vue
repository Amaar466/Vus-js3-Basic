<template>
    <h2>{{name}}</h2>
    <h2>{{user.email}}</h2>
    <button v-on:click="getData()">Click</button>
</template>

<script>
export default {
    name:"childComponent",
    props:{
        name:String,
        user:Object,
        getData:Function
    }
}
</script>