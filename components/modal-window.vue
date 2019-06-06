<template>
  <div>
    {{message}}
    <button @click="handleCloseClick">Close me</button>
  </div>
</template>

<script>
export default {
  name: 'ModalWindow',
  props: {
    message: {
      type: String,
      default: 'Hello',
    },
    onClose: {
      default: '() => {}',
    },
  },

  data() {
    return {
      fakeState: false,
    }
  },

  methods: {
    handleCloseClick() {
      this.$emit('onClose')
      this.fakeState = false
    },
  },
}
</script>
