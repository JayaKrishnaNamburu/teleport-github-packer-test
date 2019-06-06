<template>
  <div class="container">
    <Navbar></Navbar>
    Page 2
  </div>
</template>

<script>
import Navbar from '../components/navbar'

export default {
  name: 'About',
  components: {
    Navbar,
  },
}
</script>

<style>
.container {
  border: 1px solid black;
  padding: 1px solid black;
}
</style>
