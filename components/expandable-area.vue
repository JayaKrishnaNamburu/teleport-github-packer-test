<template>
  <div class="container">
    <span>{{title}}</span>
    <button @click="isExpanded = !isExpanded">
      <span v-if="isExpanded">Hide me</span>
      <span v-if="!isExpanded">Show me</span>
    </button>
    <span v-if="isExpanded">{{text}}</span>
  </div>
</template>

<script>
export default {
  name: 'ExpandableArea',
  props: {
    title: {
      type: String,
      default: 'Hello',
    },
    text: {
      type: String,
      default: "Is it me you're looking for?",
    },
  },

  data() {
    return {
      isExpanded: false,
    }
  },
}
</script>

<style>
.container {
  border: 1px solid green;
  margin: 10px;
}
</style>
