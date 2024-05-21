<template>
    <div>
        <h1>Reuse Component</h1>
        <ul>
            <li v-for="item in users" :key="item.name">
                <userComponent :data="item" :getData="getData"/>
            </li>
        </ul>
    </div>
</template>

<script>
import userComponent from './userComponent.vue';

export default {
    name: 'reuseComponent',
    components: {
        userComponent,
    },
    methods: {
        getData(name){
            alert(name);
        }
    },
    data() {
        return {
            users: [{
                    name: 'amaar',
                    email: 'amaar@gmail.com',
                    phoneNo: '19454354'
                },
                {
                    name: 'amaar123',
                    email: 'amaar123@gmail.com',
                    phoneNo: '19454354'
                },
                {
                    name: 'amaar32453',
                    email: 'amaa2354325r@gmail.com',
                    phoneNo: '19454354'
                }
            ]
        }
    },
}
</script>
