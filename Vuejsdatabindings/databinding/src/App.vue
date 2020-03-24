<template>
<div>
  <h1>{{title}}</h1>
    <input type="text" v-on: input="changeTitle">
</div>
  
</template>

<script>
export default {
  data:() => {
    return {
      title:'Good Morning'
    }
  },
  methods: {
    changeTitle(event){
      this.title =event.data.changeTitle;
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
