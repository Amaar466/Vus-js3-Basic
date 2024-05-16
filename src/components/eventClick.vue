<template>
    <h1 id="event" v-on:mousemove="getConsole()">Event Clicked</h1>
    <button v-on:click="singleClick('Single Clicked')">Single Click</button>
    <button v-on:dblclick="singleClick('Double Clicked')">Double Click</button>
</template>

<script>
export default{
    name:'eventClick',
 

    methods: {
        singleClick(data){
            alert(data);
        },
        getConsole(){
        console.log('Function Called');
    },
    }
    

}
</script>


<style scoped>
#event{
    color: chocolate;
}
</style>