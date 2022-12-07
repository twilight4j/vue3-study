<template>
  <div>
    <span>{{ comma('2222') }}</span>
  </div>
</template>
 
<script scoped>
import {computed} from 'vue'
export default {
 setup(){
  const comma = computed(()=>{
    return (val)=>{
       return String(val).replace(/\B(?=(\d{3})+(?!\d))/g, ",")
     }
  }) 
  return {
    comma
  }
 }
}
</script>