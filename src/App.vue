<script setup>
import {ref} from "vue"

let count = ref(0)
</script>

<template>
  <main>
      <container class="container">
        <h4>the current count is...</h4>
        <h1>{{count}}</h1>  
        <div>        
        <button @click="count--">-</button>
        <button @click="count++">+</button>
        </div>   

 
      </container>
  </main>
</template>

<style scoped>

main {
  width: 100vw;
  height: 100vh;
  background-color: #F6D2E0;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: Arial, Helvetica, sans-serif;
}

.container {
  width: 50vw;
  height: 50vh;
  margin: 0;
  top:50%;
  left:50%;
  text-align: center;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}

button{
  padding: 15px 30px;
  font-size: 1em;
  font-style: bold;
  border: none;
  background-color: #C8E7F5;
  margin: 3px;
  color: white;
}
</style>