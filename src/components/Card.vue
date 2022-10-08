<template>
<grid>
<img :src="url" alt="Vue.js" />
<h2>{{nombre}}</h2>
<br />
<a  :href="url" target="_blank">Descargar</a>
<a  :href="url" target="_blank">Visitar</a>
</grid>    
</template>

<script>
import Grid from "./Grid.vue";

export default{
  props: {
   url: {
    String,
   },
   nombre: {
     String,
   },
  },
};
</script>

<style scoped>

img{
    width: 8rem;
    height: 8rem;
    padding: 0.8rem;   
}

a{
    text-decoration: none;
    color:snow;
    background: #301675;
    padding: 0.3rem;
    border-radius: 5px;
    border: 1px solid #f2f2f2;
}

</style>