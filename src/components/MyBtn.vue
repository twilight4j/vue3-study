<template>
  <div class="btn">
    <slot name="icon" />
    <slot name="text" />
  </div>
</template>

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