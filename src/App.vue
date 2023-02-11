<script setup>
import {ref} from 'vue'
import Navbar from './components/Navbar.vue'
import Footer from './components/Footer.vue'

let num = ref(0)

</script>

<template>
  <!-- NAVBAR -->
  <Navbar/>

  <Footer></Footer>
</template>

<style>
body{
  overflow: hidden;
  min-height: 100vh;
  background: rgb(106,196,233);
  background: linear-gradient(0deg, rgba(106,196,233,0.9360119047619048) 0%, rgba(0,41,150,1) 100%);
}
footer{
  position: fixed;
  bottom: 0;
  width: 100%;
  display: flex;
  align-items:center;
  justify-content: center;
  height: 56px;
}
@media (max-width: 600px) {
  body{
    overflow: auto;
  }
}
</style>