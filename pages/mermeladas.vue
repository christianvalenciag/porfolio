<template>
  <div class="container_body">
    <Title class="titulo" :titleprop="title"> </Title>
    <div class="texto_corrido_inicial">
      Las mermeladas de HACENDADO eran poco ergonómicas y la etiqueta con poco
      caracter. El diseño se centra en renovar la marca y rediseñar las
      etiquetas y envases, atendiendo a valores, ergonomia y otros aspectos del
      diseño.
    </div>
    <div class="img_merme">
        <img src="/img/mermeladas/1_mermelada.jpg" alt="">
    </div>
    <div class="img_merme">
        <img src="/img/mermeladas/3_mermeladas.jpg" alt="">
    </div>
    <div class="img_confit">
        <img src="/img/mermeladas/confitura.jpg" alt="">
    </div>
  </div>
</template>

<script>
import Header from "../components/Header.vue";
import Title from "../components/Title.vue";
export default {
  components: { Header, Title },
  data() {
    return {
      title: '<span class="pink">Rediseño</span><br /> Mermeladas HACENDADO.',
    };
  },
};
</script>

<style lang="scss" scoped >
.container_body {
  
  margin: 2.5rem 6rem 1rem 6rem;
  display: grid;
  grid-template-columns: 50% 50%;
  .titulo {
    grid-column-start: 1;
    grid-column-end: 3;
  }
  .texto_corrido_inicial {
    grid-column-start: 1;
    grid-column-end: 3;
    position: relative;
    margin-top: 2rem;
    width: 30rem;
    .subtitle {
      font-size: 1.3rem;
      font-weight: bold;
    }
  }
  .img_merme{
      margin-top: 2rem;
      margin-left: -6rem;
    grid-column-start: 1;
    grid-column-end: 3;
      width: 90rem;
      img{
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: center;
      }
  }
  .img_confit{
      margin-top: 2rem;
      margin-left: 13%;
      grid-column-start: 1;
      grid-column-end: 3;
      width: 60rem;
      img{
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: center;
      }
  }
}
@media screen and (max-width: 1420px) {
  .container_body {
    .titulo {
    }
    .img_merme{
        margin-top: 2rem;
        margin-left: -6rem;
      grid-column-start: 1;
      grid-column-end: 3;
        width: 89rem;
    }
    .img_confit{
        margin-top: 2rem;
        margin-left: 13%;
        grid-column-start: 1;
        grid-column-end: 3;
        width: 58rem;
    }
  }
}
@media screen and (max-width: 1390px) {
  .container_body {
    .titulo {
    }
    .img_merme{
        margin-top: 2rem;
        margin-left: -6rem;
      grid-column-start: 1;
      grid-column-end: 3;
        width: 87rem;
    }
    .img_confit{
        margin-top: 2rem;
        margin-left: 13%;
        grid-column-start: 1;
        grid-column-end: 3;
        width: 56.5rem;
    }
  }
}
@media screen and (max-width: 1350px) {
  .container_body {
    .titulo {
    }
    .img_merme{
        margin-top: 2rem;
        margin-left: -6rem;
      grid-column-start: 1;
      grid-column-end: 3;
        width: 85rem;
    }
    .img_confit{
        margin-top: 2rem;
        margin-left: 13%;
        grid-column-start: 1;
        grid-column-end: 3;
        width: 55rem;
    }
  }
}
@media screen and (max-width: 1325px) {
  .container_body {
    .titulo {
    }
    .img_merme{
        margin-top: 2rem;
        margin-left: -6rem;
      grid-column-start: 1;
      grid-column-end: 3;
        width: 83rem;
    }
    .img_confit{
        margin-top: 2rem;
        margin-left: 13%;
        grid-column-start: 1;
        grid-column-end: 3;
        width: 53.5rem;
    }
  }
}
@media screen and (max-width: 1295px) {
  .container_body {
    .titulo {
    }
    .img_merme{
        margin-top: 2rem;
        margin-left: -6rem;
      grid-column-start: 1;
      grid-column-end: 3;
        width: 81rem;
    }
    .img_confit{
        margin-top: 2rem;
        margin-left: 13%;
        grid-column-start: 1;
        grid-column-end: 3;
        width: 52rem;
    }
  }
}
@media screen and (max-width: 1265px) {
  .container_body {
    .titulo {
    }
    .img_merme{
        margin-top: 2rem;
        margin-left: -6rem;
      grid-column-start: 1;
      grid-column-end: 3;
        width: 79rem;
    }
    .img_confit{
        margin-top: 2rem;
        margin-left: 13%;
        grid-column-start: 1;
        grid-column-end: 3;
        width: 51.5rem;
    }
  }
}
@media screen and (max-width: 1235px) {
  .container_body {
    .titulo {
    }
    .img_merme{
        margin-top: 2rem;
        margin-left: 0rem;
      grid-column-start: 1;
      grid-column-end: 3;
        width: 65rem;
    }
    .img_confit{
        margin-top: 2rem;
        margin-left: 13%;
        grid-column-start: 1;
        grid-column-end: 3;
        width: 46rem;
    }
  }
}
@media screen and (max-width: 1175px) {
  .container_body {
    .titulo {
    }
    .img_merme{
        margin-top: 2rem;
        margin-left: 0rem;
      grid-column-start: 1;
      grid-column-end: 3;
        width: 60rem;
    }
    .img_confit{
        margin-top: 2rem;
        margin-left: 13%;
        grid-column-start: 1;
        grid-column-end: 3;
        width: 44rem;
    }
  }
}
@media screen and (max-width: 1090px) {
  .container_body {
    .titulo {
    }
    .img_merme{
        margin-top: 2rem;
        margin-left: 0rem;
      grid-column-start: 1;
      grid-column-end: 3;
        width: 55rem;
    }
    .img_confit{
        margin-top: 2rem;
        margin-left: 13%;
        grid-column-start: 1;
        grid-column-end: 3;
        width: 42rem;
    }
  }
}
@media screen and (max-width: 1000px) {
  .container_body {
    .titulo {
    }
    .img_merme{
        margin-top: 2rem;
        margin-left: 0rem;
      grid-column-start: 1;
      grid-column-end: 3;
        width: 50rem;
    }
    .img_confit{
        margin-top: 2rem;
        margin-left: 13%;
        grid-column-start: 1;
        grid-column-end: 3;
        width: 38rem;
    }
  }
}
@media screen and (max-width: 947px) {
  .container_body {
    margin: 2.5rem 1rem 1rem 1rem;
  display: grid;
  grid-template-columns: 50% 50%;
  .titulo {
    grid-column-start: 1;
    grid-column-end: 3;
    font-size: 2rem;
  }
    .img_merme{
        margin-top: 2rem;
        margin-left: 0rem;
      grid-column-start: 1;
      grid-column-end: 3;
        width: 55rem;
    }
    .img_confit{
        margin-top: 2rem;
        margin-left: 13%;
        grid-column-start: 1;
        grid-column-end: 3;
        width: 39rem;
    }
  }
}
@media screen and (max-width: 910px) {
  .container_body {
  .titulo {
  }
    .img_merme{
        margin-top: 2rem;
        margin-left: 0rem;
      grid-column-start: 1;
      grid-column-end: 3;
        width: 50rem;
    }
    .img_confit{
        margin-top: 2rem;
        margin-left: 13%;
        grid-column-start: 1;
        grid-column-end: 3;
        width: 35rem;
    }
  }
}
@media screen and (max-width: 840px) {
  .container_body {
  .titulo {
  }
    .img_merme{
        margin-top: 2rem;
        margin-left: 0rem;
      grid-column-start: 1;
      grid-column-end: 3;
        width: 45rem;
    }
    .img_confit{
        margin-top: 2rem;
        margin-left: 0;
        grid-column-start: 1;
        grid-column-end: 3;
        width: 45rem;
    }
  }
}
@media screen and (max-width: 750px) {
  .container_body {
  .titulo {
  }
    .img_merme{
        margin-top: 2rem;
        margin-left: 0rem;
      grid-column-start: 1;
      grid-column-end: 3;
        width: 40rem;
    }
    .img_confit{
        margin-top: 2rem;
        margin-left: 0%;
        grid-column-start: 1;
        grid-column-end: 3;
        width: 40rem;
    }
  }
}
@media screen and (max-width: 675px) {
  .container_body {
  .titulo {
  }
    .img_merme{
        margin-top: 2rem;
        margin-left: 0rem;
      grid-column-start: 1;
      grid-column-end: 3;
        width: 35rem;
    }
    .img_confit{
        margin-top: 2rem;
        margin-left: 0;
        grid-column-start: 1;
        grid-column-end: 3;
        width: 35rem;
    }
  }
}
@media screen and (max-width: 600px) {
  .container_body {
  .titulo {
  }
    .img_merme{
        margin-top: 2rem;
        margin-left: -4rem;
      grid-column-start: 1;
      grid-column-end: 3;
        width: 40.5rem;
    }
    .img_confit{
        margin-top: 2rem;
        margin-left: -1rem;
        grid-column-start: 1;
        grid-column-end: 3;
        width: 38rem;
    }
  }
}
@media screen and (max-width: 590px) {
  .container_body {
  .titulo {
  }
    .img_merme{
        margin-top: 2rem;
        margin-left: -4rem;
      grid-column-start: 1;
      grid-column-end: 3;
        width: 40rem;
    }
    .img_confit{
        margin-top: 2rem;
        margin-left: -1rem;
        grid-column-start: 1;
        grid-column-end: 3;
        width: 37rem;
    }
  }
}
@media screen and (max-width: 580px) {
  .container_body {
  .titulo {
    
  }
    .img_merme{
        margin-top: 2rem;
        margin-left: -4rem;
      grid-column-start: 1;
      grid-column-end: 3;
        width: 39.3rem;
    }
    .img_confit{
        margin-top: 2rem;
        margin-left: -1rem;
        grid-column-start: 1;
        grid-column-end: 3;
        width: 38rem;
    }
  }
}
@media screen and (max-width: 570px) {
  .container_body {
  .titulo {
    
  }
    .img_merme{
        margin-top: 2rem;
        margin-left: 0rem;
      grid-column-start: 1;
      grid-column-end: 3;
        width: 33rem;
    }
    .img_confit{
        margin-top: 2rem;
        margin-left: 0rem;
        grid-column-start: 1;
        grid-column-end: 3;
        width: 33rem;
    }
  }
}
@media screen and (max-width: 530px) {
  .container_body {
  .titulo {
    
  }
  .texto_corrido_inicial {
    width: 20rem;
  }
    .img_merme{
        margin-top: 2rem;
        margin-left: 0rem;
      grid-column-start: 1;
      grid-column-end: 3;
        width: 29rem;
    }
    .img_confit{
        margin-top: 2rem;
        margin-left: 0rem;
        grid-column-start: 1;
        grid-column-end: 3;
        width: 29rem;
    }
  }
}
@media screen and (max-width: 490px) {
  .container_body {
  .titulo {
    
  }
  .texto_corrido_inicial {
    width: 20rem;
  }
    .img_merme{
        margin-top: 2rem;
        margin-left: 0rem;
      grid-column-start: 1;
      grid-column-end: 3;
        width: 24rem;
    }
    .img_confit{
        margin-top: 2rem;
        margin-left: 0rem;
        grid-column-start: 1;
        grid-column-end: 3;
        width: 24rem;
    }
  }
}
@media screen and (max-width: 400px) {
  .container_body {
  .titulo {
    
  }
  .texto_corrido_inicial {
    width: 20rem;
  }
    .img_merme{
        margin-top: 2rem;
        margin-left: -3rem;
      grid-column-start: 1;
      grid-column-end: 3;
        width: 27rem;
    }
    .img_confit{
        margin-top: 2rem;
        margin-left: -1rem;
        grid-column-start: 1;
        grid-column-end: 3;
        width: 25rem;
    }
  }
}
@media screen and (max-width: 390px) {
  .container_body {
  .titulo {
    font-size: 1.7rem;
  }
  .texto_corrido_inicial {
    width: 20rem;
  }
    .img_merme{
        margin-top: 2rem;
        margin-left: -3rem;
      grid-column-start: 1;
      grid-column-end: 3;
        width: 26.4rem;
    }
    .img_confit{
        margin-top: 2rem;
        margin-left: -1rem;
        grid-column-start: 1;
        grid-column-end: 3;
        width: 24.5rem;
    }
  }
}
@media screen and (max-width: 380px) {
  .container_body {
  .titulo {
    
  }
    .img_merme{
        width: 25.75rem;
    }
    .img_confit{
        width: 24rem;
    }
  }
}
@media screen and (max-width: 375px) {
  .container_body {
  .titulo {
    
  }
    .img_merme{
        width: 25.45rem;
    }
    .img_confit{
        width: 23.6rem;
    }
  }
}
@media screen and (max-width: 370px) {
  .container_body {
  .titulo {
    
  }
    .img_merme{
        width: 25.25rem;
    }
    .img_confit{
        width: 23.5rem;
    }
  }
}
@media screen and (max-width: 365px) {
  .container_body {
  .titulo {
    
  }
    .img_merme{
        width: 24.8rem;
    }
    .img_confit{
        width: 23.2rem;
    }
  }
}
@media screen and (max-width: 360px) {
  .container_body {
  .titulo {
    
  }
    .img_merme{
        width: 24.5rem;
    }
    .img_confit{
        width: 23rem;
    }
  }
}
@media screen and (max-width: 355px) {
  .container_body {
  .titulo {
    
  }
    .img_merme{
        width: 24.2rem;
    }
    .img_confit{
        width: 22.8rem;
    }
  }
}

</style>