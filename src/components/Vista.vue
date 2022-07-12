<template>

  <section class="src-components-vista">

   <label for="color">Color:</label>
   <input type="text" name="color" id="color" v-model="color">

   <label for="fondo">Fondo:</label>
   <input type="text" name="fondo" id="fondo" v-model="fondo">

   <label for="size">Size:</label>
   <input type="text" name="size" id="size" v-model="size">

   <br><br><hr>

   <label for="text">Texto:</label>
   <input type="text" name="texto" id="texto"  :style="{ background:fondo, color: color, fontSize:size }" v-model.trim="texto">

  <p v-if="texto!=''">Cantidad de palabras : {{contarPalabras}}</p>
  

  </section>

</template>

<script>

  export default  {
    name: 'src-components-vista',
    props: [],
    mounted () {

    },
    data () {
      return {
        color:'red',
        fondo:'pink',
        size:'15px',
        texto:'',
        cant:0
      }
    },
    methods: {

    },
    computed: {
      contarPalabras(){
        let cont=0
        const arrayPalabras = this.texto.split(' ')
        console.log(arrayPalabras);
        for (let i = 0; i < arrayPalabras.length; i++) {
          cont++;
        }
        return cont
      }
    }
}


</script>

<style scoped lang="css">
  .src-components-vista {
    
  }
  hr {
    background-color: #bbb;
  }
</style>
