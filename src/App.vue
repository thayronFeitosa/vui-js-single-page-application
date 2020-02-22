<template>
<div>
<h1>{{ titulo }}</h1>


<ul>
  <li v-for="foto of fotos">

    <img :src="foto.url" alt="foto.tutulo">
  </li>


  <img src="" alt="">
</ul>

</div>

</template>

<script>
export default {

  data () {
    return {
    titulo: 'alura pic',
    fotos:[
      
      {
        url: 'https://lh3.googleusercontent.com/proxy/tpJS9gOy2lsW9Yi9b_3HUTjP4l7PDp5sW7lDfzzZsAfPChj0WC73Q31diJ8qC4JqZmnIguV5a1hkT1hcLVypKs6C08fKivAeo82-_z2o75CKH10vTOsrv5nk7WKZcnEsIA',
        titulo: 'cachorro'
      }, 
    {
      url: 'https://lh3.googleusercontent.com/proxy/tpJS9gOy2lsW9Yi9b_3HUTjP4l7PDp5sW7lDfzzZsAfPChj0WC73Q31diJ8qC4JqZmnIguV5a1hkT1hcLVypKs6C08fKivAeo82-_z2o75CKH10vTOsrv5nk7WKZcnEsIA',
      titulo: 'cachorro'
    }

    ]
    
    }

  }
}
</script>

<style>
 
</style>
