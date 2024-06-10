<template>
    <img class = "logo" src="@/assets/resturant.png" alt="">
    <h2>Sign Up</h2>

    <div class="register">
        <input type="text" placeholder="Enter Name" v-model="name"/>
        <input type="text" placeholder="Enter Email" v-model="email"/>
        <input type="password" placeholder="Enter Password" v-model="password"/>
        <button @click="signUp">Sign Up</button>
    </div>
</template>

<script>
export default {
    name : 'SignUp',

    data() {
        return {
            name: '',
            email: '',
            password: ''
        };
    },
    methods: {
        signUp() {
            console.log('Signing up');
        }
    }
}
</script>

<style>

.logo{
width: 100px;
}

.register input {
    width: 300px;
    height: 40px;
    padding-left: 20px;
    display: block;
    margin-bottom: 30px;
    margin-left: auto;
    margin-right: auto;
    border: 1px solid skyblue;
}
.register button{
    width: 320px;
    height: 40px;
    border: 1px solid skyblue;
    background-color: skyblue;
    cursor: pointer;
    color: white;
}
</style>