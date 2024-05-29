<template>
    <h1>Non Props</h1>
    <nonpropsUser id="userData" />
</template>

<script>
import nonpropsUser from './nonpropsUser.vue';
export default{
    name:'nonProps',
    components:{
        nonpropsUser,
}
}
</script>