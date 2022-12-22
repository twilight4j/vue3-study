<template>
  <button @click="handlerA(), handerB()">
    Click me
  </button>
</template>

<script>
export default {
  data() {
    return {
    }
  },
  methods: {
    handlerA() {
      console.log('A')
    },
    handlerB() {
      console.log('B')
    }
  }
}
</script>