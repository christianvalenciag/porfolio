<template>
  <div class="container_body">
    <div class="flecha_invisible">

    </div>
    <Title class="titulo" :titleprop="title"> </Title>
    <div class="texto_corrido_inicial">
      La idea visual nada de la revista impresa, donde las portadas están
      enmarcadas por un amplio recuadro amarillo, la marca. Remarcan la idea de
      que el contenido es parte de la marca.
      <br /><br />
      Así bien, quise trasladar ese
      concepto de captura dentro de la marca a la parte audiovisual. En los
      programas de este canal hay tres cosas fundamentales: la fotografía, el
      video y el sónido. De forma simplificada y a través del juego de la marca
      y la captura dentro de ello, se han creado los siguientes idents.
    </div>

    <div class="img_disco">
        <video src="/img/idents/ident_fotografia.mp4" controls loop></video>
    </div>
    <div class="img_disco">
      <video src="/img/idents/ident_video.mp4" controls loop></video>
    </div>
    <div class="img_disco_2">
      <video src="/img/idents/ident_audio.mp4" controls loop></video>
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
      title: '<span class="pink">IDENTS</span><br />National Geographic.',
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
  .img_disco {
    margin-top: 2rem;
    width: 38rem;
    video {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: center;
    }
  }
  .img_disco_2 {
      margin-top: 2rem;
    grid-column-start: 1;
    grid-column-end: 3;
    width: 77rem;
    video {
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
      margin-top: 2rem;
      grid-column-start: 1;
      grid-column-end: 3;
      width: 60rem;
    }
    .img_disco_2 {
        margin-top: 2rem;
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
      margin-top: 2rem;
      grid-column-start: 1;
      grid-column-end: 3;
      width: 51rem;
    }
    .img_disco_2 {
        margin-top: 2rem;
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
      margin-top: 2rem;
      grid-column-start: 1;
      grid-column-end: 3;
      width: 51rem;
    }
    .img_disco_2 {
        margin-top: 2rem;
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
      margin-top: 2rem;
      grid-column-start: 1;
      grid-column-end: 3;
      width: 45rem;
    }
    .img_disco_2 {
        margin-top: 2rem;
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
      margin-top: 2rem;
      grid-column-start: 1;
      grid-column-end: 3;
      width: 39rem;
    }
    .img_disco_2 {
        margin-top: 2rem;
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
      margin-top: 2rem;
      grid-column-start: 1;
      grid-column-end: 3;
      width: 30rem;
    }
    .img_disco_2 {
        margin-top: 2rem;
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
      margin-top: 2rem;
      grid-column-start: 1;
      grid-column-end: 3;
      width: 25rem;
    }
    .img_disco_2 {
        margin-top: 2rem;
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
      margin-top: 2rem;
      grid-column-start: 1;
      grid-column-end: 3;
      width: 23rem;
    }
    .img_disco_2 {
        margin-top: 2rem;
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
      margin-top: 2rem;
      grid-column-start: 1;
      grid-column-end: 3;
      width: 20rem;
    }
    .img_disco_2 {
        margin-top: 2rem;
      grid-column-start: 1;
      grid-column-end: 3;
      width: 20rem;
    }
  }
}

</style>