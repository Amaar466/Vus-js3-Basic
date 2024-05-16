<template>
    <br>
    <br>
<input type="text" v-model="count">
<h2>{{ count }}</h2>
</template>

<script>
export default{
    name:'towWayBinding',
    data(){
      return {
        count:10
      }
    }
}
</script>