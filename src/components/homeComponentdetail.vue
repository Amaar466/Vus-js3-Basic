<template> 
    <h1 id="hello">Home component {{'hello'.length }}</h1>
    <h1>Name : {{ name }} </h1>
    <h1>Phone : {{ phone }} </h1>
    <h1>Email : {{ getEmail() }}</h1>
</template>

<script>
export default {
    name: 'homeComponentdetail',
    data(){
        return {
            name:'Amaar ul haq',
            phone:'0439540435',
        getEmail:function(){
            return 'amar@gmail.com'
        }
    }
    }

}
</script>

<style scoped>
#hello {
    color: orange
}
</style>