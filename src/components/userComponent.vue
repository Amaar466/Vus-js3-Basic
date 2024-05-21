<template>
    <div class="user">
    <h2>{{ data.name }}</h2>
    <h2>{{ data.email }}</h2>
   <h2>{{ data.phoneNo }}</h2>
   <button v-on:click="getData(data.name)">Click</button>
</div>

</template>

<script>
export default{
    name:'userComponent',
    props:{
        data:Object,
        getData:Function
    }
}
</script>

<style scoped>
.user{
    background-color:brown;
    padding: 10px;
    margin-bottom: 23px;
    border-bottom: 1px solid;
    color: white;

}
</style>