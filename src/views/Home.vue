<template>
  <div class="container">
    <div class="signin">
      <h1>Signin Form</h1>
      <form action="" @submit.prevent="submit">
        <input type="email" placeholder="Email id" v-model="form.email"/>
        <input type="password" placeholder="Password" v-model="form.password"/>
        <button type="submit">Signin</button>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
  data() {
    return{
      form:{
        email:'',
        password:''
      }
    }
  },
  methods:{
    signin(){
      
    }
  }
};
</script>
<style scoped>
.signin {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  box-shadow: 0px 0px 12px 0px rgba(0, 0, 0, 0.1);
}
.signin form input {
  display: block;
  margin: 20px 0;
  padding: 12px 25px;
  border: 1px solid #cccccc;
  border-radius: 4px;
}
.signin form button {
  padding: 12px 25px;
  background-color: #18ac18;
  color: #ffffff;
  font-size: 18px;
  width: 100%;
  border: none;
  cursor: pointer;
}
.signin form button:hover {
  opacity: 0.7;
}
</style>
