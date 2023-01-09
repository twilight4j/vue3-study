<template>
  <input
    type="text"
    @keydown="handler" />
</template>

<script>
export default {
  methods: {
    handler(event) {
        console.log(event)
      // console.log('Enter!!')
      
    }
  }
}
</script>
