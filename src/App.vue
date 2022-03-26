<template>
<h1>{{ title }}</h1>
<ul>
  <li v-for="task in tasks" :key="task.id">
    {{ task.id }}. {{ task.name }}
  </li>
</ul>
</template>

<script>

export default {
  data(){
    return{
      title: 'My To-Do App',
      tasks:[
        { id: 1, name: 'Learn Vue', finished: false},
        { id: 2, name: 'Build Vue', finished: false},
        { id: 3, name: 'Build  o-Do App', finished: false},
      ]
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
