<template>
       Email::<input type="email" v-model="email">
    <br><br>
    Password::<input type="password" v-model="password">
    <br><br>
    <button v-on:click="getData()">Get Value</button>
</template>

<script>
export default{
    name:'getInput',

    data(){
        return{
            email:null,
            password:null,
        }
    },

    methods:{
        getData(){
           console.warn('hello', this.email,this.password);
        }
     
    }
}
</script>