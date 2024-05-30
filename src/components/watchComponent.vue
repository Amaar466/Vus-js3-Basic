<template>
    <h1>Watch Component</h1>
    <h2>{{ count }}</h2>
    <button v-on:click="count=count+1">+</button>
    <button v-on:click="count=count-1">-</button>
</template>

<script>
export default{
    data() {
        return {
            count:0
        }
    },
    watch:{
        count(val , prev){
        if (val>5 && val<prev) {
           this.count=0;
        }
        }
    }
}
</script>