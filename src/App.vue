<template>
  <div id="app">
    <Vista/>
    <h2><i>RESPUESTAS</i></h2>
        <div class="table responsive">
          <table class="table table-dark">
            <tr>
              <th>Pregunta</th>
              <th>Respuesta</th>
            </tr>
            <tr>
             <th>1</th>
             <th>B</th>
            </tr>
            <tr>
             <th>2</th>
             <th>C</th>
            </tr>
            <tr>
             <th>3</th>
             <th>A</th>
            </tr>
            <tr>
             <th>4</th>
             <th>C,D</th>
            </tr>
            <tr>
             <th>5</th>
             <th>A</th>
            </tr>
            

            
            
          </table>
      </div>
  </div>
</template>

<script>
import Vista from './components/Vista.vue'

export default {
  name: 'App',
  components: {
    Vista
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
