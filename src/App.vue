<script setup>
  
  import Login from './components/Login.vue'
  import Main from './components/Main.vue'
  import Inventory from './components/Inventory.vue'
  import History from './components/History.vue'
  import AddProduct from './components/AddProduct.vue'
  import { ref } from 'vue'
  
  let scene = ref('login');
  
  
</script>

<template>

  <button @click="scene = 'login'">Login</button>
  <button @click="scene = 'menu'">Main</button>
  <button @click="scene = 'inventory'">Inventory</button>
  <button @click="scene = 'history'">History</button>
  <button @click="scene = 'addproduct'">Add Product</button>
  
  <Login v-if="scene === 'login'"/>
  <Main v-if="scene === 'menu'"/>
  <Inventory v-if="scene === 'inventory'"/>
  <History v-if="scene === 'history'"/>
  <AddProduct v-if="scene === 'addproduct'"/>
  
  

</template>

<style scoped>
</style>
