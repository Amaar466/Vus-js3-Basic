<template>
<h2>Check Box and Radio Button</h2>
<label for="java">Java</label>
<input type="checkbox" value="java" id="java" v-model="technology" >
<label for="php">Php</label>
<input type="checkbox" value="php" id="php" v-model="technology">
<label for="laravel">Laravel</label>
<input type="checkbox" value="laravel" id="laravel" v-model="technology">
<br /> <br />

<h3>Who i am</h3>
<label for="student">Student</label>
<input type="radio" value="student" v-model="who" name="who" id="student" >

<label for="developer">Developer</label>
<input type="radio" value="developer" v-model="who" name="who" id="developer" >

<h4>Selected Technology::{{ technology }}</h4>
<h4>I am a ::{{ who }}</h4>

</template>


<script>
export default{
    name:'checkBox',
    data() {
        return {
            technology:[],
            who:null
        }
    },
}
</script>