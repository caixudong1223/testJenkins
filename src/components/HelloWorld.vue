<template>
  <div class="hello">
    <router-link to="/parent/child">子组件/child</router-link>
    <p>
      hahahaahahah
    </p>
    <h1>{{ msg }}</h1>
    <p>{{count}}</p>
    <router-view :count="count"></router-view>
    
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: '父组件',
      count: 0
    }
  },
  created(){
    this.setTimer()
  },
  mounted(){
    
  },
  methods: {
    setTimer(){
      setInterval(() => {  
        this.count++;
      }, 1000)
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}

.hello{
  border: 1px solid #ccc;
}

</style>
