<template>
    <h1>Props in vue js 3</h1>
<studentComponentProps name="amaar"/>
<teacherComponentProps name="tariq"/>

</template>

<script>
import studentComponentProps from './studentComponentProps.vue';
import teacherComponentProps from './teacherComponentProps.vue';
export default {
    components:{
        studentComponentProps,
        teacherComponentProps
    }
}
</script>