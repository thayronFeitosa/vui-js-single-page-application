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

    ]
    
    }

  },
  created(){
   let promise = this.$http.get('http://localhost:3000/v1/fotos');

  promise.then(res =>{
    res.json().then(fotos => this.fotos= fotos);

  });
}
}
</script>

<style>
 
</style>
