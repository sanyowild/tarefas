<template>
  <div id="app">
  <h1>tarefas</h1> 
  <taskgrid :tasks="tasks"/>
    
  </div>
</template>

<script>
import taskgrid from './components/taskgrid.vue'

export default {
  components: {taskgrid},
  name: 'app',
  data(){
    return{
      tasks:[
        {name:'comprar remedio',pending:false},
        {name:'passear com o cachorro',pending:true}
        ]

    }
  }
}
</script>

<style>
body{
background: #F7971E;  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, #FFD200, #F7971E);  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, #FFD200, #F7971E); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
}

#app{
  display: flex;
  flex: 1;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

#app h1{
  margin-bottom: 5px;
  font-weight: 300;
  font-size: 5rem;
}
</style>
