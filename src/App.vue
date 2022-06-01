<template>
<h1>POST Method API</h1>
  <input type="text" name="email" v-model="email" /> <br /> <br />
  <input type="password" name="password" v-model="password" /> <br /> <br />
  <button v-on:click="addUser()">Add User</button>
</template>

<script>
import axios from 'axios'
export default {
  name: 'App',
  data(){
    return{
      email: '',
      password: ''
    }
  },
  methods: {
    async addUser(){
      console.log(this.email, this.password);
      
      let result = await axios.post("http://localhost:3000/users",{
        email:this.email,
        password:this.password
      });
      console.log("result", result);
    }
  }

}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
