<template>
  <!-- <MyBtn
    class="heropy"
    style="color: red;"
    color="##ff000"
    @hello="log">
    Apple
  </MyBtn> -->
  <h1>branch_test</h1>
  <div>
    <span>{{ comma('1234') }}</span>
  </div>
  <h1>composition api</h1>
  <Compositive />
</template>
 
 <script>
 import MyBtn from '~/components/MyBtn'
 import Compositive from '~/components/Compositive'
 export default {
  components: {
    MyBtn, 
    Compositive
  },
  computed:{
    comma(){
      return (val)=>{
        return String(val).replace(/\B(?=(\d{3})+(?!\d))/g, ",")
      }
    }
  }
}
</script>