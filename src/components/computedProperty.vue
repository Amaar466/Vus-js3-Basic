<template>
    <h1>Computed Property by computed method {{ getResult }}</h1>
    <h2>{{ dollar }}</h2>
    <h2>{{ rupeeVal }}</h2>
    <h2>{{ discont }}</h2>
    
</template>

<script>
export default{
    data() {
        return {
            dollar:100,
            rupeeVal:20,
            discont:10,
        }
    },
    computed:{
        getResult(){
            return (this.dollar*this.rupeeVal)-this.discont;
        }

    }
}
</script>