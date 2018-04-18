<template>
  <div class="child">
      <p>子组件</p>
      <p>{{count}}</p>
  </div>
</template>

<script>
export default {
  data(){
      return {
          
      }
  },
  props: ['count']
}
</script>


<style scoped>
    .child{
        border: 1px solid green;
        width: 80%;
        margin: 0 auto;
    }
</style>
