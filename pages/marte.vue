<template>
  <div class="container_body">
    <Title class="titulo" :titleprop="title"> </Title>
    <div class="texto_corrido_inicial">
      Prototipo pensado como una App para poder ver el tiempo en marte sacado de
      datos a tiempo real de los robots que están explorándolo.
      <br /><br />

      El potencial de esta App reside en que también la he programado con HTML ,
      CSS y JS. Los datos se sacan a partir de una API proporcionada por la
      propia NASA que hacen que los datos sean verídicos.
    </div>
    <div class="img_marte_1" data-aos="fade-up" data-aos-duration="2000">
      <img src="/img/marte/MARTE_1.png" alt="" />
    </div>
    <div class="texto_corrido_inicial text_2_marte">
      <h3 class="subtitle">ACCIONES.</h3>
      Esta App tiene un apartado de información que nos explica la nomenclatura
      utilizada para este planeta, así como otros datos.
      <br /><br />
      También poder guardar temperaturas de algunos días, así como revisar sus
      datos o borrarlas.
      <div class="img_marte_2">
        <img data-aos="fade-up" data-aos-duration="2000" src="/img/marte/MARTE_2.png" alt="" />
        <img data-aos="fade-up" data-aos-duration="2000" src="/img/marte/MARTE_3.png" alt="" />
      </div>
    </div>
    <div class="buttons_link">
      <a href=" https://christianvalenciag.github.io/marte/" class="button_link_a button_blue">VER EN GITHUB</a>
      <a href=" https://www.figma.com/file/P5lxYBpVYIngRnAIV1azVQ/MARTE?node-id=0%3A1" class="button_link_a button_pink">VER PROTOTIPO</a>
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
        '<span class="pink">Diseño y programación</span><br /> APP tiempo en Marte.',
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
    position: relative;
    margin-top: 2rem;
    width: 30rem;
    .texto_into {
      margin-left: 7rem;
      position: absolute;
      top: 8rem;
      right: -14rem;
      .iconify_1 {
        color: #066772;
        margin: 0 0 0 19rem;
      }
    }
    .subtitle {
      font-size: 1.25rem;
      margin: 0 0 0.5rem 0;
    }
    .img_marte_2{
      display: flex;
      width: 35rem;
      margin-top: 2rem;
      margin-left: -6rem;
        img {
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: center;
        }
    }
    &.text_2_marte{
      margin-top: -30rem;
      margin-left: 10rem;
    }
  }
  .img_marte_1 {
    margin-left: 4rem;
    margin-top: -6rem;
    width: 25rem;
    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: center;
    }
  }
  .buttons_link{
    margin-left: 3.5rem;
    margin-top: 11.5rem;
    width: 70%;
    display: flex;
    flex-direction: column;
    .button_link_a{
      display: flex;
      justify-content: center;
      align-items: center;

      color: white;
      padding: .75rem 5rem;
      border-radius: 1rem;
      &.button_blue{
        background-color: #066772;
        opacity: 80%;
        margin-bottom: 1rem;
        &:hover{
          opacity: 100%;
        }
      }
      &.button_pink{
        opacity: 85%;
        background-color: #EC695E;
        &:hover{
          opacity: 100%;
        }
      }
    }
  }
}

@media screen and (max-width: 1360px) {
      .container_body {
      .titulo {
      }
      .texto_corrido_inicial {
        
        .img_marte_2{
          display: flex;
          width: 35rem;
          margin-top: 2rem;
          margin-left: -6rem;
            img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: center;
            }
        }
        &.text_2_marte{
          margin-top: -30rem;
          margin-left: 10rem;
        }
      }
      .img_marte_1 {
        margin-left: 9rem;
        margin-top: -6rem;
        width: 25rem;
        img {
          width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;
        }
      }
      
    }
}
@media screen and (max-width: 1160px) {
      .container_body {
      .titulo {
      }
      .texto_corrido_inicial {
        
        .img_marte_2{
          display: flex;
          width: 35rem;
          margin-top: 2rem;
          margin-left: -3rem;
            img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: center;
            }
        }
        &.text_2_marte{
          margin-top: -30rem;
          margin-left: 0rem;
        }
      }
      .img_marte_1 {
        margin-left: 9rem;
        margin-top: -6rem;
        width: 25rem;
        img {
          width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;
        }
      }
          .buttons_link{
        margin-left: 8rem;
        margin-top: 22rem;
        width: 70%;
        display: flex;
        flex-direction: column;
        .button_link_a{
          display: flex;
          justify-content: center;
          align-items: center;

          color: white;
          padding: .75rem 5rem;
          border-radius: 1rem;
          &.button_blue{
            background-color: #066772;
            opacity: 80%;
            margin-bottom: 1rem;
            &:hover{
              opacity: 100%;
            }
          }
          &.button_pink{
            opacity: 85%;
            background-color: #EC695E;
            &:hover{
              opacity: 100%;
            }
          }
        }
      }
      
    }
}
@media screen and (max-width: 1060px) {
      .container_body {
      .titulo {
        
      }
      .texto_corrido_inicial {
        
        .img_marte_2{
          display: flex;
          width: 35rem;
          margin-top: 2rem;
          margin-left: -3rem;
            img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: center;
            }
        }
        &.text_2_marte{
          margin-top: -20rem;
          margin-left: 0rem;
        }
      }
      .img_marte_1 {
        margin-left: 8rem;
        margin-top: -6rem;
        width: 20rem;
        img {
          width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;
        }
      }
          .buttons_link{
            grid-column-start: 1;
    grid-column-end: 3;
        margin-left: 0rem;
        margin-top: 2rem;
        width: 70%;
        display: flex;
        flex-direction: column;
        .button_link_a{
          display: flex;
          justify-content: center;
          align-items: center;

          color: white;
          padding: .75rem 5rem;
          border-radius: 1rem;
          &.button_blue{
            background-color: #066772;
            opacity: 80%;
            margin-bottom: 1rem;
            &:hover{
              opacity: 100%;
            }
          }
          &.button_pink{
            opacity: 85%;
            background-color: #EC695E;
            &:hover{
              opacity: 100%;
            }
          }
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
        font-size: 2rem;
      }
      .texto_corrido_inicial {
        width: 30rem;
        .img_marte_2{
          display: flex;
          width: 35rem;
          margin-top: 2rem;
          margin-left: -1rem;
            img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: center;
            }
        }
        &.text_2_marte{
          margin-top: -20rem;
          margin-left: 0rem;
        }
      }
      .img_marte_1 {
        margin-left: 8rem;
        margin-top: -6rem;
        width: 17rem;
        img {
          width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;
        }
      }
          .buttons_link{
            grid-column-start: 1;
    grid-column-end: 3;
        margin-left: 0rem;
        margin-top: 2rem;
        width: 70%;
        display: flex;
        flex-direction: column;
        .button_link_a{
          display: flex;
          justify-content: center;
          align-items: center;

          color: white;
          padding: .75rem 5rem;
          border-radius: 1rem;
          &.button_blue{
            background-color: #066772;
            opacity: 80%;
            margin-bottom: 1rem;
            &:hover{
              opacity: 100%;
            }
          }
          &.button_pink{
            opacity: 85%;
            background-color: #EC695E;
            &:hover{
              opacity: 100%;
            }
          }
        }
      }
      
    }
}
@media screen and (max-width: 847px) {
      .container_body {
      margin: 2.5rem 1rem 1rem 1rem;
      display: grid;
      grid-template-columns: 50% 50%;
      .titulo {
        font-size: 2rem;
      }
      .texto_corrido_inicial {
        width: 30rem;
        .img_marte_2{
          display: flex;
          width: 23rem;
          margin-top: 2rem;
          margin-left: -1rem;
            img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: center;
            }
        }
        &.text_2_marte{
          margin-top: -10rem;
          margin-left: 2rem;
        }
      }
      .img_marte_1 {
        margin-left: 9rem;
        margin-top: -6rem;
        width: 13rem;
        img {
          width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;
        }
      }
          .buttons_link{
            grid-column-start: 1;
    grid-column-end: 3;
        margin-left: 0rem;
        margin-top: 2rem;
        width: 70%;
        display: flex;
        flex-direction: column;
        .button_link_a{
          display: flex;
          justify-content: center;
          align-items: center;

          color: white;
          padding: .75rem 5rem;
          border-radius: 1rem;
          &.button_blue{
            background-color: #066772;
            opacity: 80%;
            margin-bottom: 1rem;
            &:hover{
              opacity: 100%;
            }
          }
          &.button_pink{
            opacity: 85%;
            background-color: #EC695E;
            &:hover{
              opacity: 100%;
            }
          }
        }
      }
      
    }
}
@media screen and (max-width: 747px) {
      .container_body {
      margin: 2.5rem 1rem 1rem 1rem;
      display: grid;
      grid-template-columns: 50% 50%;
      .titulo {
        font-size: 2rem;
      }
      .texto_corrido_inicial {
        width: 30rem;
        .img_marte_2{
          display: flex;
          width: 23rem;
          margin-top: 2rem;
          margin-left: -1rem;
            img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: center;
            }
        }
        &.text_2_marte{
          margin-top: 1rem;
          margin-left: 2rem;
        }
      }
      .img_marte_1 {
        grid-column-start: 1;
        grid-column-end: 3;
        margin-left: 20rem;
        margin-top: 2rem;
        width: 16rem;
        img {
          width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;
        }
      }
      
    }
}
@media screen and (max-width: 647px) {
      .container_body {
      margin: 2.5rem 1rem 1rem 1rem;
      display: grid;
      grid-template-columns: 50% 50%;
      .titulo {
        font-size: 2rem;
      }
      .texto_corrido_inicial {
        width: 30rem;
        .img_marte_2{
          display: flex;
          width: 23rem;
          margin-top: 2rem;
          margin-left: -1rem;
            img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: center;
            }
        }
        &.text_2_marte{
          margin-top: 1rem;
          margin-left: 2rem;
        }
      }
      .img_marte_1 {
        grid-column-start: 1;
        grid-column-end: 3;
        margin-left: 13rem;
        margin-top: 2rem;
        width: 16rem;
        img {
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
      display: grid;
      grid-template-columns: 50% 50%;
      .titulo {
        font-size: 2rem;
      }
      .texto_corrido_inicial {
        width: 20rem;
        .img_marte_2{
          display: flex;
          width: 20rem;
          margin-top: 2rem;
          margin-left: .5rem;
            img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: center;
            }
        }
        &.text_2_marte{
          margin-top: 1rem;
          margin-left: 0rem;
        }
      }
      .img_marte_1 {
        grid-column-start: 1;
        grid-column-end: 3;
        margin-left: 1.5rem;
        margin-top: 2rem;
        width: 16rem;
        img {
          width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;
        }
      }
      .buttons_link{
            grid-column-start: 1;
        grid-column-end: 3;
        margin-left: 0rem;
        margin-top: 2rem;
        width: 100%;
        display: flex;
        flex-direction: column;
        .button_link_a{
          display: flex;
          justify-content: center;
          align-items: center;

          color: white;
          padding: .75rem 5rem;
          border-radius: 1rem;
          &.button_blue{
            background-color: #066772;
            opacity: 80%;
            margin-bottom: 1rem;
            &:hover{
              opacity: 100%;
            }
          }
          &.button_pink{
            opacity: 85%;
            background-color: #EC695E;
            &:hover{
              opacity: 100%;
            }
          }
        }
      }
    }
}

// 530
</style>