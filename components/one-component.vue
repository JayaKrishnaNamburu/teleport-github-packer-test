<template>
  <div data-static-attr="test" :data-dynamic-attr="title">
    <span>Hello World!{{title}}</span>
    <span v-for="(item, index) in items" :key="index">
      {{item}}
      <ul>
        <li v-for="(item, index) in items" :key="index">{{item}}</li>
      </ul>
    </span>
    <span v-if="title === 'matching'">Now you see me!</span>
    <video autoplay>
      <source src="https://www.quirksmode.org/html5/videos/big_buck_bunny.mp4" type="video/mp4" />
      This browser does not support the video formats given
    </video>
    <slot></slot>
    <nuxt-link to="/about">About Page</nuxt-link>
  </div>
</template>

<script>
export default {
  name: 'OneComponent',
  props: {
    title: {
      type: String,
      default: 'Hello',
    },
    items: {
      type: Array,
      default: [],
    },
  },

  data() {
    return {
      isVisible: true,
      items: ['angular', 'react', 'vue'],
    }
  },
}
</script>
