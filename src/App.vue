<template>
  <div class="main">
      <h1>Hello Friend</h1>
      <label for="name">Enter Name:</label>
      <input type="text" name="" id="name" v-model="username" @click="update">
      <button @click="deleteName">Delete</button>
      <p>Your Name is: <span>{{ username }}</span></p>
  </div>    
</template>

<script>
  export default{
  data(){
    return{
       username: '',
       default:'Daniyal'
    }
  },
  methods:{
    deleteName(){
      this.username=this.default;
    }
  }
}
</script>

<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app{
  align-items: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 335px 500px;
  background-color:darkcyan;
  color:white;
  font-size: 20px;  
}
p{
  width: fit-content;
  word-break: break-all;
  margin-top: 10px;
}
label{
  margin-right: 10px;
}
input{
  padding: 10px;
  outline: none;
  border: none;
  border-radius: 10px;
  margin-right: 10px;
  margin-top: 30qpx;
}
button{
  padding: 10px;
  outline: none;
  border: none;
  border-radius: 10px;
  color: aliceblue;
  background-color: gold
}
span{
  color:crimson;
  text-shadow: 1em
}


</style>
