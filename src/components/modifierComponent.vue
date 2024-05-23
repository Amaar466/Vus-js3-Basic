<template>
    <h1>Modifier</h1>
    <input type="text" v-model.trim="data">
    <h2>Data is: {{ data }}</h2>
</template>

<script>
export default{
  data() {
    return {
        data:'',
    }
  },
}
</script>