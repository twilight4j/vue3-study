<template>
  <button @click="add">
    ADD
  </button>
  <h1>{{ reversedMessage }}</h1>
  <h1>{{ reversedMessage }}</h1>
  <h1>{{ reversedMessage }}</h1>
  <h1>{{ reversedMessage }}</h1>
</template>


<script>
export default {
  data() {
    return {
      // Getter, Setter
      msg : 'Helo Computed!'
    }
  },
  computed: {
    // Getter
    // reversedMessage() {
    //   return this.msg.split('').reverse().join('')
    // }
    // Getter, Setter
    reversedMessage: {
      get() {
       return this.msg.split('').reverse().join('') 
      },
      set(value) {
        this.msg = value
      }
    }
  },
  methods: {
    add() {
      this.reversedMessage += '!?'
    }
  }
}</script>