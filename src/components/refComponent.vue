<template>
    <h1>Ref Component</h1>
    <input type="text"  ref="input">
    <button v-on:click="getData">Click me</button>
</template>

<script>
export default {

     methods: {
        getData(){
            this.$refs.input.focus();
            this.$refs.input.style.color="red";
            const val=this.$refs.input.value;
            console.warn(val);
        }
     },


}
</script>