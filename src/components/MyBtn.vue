<template>
  <div class="btn">
    <slot />
  </div>
  <h1 @dblclick="$emit('heropy',$event)">
    ABC
  </h1>
  <input
    type="text"
    v-model="msg" />
</template>

<script>
export default {
  emits: [
    'heropy',
    'changeMsg'
  ],
  data(){
    return {
      msg: ''
    }
  },
  watch: {
    msg(){
      this.$emit('changeMsg', this.msg)
    }
  }
}
</script>

<style scoped lang="scss">
.btn {
  display: inline-block;
  margin: 4px;
  padding: 6px 12px;
  border-radius: 4px;
  background-color: gray;
  color: white;
  cursor: pointer;
}
</style>