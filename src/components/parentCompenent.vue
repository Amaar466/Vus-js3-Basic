<template>
<h1>Pass Data Parent to Child</h1>
<childComponent name="Amaar ul haq" :user="user"  :getData="getData"/>
</template>

<script>
import childComponent from './childComponent.vue';
export default {
    name:'parentComponent',
    components:{
        childComponent
    },
    data() {
        return {
            user:{name:'bilal', email:'bilal@gmail.com'},
        }
    },
    methods: {
        getData(){
            console.warn('Parent Function Called');
        }
    },
}
</script>