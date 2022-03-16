<template>
  <div>
    <div class="container">
      <h1>Tabla de Usuarios</h1>
      <table class="table">
        <thead>
          <tr>
            <th>#</th>
            <th>Nombre</th>
            <th>Apellido</th>
            <th>RUN</th>
            <th>Nacimiento</th>
            <th>Edad</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="(persona,i) in personas" :key="i">
            <td>{{persona.id}}</td>
            <td>{{persona.nombre}}</td>
            <td>{{persona.apellido}}</td>
            <td>{{persona.run}}</td>
            <td>{{persona.nacimiento}}</td>
            <td>{{persona.edad}}</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>

<script>


export default {
  name: 'App',
  data(){
    return{
      personas:[
        {
          id:'1',
          nombre:"Jorge",
          apellido:"Solis",
          run:'17783008-9',
          nacimiento:'19-05-1991',
          edad:'30'
        },
        {
          id:'2',
          nombre:"Pamela",
          apellido:"Solis",
          run:'13074066-9',
          nacimiento:'28-06-1976',
          edad:'46'
        },
        {
          id:'3',
          nombre:"Powder",
          apellido:"Solis",
          run:'17783008-9',
          nacimiento:'01-10-2021',
          edad:'1'
        },
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
