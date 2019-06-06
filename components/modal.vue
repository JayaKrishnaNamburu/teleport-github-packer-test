<template>
  <template>
    <button @click="isOpen = true">Show Popup</button>
    <ModalWindow @onClose="isOpen = false" v-if="isOpen"></ModalWindow>
  </template>
</template>

<script>
import ModalWindow from './modal-window'

export default {
  name: 'Modal',
  components: {
    ModalWindow,
  },

  data() {
    return {
      isOpen: false,
    }
  },
}
</script>
