<template>
    <h1>Form Component</h1>
    <ul>
        <li v-for="item in error" class="error" v-bind:key="item">
        {{ item }} not valid
        </li>
    </ul>
    <!-- <form > -->
    {{ form }}
    <br /><br />
    <label for="name">Name</label>
    <input type="text" name="name"  v-model="form.name" required>
    <br /><br />
    <label for="email">Email</label>
    <input type="text" name="email" v-model="form.email">
    <br /><br />
    <label for="password">Password</label>
    <input type="password" name="password" v-model="form.password">
    <br /><br />
    <input type="radio" v-model="form.picked" value="a" />
    <br /><br />
    <label>
        <input type="radio" value="male" name="gender" v-model="form.gender"> Male
    </label>
    <label>
        <input type="radio" value="female" name="gender" v-model="form.gender"> Female
    </label>
    <br /><br />
    <select v-model="form.selected">
        <option disabled value="">Please select one</option>
        <option>Lahore</option>
        <option>Karchi</option>
        <option>Islamabad</option>
    </select>
    <button type="submit" v-on:click="save">Submit</button>
    <!-- </form> -->
</template>

<script>
// import { ref } from 'vue';
export default {
    data() {
        return {
            form: {
                name: '',
                email: '',
                password: '',
                selected: '',
                picked: '',
                gender: ''
            },
            error: []

        }
    },
    methods: {
        save() {
            this.error = [];
            for (const item in this.form) {
                if (this.form[item] === "") {
                    this.error.push(item);
                }
            }
            if (this.error.length === 0) {
                console.warn('Data saved:', this.name, this.email, this.selected, this.picked, this.gender);
            } else {
                console.warn('Please fill in all required fields:', this.error);
            }
        }
    }


}
</script>
<style scoped>
.error{
    color: red;
}
</style>

