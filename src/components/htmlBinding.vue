<template>
    <h1>Html Binding</h1>
    <h2>{{ text }}</h2>
    <h2>{{ tag }}</h2>
    <h3 v-html="tag"></h3>
</template>

<script>
export default{
    data(){
    return{
        text:'some thing',
        tag:'<h1>Heading </h1>'
    }
}
}
</script>