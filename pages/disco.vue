<template>
  <div class="container_body">
    <Title class="titulo" :titleprop="title"> </Title>
    <div class="texto_corrido_inicial">
      Esta es el diseño de una portada de disco para el sencillo "Sun Goes Down" del
      artista y cantante `Lil Nas X`. Esta canción habla de sus miedos cuando era
      pequeño, entre ellos el racismo interiorizado el cual le hacía cuestionar
      y odiar sus labios. El disco pretende remarcar eses labios, fuera
      ocultados con unas letras opacas y negras y en el interior resaltado con
      un rojo, a modo de pintalabios
      <br /><br />
      <div class="subtitle blue">¿Por qué?</div>
      <br />
      Pretendo mostrar como muchas
      veces lo que primero se ve y lo que realmente es, tiene pequeños matices.
      Hace referencia a como a lo largo de la canción se va queriendo más y
      tambien al conjunto de la era (disco) en el que tambien habla de su
      reciente salida del armario.
    </div>
    
    <div class="img_disco">
      <img src="/img/disco/DISCO_2.png" alt="" />
    </div>
    <div class="img_disco">
      <img src="/img/disco/DISCO_3.png" alt="" />
    </div>
    <div class="img_disco_2">
      <img src="/img/disco/DISCO.png" alt="" />
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
        '<span class="pink">Diseño ilustrativo</span><br /> portada vinilo.',
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
  .img_disco{
      margin-top: -3rem;
    width: 40rem;
    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: center;
    }
  }
  .img_disco_2{
    margin-top: -8rem;
    grid-column-start: 1;
    grid-column-end: 3;
    width: 75rem;
    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: center;
    }
  }
}
@media screen and (max-width: 1410px) {
  .container_body {
  
      .titulo {
      }
    .img_disco {
      margin-top: 2rem;
      width: 33rem;
    }
    .img_disco_2 {
        margin-top: 2rem;
      grid-column-start: 1;
      grid-column-end: 3;
      width: 71rem;
    }
  }
}
@media screen and (max-width: 1280px) {
  .container_body {
  
      .titulo {
      }
    .img_disco {
      margin-top: 2rem;
      width: 29rem;
    }
    .img_disco_2 {
        margin-top: 2rem;
      grid-column-start: 1;
      grid-column-end: 3;
      width: 63rem;
    }
  }
}
@media screen and (max-width: 1180px) {
  .container_body {
  
      .titulo {
      }
    .img_disco {
      margin-top: -5rem;
      grid-column-start: 1;
      grid-column-end: 3;
      width: 60rem;
    }
    .img_disco_2 {
        margin-top: -5rem;
      grid-column-start: 1;
      grid-column-end: 3;
      width: 60rem;
    }
  }
}
@media screen and (max-width: 1100px) {
  .container_body {
  
      .titulo {
      }
    .img_disco {
      margin-top: -5rem;
      grid-column-start: 1;
      grid-column-end: 3;
      width: 51rem;
    }
    .img_disco_2 {
       margin-top: -5rem;
      grid-column-start: 1;
      grid-column-end: 3;
      width: 51rem;
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
      }
    .img_disco {
      margin-top: -5rem;
      grid-column-start: 1;
      grid-column-end: 3;
      width: 51rem;
    }
    .img_disco_2 {
      margin-top: -5rem;
      grid-column-start: 1;
      grid-column-end: 3;
      width: 51rem;
    }
  }
}
@media screen and (max-width: 847px) {
  .container_body {
      .titulo {
      }
      .texto_corrido_inicial {
        width: 30rem;
      }
    .img_disco {
      grid-column-start: 1;
      grid-column-end: 3;
      width: 45rem;
    }
    .img_disco_2 {
      grid-column-start: 1;
      grid-column-end: 3;
      width: 45rem;
    }
  }
}
@media screen and (max-width: 752px) {
  .container_body {
      .titulo {
      }
      .texto_corrido_inicial {
        width: 30rem;
      }
    .img_disco {
      grid-column-start: 1;
      grid-column-end: 3;
      width: 39rem;
    }
    .img_disco_2 {
      grid-column-start: 1;
      grid-column-end: 3;
      width: 39rem;
    }
  }
}
@media screen and (max-width: 652px) {
  .container_body {
      .titulo {
      }
      .texto_corrido_inicial {
        width: 30rem;
      }
    .img_disco {
      margin: -2rem;
      grid-column-start: 1;
      grid-column-end: 3;
      width: 30rem;
    }
    .img_disco_2 {
      margin: -2rem;
      grid-column-start: 1;
      grid-column-end: 3;
      width: 30rem;
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
    .img_disco {
      grid-column-start: 1;
      grid-column-end: 3;
      width: 25rem;
    }
    .img_disco_2 {
      grid-column-start: 1;
      grid-column-end: 3;
      width: 25rem;
    }
  }
}
@media screen and (max-width: 420px) {
  .container_body {
      .titulo {
      }
      .texto_corrido_inicial {
        width: 20rem;
      }
    .img_disco {
      grid-column-start: 1;
      grid-column-end: 3;
      width: 23rem;
    }
    .img_disco_2 {
      grid-column-start: 1;
      grid-column-end: 3;
      width: 23rem;
    }
  }
}
@media screen and (max-width: 380px) {
  .container_body {
      .titulo {
      }
      .texto_corrido_inicial {
        width: 20rem;
      }
    .img_disco {
      grid-column-start: 1;
      grid-column-end: 3;
      width: 20rem;
    }
    .img_disco_2 {
      grid-column-start: 1;
      grid-column-end: 3;
      width: 20rem;
    }
  }
}

</style>