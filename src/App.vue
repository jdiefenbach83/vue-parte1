<template>
<div>
  <h1 v-text="titulo"></h1>
  <ul>
    <li v-for="foto of fotos" :key="foto.titulo">
      <img :src="foto.url" :alt="foto.titulo">
    </li>    
  </ul>
</div>
</template>

<script>
export default {
  data() {
    return {
      titulo: 'Alura Pic',
      fotos: [
        {
          url: 'https://academiawashington.com.br/wp-content/uploads/2017/09/coisas-incriveis-sobre-seu-cachorro.jpg',
          titulo: 'cachorro'
        },
        {
          url: 'https://academiawashington.com.br/wp-content/uploads/2017/09/coisas-incriveis-sobre-seu-cachorro.jpg',
          titulo: 'Cachorrão'
        }
      ]
    }
  }  
}
</script>

<style>

</style>
