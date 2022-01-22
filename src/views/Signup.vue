<template>
  <div class="signup">
    <h1>This is an Signup Page</h1>
    <form action="">
      <input type="email" placeholder="Email id" v-model="form.email">
      <input type="password" placeholder="Password" v-model="form.password">
      <button>Signup</button>
      <p>{{form.email}}</p>
      <p>{{form.password}}</p>
    </form>
  </div>
</template>
<script>
export default {
  data() {
    return{
      form:{
        email:'',
        password:''
      }
    }
  },
  methods:{
    signup(){

    }
  }
}
</script>
<style scoped>
.signup{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.signup form input{
  padding: 12px 25px;
  border: 1px solid #cccccc;
  display: block;
  margin: 15px 0;
}
.signup form button{
  background-color: rgb(187, 24, 24);
  color: #ffffff;
  padding: 12px 25px;
  font-size: 18px;
  border: none;
  border-radius: 4px;
  width:100%;
  cursor: pointer;
}
.signup form button:hover{
  opacity: 0.7;
}
</style>
