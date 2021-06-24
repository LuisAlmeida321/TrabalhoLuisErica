<template>
  <v-carousel
    cycle
    height="90%"
    hide-delimiter-background
    show-arrows-on-hover
    class="carousel"
  >
    <v-carousel-item
      v-for="(slide, i) in slides"
      :key="i"
    >
        <v-row
          class="fill-height"
          align="center"
          justify="center"
        >
          <img :src="slide.imagem ">
        </v-row>
    </v-carousel-item>
  </v-carousel>
</template>

<script>


import axios from "axios";

export default {
  data(){
    return{
       slides:[]
    }
  },
  components: {

  }, 
  mounted(){
    axios
     .get("https://blogjogos-86479-default-rtdb.firebaseio.com/.json")
     .then(response => (this.slides = response.data.data));

  
  },
  }

</script>


<style>
.letras{
  color: black;
}
.carousel{
  background-color: black;
}

</style>