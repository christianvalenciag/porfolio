<template>
  <div class="container_body">
    <Title class="titulo" :titleprop="title"> </Title>
    <div class="texto_corrido_inicial">
      Esta revista nace desde la intención de comunicar a la ciudadanía sucesos
      sociales de gran controversia e injusticia. La idea parte desde la
      sobrieda y seriedad para crear una comunicación directa e impactante. Dos
      colores corporativos y muy visual.
    </div>
    <div class="texto_corrido_inicial">
      <div class="subtitle blue">MANIFIESTO</div>
      Esta revista nace con el propósito de informar, concienciar y
      denunciar hechos globales y nacionales. Desde FAKDEM somos conscientes de
      la manipulación que sufre la información en esta era digital. Con esta
      revista queremos sacar a la luz toda la verdad sin ningún tipo de
      maquillaje, de color. Está muy enfocada a temas sociales de actualidad.
      <br /><br /> 
      En esta revista, cada numero de dedicará a una sección concreta. Dicha
      sección tendrá relacionada una ONG a donde irá a destinados la recaudación
      por dicho número. La sección ultima, de dictada a artículos localizados en
      España en general, nunca será protagonista, por lo que no tiene ONG
      relacionada.
      <br /><br /> 
      Las ONG por sección, son: “Seguro que no eres homófobo porque
      tienes un amigo gay.”, los fondos para COGAM. “Ni machismo ni feminismo,
      igualdad?”, los fondos irán para OXFAM Intermón. “No eres racista,
      pero…?”, los fondos irán para FEDERACIÓN S.O.S. Racismo. “Yo amo las
      pieles vivas muertas, en abrigos…”, los fondos irán para ADDA. “El cambio
      climático es una invención de los chinos, obvio.” , los fondos irán para
      AMA.
    </div>
    <div class="img_revista">
        <img src="/img/revista/REVISTAS_PLIEGOS.png" alt="">
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
      title:
        '<span class="pink">Creación y diseño</span><br /> Revista FAKDEM.',
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
    margin-bottom: 2rem;
    .subtitle{
        font-size: 1.3rem;
        font-weight: bold;
    }
  }
  .img_revista{

      margin-left: -6rem;
    grid-column-start: 1;
    grid-column-end: 3;
      width: 95rem;
      img{
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: center;
      }
  }
}
@media screen and (max-width: 1304px) {
  .container_body {
  
    .img_revista{

      margin-left: -6rem;
    grid-column-start: 1;
    grid-column-end: 3;
      width: 85rem;
      img{
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: center;
      }
  }
  }
}
@media screen and (max-width: 1170px) {
  .container_body {
    
    .img_revista{

      margin-left: -6rem;
    grid-column-start: 1;
    grid-column-end: 3;
      width: 75rem;
      img{
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: center;
      }
  }
  }
}
@media screen and (max-width: 1030px) {
  .container_body {
    
    .img_revista{

      margin-left: -6rem;
    grid-column-start: 1;
    grid-column-end: 3;
      width: 65rem;
      img{
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: center;
      }
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
    .texto_corrido_inicial {
    grid-column-start: 1;
    grid-column-end: 3;
    position: relative;
    margin-top: 2rem;
    width: 30rem;
    margin-bottom: 2rem;
    .subtitle{
      margin-top: -2rem;
        font-size: 1.2rem;
        font-weight: bold;
    }
  }
    .img_revista{

      margin-left: -6rem;
    grid-column-start: 1;
    grid-column-end: 3;
      width: 65rem;
      img{
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: center;
      }
  }
  }
}
@media screen and (max-width: 847px) {
  .container_body {
    margin: 2.5rem 1rem 1rem 1rem;
    .titulo {
      font-size: 2rem;
    }
    .texto_corrido_inicial {
    margin-top: 2rem;
    width: 30rem;
    margin-bottom: 2rem;
    .subtitle{
      margin-top: -2rem;
        font-size: 1.2rem;
        font-weight: bold;
    }
  }
    .img_revista{

    margin-left: -6rem;
    grid-column-start: 1;
    grid-column-end: 3;
      width: 58rem;
      img{
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: center;
      }
  }
  }
}
@media screen and (max-width: 770px) {
  .container_body {
    margin: 2.5rem 1rem 1rem 1rem;
    .titulo {
      font-size: 2rem;
    }
    .texto_corrido_inicial {
    margin-top: 2rem;
    width: 30rem;
    margin-bottom: 2rem;
    .subtitle{
      margin-top: -2rem;
        font-size: 1.2rem;
        font-weight: bold;
    }
  }
    .img_revista{

    margin-left: -6rem;
    grid-column-start: 1;
    grid-column-end: 3;
      width: 54rem;
      img{
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: center;
      }
  }
  }
}
@media screen and (max-width: 600px) {
  .container_body {
    margin: 2.5rem 1rem 1rem 1rem;
    .titulo {
      font-size: 2rem;
    }
    .texto_corrido_inicial {
    margin-top: 2rem;
    width: 30rem;
    margin-bottom: 2rem;
    .subtitle{
      margin-top: -2rem;
        font-size: 1.2rem;
        font-weight: bold;
    }
  }
    .img_revista{

    margin-left: -6rem;
    grid-column-start: 1;
    grid-column-end: 3;
      width: 45rem;
      img{
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: center;
      }
  }
  }
}
@media screen and (max-width: 530px) {
  .container_body {
    margin: 2.5rem 1rem 1rem 1rem;
    .titulo {
      font-size: 2rem;
    }
    .texto_corrido_inicial {
    margin-top: 2rem;
    width: 20rem;
    margin-bottom: 2rem;
    .subtitle{
      margin-top: -2rem;
        font-size: 1.2rem;
        font-weight: bold;
    }
  }
    .img_revista{

    margin-left: -6rem;
    grid-column-start: 1;
    grid-column-end: 3;
      width: 39rem;
      img{
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: center;
      }
  }
  }
}
@media screen and (max-width: 430px) {
  .container_body {
    margin: 2.5rem 1rem 1rem 1rem;
    .titulo {
      font-size: 2rem;
    }
    .texto_corrido_inicial {
    margin-top: 2rem;
    width: 20rem;
    margin-bottom: 2rem;
    .subtitle{
      margin-top: -2rem;
        font-size: 1.2rem;
        font-weight: bold;
    }
  }
    .img_revista{

    margin-left: -6rem;
    grid-column-start: 1;
    grid-column-end: 3;
      width: 32rem;
      img{
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: center;
      }
  }
  }
}
@media screen and (max-width: 375px) {
  .container_body {
    margin: 2.5rem 1rem 1rem 1rem;
    .titulo {
      font-size: 2rem;
    }
    .texto_corrido_inicial {
    margin-top: 2rem;
    width: 20rem;
    margin-bottom: 2rem;
    .subtitle{
      margin-top: -2rem;
        font-size: 1.2rem;
        font-weight: bold;
    }
  }
    .img_revista{

    margin-left: -6rem;
    grid-column-start: 1;
    grid-column-end: 3;
      width: 29rem;
      img{
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: center;
      }
  }
  }
}


</style>