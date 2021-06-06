<template>
  <div class="container_body">
    <Title class="titulo" :titleprop="title"></Title>
    <div class="texto_corrido_inicial">
      Dentro del diseño gráfico tengo amplio conocimientos de muchos sectores
      pero en los que más cómodo me encuentro sería los ya mencionados. Destaco
      tambien la capacidad para génerar ideas y me encuentro comodo trabajando
      en equipo, pudiendo llegar a mejores resultados.
    </div>
    <div class="text_relative">
      <div class="texto_lateral_index">
        <div class="titulo_text_l">ALGUNOS TRABAJOS</div>
        <div class="text_l">
          Estes son tres de los proyectos que más destacos ahora mismo.
        </div>
        <div class="arrow" data-aos="fade-down-left" data-aos-duration="2000">
          <span
            class="iconify"
            data-icon="carbon:arrow-down-left"
            data-inline="false"
          ></span>
        </div>
      </div>
    </div>
    <div class="img">
      <div class="img_revista" data-aos="fade-up" data-aos-duration="2000">
        <img src="/img/revista.png" alt="">
      </div>
      <div class="text_revista">
        <div class="title_revista">
          Creación y diseño
        </div>
        <div class="texto">
          de una revista de reivindicación social, “FAKDEM”.
        </div>
        <div class="leer_mas">
          <NuxtLink class="leer_mas_nuxt" to="revista">Leer más <span class="iconify" data-icon="akar-icons:circle-plus" data-inline="false"></span> </NuxtLink>
        </div>
      </div>
    </div>
    <div class="img img_derecha">
      <div class="text_revista text_ident">
        <div class="title_revista">
          Idents
        </div>
        <div class="texto">
          para la canal televisivon <br /> de National Geographic Channel.
        </div>
        <div class="leer_mas">
          <NuxtLink class="leer_mas_nuxt" to="idents">Leer más <span class="iconify" data-icon="akar-icons:circle-plus" data-inline="false"></span> </NuxtLink>
        </div>
      </div>
      <div class="img_ident" data-aos="fade-down-left" data-aos-duration="2000">
        <img src="/img/tv.png" alt="">
      </div>
    </div>
    <div class="img img_disco_x">
      <div class="img_disco" data-aos="fade-right" data-aos-duration="2000">
        <img src="/img/DISCO.png" alt="">
      </div>
      <div class="text_revista text_disco">
        <div class="title_revista">
          Diseño
        </div>
        <div class="texto">
          de una portada de disco para "SUN GOES DOWN".
        </div>
        <div class="leer_mas">
          <NuxtLink class="leer_mas_nuxt" to="disco">Leer más <span class="iconify" data-icon="akar-icons:circle-plus" data-inline="false"></span> </NuxtLink>
        </div>
      </div>
    </div>
    <div class="img img_derecha">
      <div class="text_revista text_mermelada">
        <div class="title_revista">
          Rediseño
        </div>
        <div class="texto">
          de la marca HACENDADO y linea de mermeladas.
        </div>
        <div class="leer_mas">
          <NuxtLink class="leer_mas_nuxt" to="mermeladas">Leer más <span class="iconify" data-icon="akar-icons:circle-plus" data-inline="false"></span> </NuxtLink>
        </div>
      </div>
      <div class="img_mermelada" data-aos="fade-left" data-aos-duration="2000">
        <img src="/img/3_mermeladas.png" alt="">
      </div>
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
        'Como diseñador <span class="blue">gráfico</span>: <span class="pink">Branding</span>, Carteleria y Maquetación.',
    };
  },
};
</script>

<style lang="scss" scoped>
.container_body {
  
  margin: 2.5rem 6rem 1rem 6rem;
  display: grid;
  grid-template-columns: 50% 50%;
  .titulo {
    grid-column-start: 1;
    grid-column-end: 3;
  }
  .texto_corrido_inicial {
    margin-top: 2rem;
    width: 30rem;
  }
  .text_relative {
    position: relative;
    .texto_lateral_index {
      position: absolute;
      display: flex;
      flex-direction: column;
      align-items: flex-end;
      bottom: -6rem;
      right: 0.001rem;
      .titulo_text_l {
        margin: 0;
        padding: 0;
        font-size: 1.5rem;
        font-weight: bold;
      }
      .text_l {
        text-align: right;
        width: 20rem;
      }
      .arrow {
        color: #ec695e;
        width: 2rem;
        .iconify {
          width: 100%;
          height: 100%;
        }
      }
    }
  }
  .img{
    position: relative;
    grid-column-start: 1;
    grid-column-end: 3;
    &.img_derecha{
      display: flex;
      justify-content: flex-end;
    }
    &.img_disco_x{
      padding-top: 1rem ;
    }
    .img_revista{
      margin-top: 2rem;
      margin-left: -15rem;
      width: 53rem;
      img{
        width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
    .text_revista{
      position: absolute;
      top: 10rem;
        left: 35rem;
        &.text_ident{
          top: 7rem;
          left: 32rem;
        }
        &.text_disco{
        top: 9rem;
        left: 37rem;
        }
        &.text_mermelada{
          top: 10rem;
          left: 28rem;
        }
      .title_revista{
        color: #066772;
          font-size: 1.2rem;
      }
      .texto{
          width: 12rem;
        }
        .leer_mas{
          margin-top: 1rem;
          .leer_mas_nuxt{
            position: relative;
            color: black;
          .iconify{
            position: absolute;
            top: .2rem;
            left: 4rem;
          }
          &:hover{
            color: #EC695E;
          }
          }
        }
    }
    .img_ident{
      margin-top: -13rem;
      width: 33rem;
      img{
        width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
    .img_disco{
      margin-top: -10rem;
      margin-left: -5rem;
      width: 45rem;
      img{
        width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
    .img_mermelada{
      margin-top: 0rem;
      margin-right: -6rem;
      width: 43rem;
      img{
        width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
  }
  
}
@media screen and (max-width: 1384px) {
    .container_body {
      margin: 2.5rem 6rem 1rem 6rem;
      display: grid;
      grid-template-columns: 50% 50%;
      .titulo {
        grid-column-start: 1;
        grid-column-end: 3;
      }
      .img{
        .text_revista{
        position: absolute;
        top: 10rem;
        left: 35rem;
        &.text_ident{
          top: 7rem;
          left: 29rem;
        }
        &.text_disco{
        top: 9rem;
        left: 37rem;
        }
        &.text_mermelada{
          top: 10rem;
          left: 24rem;
        }
        .title_revista{
         color: #066772;
          font-size: 1.2rem;
      }
      .texto{
          width: 12rem;
        }
        .leer_mas{
          margin-top: 1rem;
          .leer_mas_nuxt{
            position: relative;
            color: black;
          .iconify{
            position: absolute;
            top: .2rem;
            left: 4rem;
          }
          &:hover{
            color: #EC695E;
          }
          }
        }
    }
      }
    }
}
@media screen and (max-width: 1344px) {
    .container_body {
      margin: 2.5rem 6rem 1rem 6rem;
      display: grid;
      grid-template-columns: 50% 50%;
      .titulo {
        grid-column-start: 1;
        grid-column-end: 3;
      }
      .img{
        .text_revista{
        &.text_ident{
          top: 7rem;
          left: 23rem;
        }
        &.text_mermelada{
          top: 10rem;
          left: 19rem;
        }
        .title_revista{
         color: #066772;
          font-size: 1.2rem;
      }
    }
      }
    }
}
@media screen and (max-width: 1264px) {
    .container_body {
      margin: 2.5rem 6rem 1rem 6rem;
      display: grid;
      grid-template-columns: 50% 50%;
      .titulo {
        grid-column-start: 1;
        grid-column-end: 3;
      }
      .img{
        .text_revista{
        &.text_ident{
          top: 7rem;
          left: 18rem;
        }
        &.text_mermelada{
          top: 10rem;
          left: 14rem;
        }
        .title_revista{
         color: #066772;
          font-size: 1.2rem;
      }
    }
      }
    }
}
@media screen and (max-width: 1184px) {
    .container_body {
      margin: 2.5rem 6rem 1rem 6rem;
      display: grid;
      grid-template-columns: 50% 50%;
      .titulo {
        grid-column-start: 1;
        grid-column-end: 3;
      }
      .img{
        &.img_derecha{
        display: flex;
        justify-content: flex-end;
        }
      .img_revista{
        margin-top: 2rem;
        margin-left: -25rem;
        width: 53rem;
          img{
            width: 100%;
              height: 100%;
              object-fit: cover;
              object-position: center;

          }
       }
        .text_revista{
          position: absolute;
        top: 8rem;
        left: 22rem;
        &.text_ident{
          top: 7rem;
          left: 11rem;
        }
        &.text_disco{
        top: 9rem;
        left: 31rem;
        }
        &.text_mermelada{
          top: 10rem;
          left: 8rem;
        }
        .title_revista{
         color: #066772;
          font-size: 1.2rem;
      }
    }
    .img_ident{
      margin-top: -13rem;
      width: 33rem;
      img{
        width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
    .img_disco{
      margin-top: -10rem;
      margin-left: -10rem;
      width: 45rem;
      img{
        width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
    .img_mermelada{
      margin-top: 0rem;
      margin-right: -6rem;
      width: 43rem;
      img{
        width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
      }
    }
}
@media screen and (max-width: 1084px) {
    .container_body {
      margin: 2.5rem 6rem 1rem 6rem;
      display: grid;
      grid-template-columns: 50% 50%;
      .titulo {
        grid-column-start: 1;
        grid-column-end: 3;
      }
      .img{
        &.img_derecha{
        display: flex;
        justify-content: flex-end;
        }
        &.img_disco_x{
          margin-top: 2rem ;
        }
      .img_revista{
        margin-top: 2rem;
        margin-left: -17rem;
        width: 43rem;
          img{
            width: 100%;
              height: 100%;
              object-fit: cover;
              object-position: center;

          }
       }
        .text_revista{
          position: absolute;
        top: 8rem;
        left: 22rem;
        &.text_ident{
          top: -1.5rem;
          left: 18rem;
        }
        &.text_disco{
        top: 6rem;
        left: 25rem;
        }
        &.text_mermelada{
          top: 7rem;
          left: 13rem;
        }
        .title_revista{
         color: #066772;
          font-size: 1.2rem;
      }
    }
    .img_ident{
      margin-top: -13rem;
      width: 23rem;
      img{
        width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
    .img_disco{
      margin-top: -10rem;
      margin-left: -10rem;
      width: 38rem;
      img{
        width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
    .img_mermelada{
      margin-top: 0rem;
      margin-right: -6rem;
      width: 33rem;
      img{
        width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
      }
    }
}
@media screen and (max-width: 1017px) {
    .container_body {
      margin: 2.5rem 6rem 1rem 6rem;
      display: grid;
      grid-template-columns: 50% 50%;
      .titulo {
        grid-column-start: 1;
        grid-column-end: 3;
      }
      .texto_corrido_inicial {
    margin-top: 2rem;
    width: 30rem;
      }
        .text_relative {
          position: relative;
          .texto_lateral_index {
            position: absolute;
            display: flex;
            flex-direction: column;
            align-items: flex-end;
            bottom: -10rem;
            right: 0.001rem;
            .titulo_text_l {
              margin: 0;
              padding: 0;
              font-size: 1.5rem;
              font-weight: bold;
            }
            .text_l {
              text-align: right;
              width: 20rem;
            }
            .arrow {
              color: #ec695e;
              width: 2rem;
              .iconify {
                width: 100%;
                height: 100%;
              }
            }
          }
        }
      .img{
        &.img_derecha{
        display: flex;
        justify-content: flex-end;
        }
      .img_revista{
        margin-top: 2rem;
        margin-left: -20rem;
        width: 43rem;
          img{
            width: 100%;
              height: 100%;
              object-fit: cover;
              object-position: center;

          }
       }
        .text_revista{
          position: absolute;
        top: 8rem;
        left: 20rem;
        &.text_ident{
          top: 1rem;
          left: 12rem;
        }
        &.text_disco{
        top: 10.5rem;
        left: 25rem;
        }
        &.text_mermelada{
          top: 7rem;
          left: 9rem;
        }
        .title_revista{
         color: #066772;
          font-size: 1.2rem;
      }
    }
    .img_ident{
      margin-top: -10rem;
      width: 23rem;
      img{
        width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
    .img_disco{
      margin-top: -6rem;
      margin-left: -10rem;
      width: 38rem;
      img{
        width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
    .img_mermelada{
      margin-top: 0rem;
      margin-right: -6rem;
      width: 33rem;
      img{
        width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
      }
    }
}

////////// cambio de tamaños texto y margenes //////////

@media screen and (max-width: 947px) {
    .container_body {
      margin: 2.5rem 1rem 1rem 1rem;
      display: grid;
      grid-template-columns: 50% 50%;
      .titulo {
        grid-column-start: 1;
        grid-column-end: 3;
        font-size: 2rem;
        width: 30rem;
      }
      .texto_corrido_inicial {
    margin-top: 2rem;
    width: 30rem;
      }
        .text_relative {
          position: relative;
          .texto_lateral_index {
            position: absolute;
            display: flex;
            flex-direction: column;
            align-items: flex-end;
            bottom: -10rem;
            right: 0.001rem;
            .titulo_text_l {
              margin: 0;
              padding: 0;
              font-size: 1.2rem;
              font-weight: bold;
            }
            .text_l {
              text-align: right;
              width: 20rem;
            }
            .arrow {
              color: #ec695e;
              width: 1.5rem;
              .iconify {
                width: 100%;
                height: 100%;
              }
            }
          }
        }
      .img{
        &.img_derecha{
        display: flex;
        justify-content: flex-end;
        }
        &.img_disco_x{
          margin-top: 1rem ;
        }
      .img_revista{
        margin-top: 2rem;
        margin-left: -13rem;
        width: 33rem;
          img{
            width: 100%;
              height: 100%;
              object-fit: cover;
              object-position: center;

          }
       }
        .text_revista{
          position: absolute;
        top: 16rem;
        left: 20rem;
        &.text_ident{
          top: 4rem;
          left: 28rem;
        }
        &.text_disco{
        top: 4.5rem;
        left: 23rem;
        }
        &.text_mermelada{
          top: 4rem;
          left: 17rem;
        }
        .title_revista{
         color: #066772;
          font-size: 1.1rem;
      }
    }
    .img_ident{
      margin-top: -2rem;
      width: 15rem;
      img{
        width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
    .img_disco{
      margin-top: -6rem;
      margin-left: -3rem;
      width: 28rem;
      img{
        width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
    .img_mermelada{
      margin-top: -2rem;
      margin-right: -1rem;
      width: 26rem;
      img{
        width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
      }
    }
}
@media screen and (max-width: 907px) {
    .container_body {
      margin: 2.5rem 1rem 1rem 1rem;
      display: grid;
      grid-template-columns: 50% 50%;
      .titulo {
        grid-column-start: 1;
        grid-column-end: 3;
        font-size: 2rem;
        width: 30rem;
      }
      .texto_corrido_inicial {
    margin-top: 2rem;
    width: 30rem;
      }
        .text_relative {
          position: relative;
          .texto_lateral_index {
            position: absolute;
            display: flex;
            flex-direction: column;
            align-items: flex-end;
            bottom: -10rem;
            right: 0.001rem;
            .titulo_text_l {
              margin: 0;
              padding: 0;
              font-size: 1.2rem;
              font-weight: bold;
            }
            .text_l {
              text-align: right;
              width: 20rem;
            }
            .arrow {
              color: #ec695e;
              width: 1.5rem;
              .iconify {
                width: 100%;
                height: 100%;
              }
            }
          }
        }
      .img{
        &.img_derecha{
        display: flex;
        justify-content: flex-end;
        }
      .img_revista{
        margin-top: 9rem;
        margin-left: 15rem;
        width: 33rem;
          img{
            width: 100%;
              height: 100%;
              object-fit: cover;
              object-position: center;

          }
       }
        .text_revista{
          position: absolute;
        top: 10.5rem;
        left: 19rem;
        &.text_ident{
          top: 0rem;
          left: 20rem;
        }
        &.text_disco{
        top: 11rem;
        left: 15rem;
        }
        &.text_mermelada{
          top: 3rem;
          left: 27rem;
        }
        .title_revista{
         color: #066772;
          font-size: 1.1rem;
      }
    }
    .img_ident{
      margin-top: -9rem;
      margin-right: 37rem;
      width: 15rem;
      img{
          width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
    .img_disco{
      margin-top: 0rem;
      margin-left: 24rem;
      width: 28rem;
      img{
        width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
    .img_mermelada{
      margin-top: -2rem;
      margin-right: 30rem;
      width: 26rem;
      img{
        width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
      }
    }
}
@media screen and (max-width: 880px) {
    .container_body {
      margin: 2.5rem 1rem 1rem 1rem;
      display: grid;
      grid-template-columns: 50% 50%;
      .titulo {
        grid-column-start: 1;
        grid-column-end: 3;
        font-size: 2rem;
        width: 30rem;
      }
      .texto_corrido_inicial {
    margin-top: 2rem;
    width: 30rem;
      }
        .text_relative {
          position: relative;
          .texto_lateral_index {
            position: absolute;
            display: flex;
            flex-direction: column;
            align-items: flex-end;
            bottom: -10rem;
            right: 0.001rem;
            .titulo_text_l {
              margin: 0;
              padding: 0;
              font-size: 1.2rem;
              font-weight: bold;
            }
            .text_l {
              text-align: right;
              width: 20rem;
            }
            .arrow {
              color: #ec695e;
              width: 1.5rem;
              .iconify {
                width: 100%;
                height: 100%;
              }
            }
          }
        }
      .img{
        &.img_derecha{
        display: flex;
        justify-content: flex-end;
        }
      .img_revista{
        margin-top: 9rem;
        margin-left: 15rem;
        width: 33rem;
          img{
            width: 100%;
              height: 100%;
              object-fit: cover;
              object-position: center;

          }
       }
        .text_revista{
          position: absolute;
        top: 10.5rem;
        left: 19rem;
        &.text_ident{
          top: 0rem;
          left: 20rem;
        }
        &.text_disco{
        top: 11rem;
        left: 15rem;
        }
        &.text_mermelada{
          top: 3rem;
          left: 27rem;
        }
        .title_revista{
         color: #066772;
          font-size: 1.1rem;
      }
    }
    .img_ident{
      margin-top: -9rem;
      margin-right: 34rem;
      width: 15rem;
      img{
          width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
    .img_disco{
      margin-top: 0rem;
      margin-left: 24rem;
      width: 28rem;
      img{
        width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
    .img_mermelada{
      margin-top: -2rem;
      margin-right: 27rem;
      width: 26rem;
      img{
        width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
      }
    }
}
@media screen and (max-width: 830px) {
    .container_body {
      margin: 2.5rem 1rem 1rem 1rem;
      display: grid;
      grid-template-columns: 50% 50%;
      .titulo {
        grid-column-start: 1;
        grid-column-end: 3;
        font-size: 2rem;
        width: 30rem;
      }
      .texto_corrido_inicial {
    margin-top: 2rem;
    width: 30rem;
      }
        .text_relative {
          position: relative;
          .texto_lateral_index {
            position: absolute;
            display: flex;
            flex-direction: column;
            align-items: flex-end;
            bottom: -10rem;
            right: 0.001rem;
            .titulo_text_l {
              margin: 0;
              padding: 0;
              font-size: 1.2rem;
              font-weight: bold;
            }
            .text_l {
              text-align: right;
              width: 20rem;
            }
            .arrow {
              color: #ec695e;
              width: 1.5rem;
              .iconify {
                width: 100%;
                height: 100%;
              }
            }
          }
        }
      .img{
        grid-column-start: 1;
        grid-column-end: 3;
        &.img_derecha{
        display: flex;
        justify-content: flex-end;
        }
      .img_revista{
        margin-top: 9rem;
        margin-left: 15rem;
        width: 33rem;
          img{
            width: 100%;
              height: 100%;
              object-fit: cover;
              object-position: center;

          }
       }
        .text_revista{
          position: absolute;
        top: 10.5rem;
        left: 19rem;
        &.text_ident{
          top: 0rem;
          left: 20rem;
        }
        &.text_disco{
        top: 11rem;
        left: 15rem;
        }
        &.text_mermelada{
          top: 3rem;
          left: 27rem;
        }
        .title_revista{
         color: #066772;
          font-size: 1.1rem;
      }
    }
    .img_ident{
      margin-top: -9rem;
      margin-right: 31rem;
      width: 15rem;
      img{
          width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
    .img_disco{
      margin-top: 0rem;
      margin-left: 24rem;
      width: 28rem;
      img{
        width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
    .img_mermelada{
      margin-top: -2rem;
      margin-right: 23.7rem;
      width: 26rem;
      img{
        width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
      }
    }
}
@media screen and (max-width: 780px) {
    .container_body {
      margin: 2.5rem 1rem 1rem 1rem;
      display: grid;
      grid-template-columns: 50% 50%;
      .titulo {
        grid-column-start: 1;
        grid-column-end: 3;
        font-size: 2rem;
        width: 30rem;
      }
      .texto_corrido_inicial {
    margin-top: 2rem;
    width: 30rem;
      }
        .text_relative {
          position: relative;
          .texto_lateral_index {
            position: absolute;
            display: flex;
            flex-direction: column;
            align-items: flex-end;
            bottom: -10rem;
            right: 0.001rem;
            .titulo_text_l {
              margin: 0;
              padding: 0;
              font-size: 1.2rem;
              font-weight: bold;
            }
            .text_l {
              text-align: right;
              width: 20rem;
            }
            .arrow {
              color: #ec695e;
              width: 1.5rem;
              .iconify {
                width: 100%;
                height: 100%;
              }
            }
          }
        }
      .img{
        grid-column-start: 1;
        grid-column-end: 3;
        &.img_derecha{
        display: flex;
        justify-content: flex-end;
        }
      .img_revista{
        margin-top: 9rem;
        margin-left: 12rem;
        width: 33rem;
          img{
            width: 100%;
              height: 100%;
              object-fit: cover;
              object-position: center;

          }
       }
        .text_revista{
          position: absolute;
        top: 10.5rem;
        left: 15rem;
        &.text_ident{
          top: 0rem;
          left: 20rem;
        }
        &.text_disco{
        top: 11rem;
        left: 10rem;
        }
        &.text_mermelada{
          top: 3rem;
          left: 27rem;
        }
        .title_revista{
         color: #066772;
          font-size: 1.1rem;
      }
    }
    .img_ident{
      margin-top: -9rem;
      margin-right: 27rem;
      width: 15rem;
      img{
          width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
    .img_disco{
      margin-top: 0rem;
      margin-left: 19rem;
      width: 28rem;
      img{
        width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
    .img_mermelada{
      margin-top: -2rem;
      margin-right: 20rem;
      width: 26rem;
      img{
        width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
      }
    }
}
@media screen and (max-width: 600px) {
    .container_body {
      margin: 2.5rem 1rem 1rem 1rem;
      display: grid;
      grid-template-columns: 50% 50%;
      .titulo {
        grid-column-start: 1;
        grid-column-end: 3;
        font-size: 2rem;
        width: 30rem;
      }
      .texto_corrido_inicial {
        grid-column-start: 1;
        grid-column-end: 3;
        margin-top: 2rem;
        width: 100%;
      }
        .text_relative {
          grid-column-start: 1;
        grid-column-end: 3;
          position: relative;
          .texto_lateral_index {
            position: absolute;
            display: flex;
            flex-direction: column;
            align-items: flex-end;
            bottom: -10rem;
            right: 0.001rem;
            .titulo_text_l {
              margin: 0;
              padding: 0;
              font-size: 1.2rem;
              font-weight: bold;
            }
            .text_l {
              text-align: right;
              width: 20rem;
            }
            .arrow {
              color: #ec695e;
              width: 1.5rem;
              .iconify {
                width: 100%;
                height: 100%;
              }
            }
          }
        }
      .img{
        grid-column-start: 1;
        grid-column-end: 3;
        &.img_derecha{
        display: flex;
        justify-content: flex-end;
        }
      .img_revista{
        margin-top: 9rem;
        margin-left: -4rem;
        width: 27rem;
          img{
            width: 100%;
              height: 100%;
              object-fit: cover;
              object-position: center;

          }
       }
        .text_revista{
          position: absolute;
        top: 20rem;
        left: 0rem;
        &.text_ident{
          top: 5rem;
          left: 14rem;
        }
        &.text_disco{
          z-index: 1;
        top: 16rem;
        left: 10rem;
        }
        &.text_mermelada{
          top: 6rem;
          left: 0rem;
        }
        .title_revista{
         color: #066772;
          font-size: 1.1rem;
      }
    }
    .img_ident{
      margin-top: 2rem;
      margin-right: 10.5rem;
      width: 15rem;
      img{
          width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
    .img_disco{
      margin-top: 0rem;
      margin-left: 0rem;
      width: 23rem;
      img{
        width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
    .img_mermelada{
      margin-top: 13rem;
      margin-right: 0rem;
      width: 26rem;
      img{
        width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
      }
    }
}
@media screen and (max-width: 390px) {
    .container_body {
    
      .img{
      .img_revista{
       }
        .text_revista{
        &.text_ident{
          top: 5rem;
          left: 12rem;
        }
    }
    .img_ident{
      margin-top: 2rem;
      margin-right: 10.5rem;
      width: 15rem;
      img{
          width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
    
      }
    }
}

@media screen and (max-width: 378px) {
    .container_body {
    
      .img{
      .img_revista{
       }
        .text_revista{
        &.text_ident{
          top: 5rem;
          left: 11.5rem;
        }
    }
    .img_ident{
      margin-top: 2rem;
      margin-right: 10.5rem;
      width: 15rem;
      img{
          width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
    
      }
    }
}
@media screen and (max-width: 365px) {
    .container_body {
       .titulo {
        grid-column-start: 1;
        grid-column-end: 3;
        font-size: 1.75rem;
        width: 25rem;
      }
      .img{
      .img_revista{
       }
        .text_revista{
        &.text_ident{
          top: 5rem;
          left: 10.5rem;
        }
    }
    .img_ident{
      margin-top: 2rem;
      margin-right: 10.5rem;
      width: 15rem;
      img{
          width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
    
      }
    }
}
@media screen and (max-width: 340px) {
    .container_body {
       .titulo {
        grid-column-start: 1;
        grid-column-end: 3;
        font-size: 1.75rem;
        width: 25rem;
      }
      .img{
      .img_revista{
       }
        .text_revista{
        &.text_ident{
          top: 5rem;
          left: 9rem;
        }
    }
    .img_ident{
      margin-top: 2rem;
      margin-right: 10.5rem;
      width: 15rem;
      img{
          width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;

      }
    }
    
      }
    }
}
</style>
