<template>
    <h1>For Loops</h1>
    <ul>
        <li v-for="item in technology" :key="item">
            {{ item }}
        </li>
    </ul>

    <ul>
        <li v-for="item in user" :key="item.name">
           Name::{{item.name}} and Email is {{ item.email }}
        </li>
    </ul>
</template>

<script>
export default {
    data() {
        return {
            technology: ["html", "php", "laravel"],
            user: [{
                name: 'Amaar',
                email: 'amaar@gmail.com'
            }
                ,
            {
                name: 'hadi',
                email: 'hadi@gmail.com'
            },
            {
                name: 'arslan',
                email: 'arslan@gmail.com'
            }
        ]
        }
    },
}
</script>