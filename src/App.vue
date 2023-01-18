<template>
  <Hello ref="hello" />
</template>

<script>
import Hello from '~/components/Hello'
export default {
  components: {
    Hello
  },
  mounted() {
    console.log('mounted:', this.$refs.hello.$refs.good)
  }
}
</script>