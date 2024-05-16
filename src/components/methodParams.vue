<template>
    <h1 id="metparms">method And Params</h1>
    <h2>Name :: {{ getName('peter') }}</h2>
    <h2>getdata :: {{ getData() }}</h2>
    <h2>getdata by Name :: {{ getData() .name }}</h2>
    <h2>getdata by email:: {{ getData() .email }}</h2>
</template>


<script>
export default{
    name:'methodParams',
    data(){
        return {
            email:"amaarulhaq@gmail.com",
        }
    },

    methods:{
        getName(name){
            return name;
        },
        getData(){
            return {
                name:'amaar',
                email:this.email
            }
        }
    },
    
}

</script>


<style scoped>
#metparms{
    color: brown;
}
</style>