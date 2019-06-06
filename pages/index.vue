<template>
  <div class="container">
    <Navbar></Navbar>
    Page 1
  </div>
</template>

<script>
import Navbar from '../components/navbar'

export default {
  name: 'Home',
  components: {
    Navbar,
  },
}
</script>

<style>
.container {
  border: 1px solid green;
  padding: 10px;
}
</style>
