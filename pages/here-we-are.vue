<template>
  <div class="container">
    <Navbar></Navbar>
    Page 3
    <OneComponent></OneComponent>
  </div>
</template>

<script>
import Navbar from '../components/navbar'
import OneComponent from '../components/one-component'

export default {
  name: 'Us',
  components: {
    Navbar,
    OneComponent,
  },
}
</script>

<style>
.container {
  border: 1px solid black;
  padding: 1px solid black;
}
</style>
