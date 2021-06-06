<template>
  <div class="container_body">
    <Title class="titulo" :titleprop="title"> </Title>
    <div class="texto_corrido_inicial">
      El rediseño de FILMIN empieza con un gran proceso de estudio incluyedo
      sistemas como Sitemaps, User Flows, así como creación de Componentes y un
      proceso de diseño desde Low Fi hasta el prototipo High Fi.
      <br />
      <div class="blue">
        (Trabajo completo en Figma, al final de esta página)
      </div>
      <div class="texto_into">
        Empezamos con el rediseño de la marca, simplificándola, manteniendo su
        color corporativo y aludiendo a “lo encendido”.
        <br />
        <span
          class="iconify iconify_1"
          data-icon="akar-icons:arrow-right"
          data-inline="false"
        ></span>
      </div>
    </div>
    <div class="img_filmin_1" data-aos="fade-up" data-aos-duration="2000">
      <img src="/img/filmin/inicio.png" alt="" />
    </div>
    <div class="texto_corrido_inicial inicio_cam_bus">
      <h3 class="subtitle">INICIO, CANALES Y BÚSQUEDA.</h3>
      Rediseño del menú superior, añadiendo Perfil. Bajamos la lupa al menu
      inferior y añadimos el botón de regreso al inicio, para mejorar la
      navegación. Un inicio con carruseles que mejoran la experiencia. Cobran
      importancia los canales principales que esta app nos ofrece, poniéndolos
      en el inico y con una nueva interface. Las colecciones pasan a sugerirse
      en la búsqueda y no como parte del menú principal.
      <span
        class="iconify iconify_2"
        data-icon="akar-icons:arrow-left"
        data-inline="false"
      ></span>
    </div>
    <div class="img_filmin_2">
      <div class="img_one" data-aos="fade-up" data-aos-duration="2000">
        <img src="/img/filmin/HOME.png" alt="" />
      </div>
      <div class="img_two" data-aos="fade-up" data-aos-duration="3000">
        <img src="/img/filmin/CANAL.png" alt="" />
      </div>
      <div class="img_three" data-aos="fade-up" data-aos-duration="3000">
        <img src="/img/filmin/LUPA.png" alt="" />
      </div>
    </div>
    <div class="texto_corrido_inicial pelis_filtr">
      <h3 class="subtitle">PELÍCULAS Y FILTROS.</h3>
      Ahora podemos filtrar por géneros y filtros las películas, series y
      clásicos, acciones que antes el usuario no podía realizar de forma fácil y
      accesible.
    </div>

    <div v-swiper:mySwiper="swiperOption" class="mySwiper">
      <div class="swiper-wrapper">
        <div class="swiper-slide" :key="banner" v-for="banner in banners">
          <img :src="banner" class="img_carr">
        </div>
      </div>
      <div class="swiper-pagination"></div>
    </div>


    <!-- <div class="img_filmin_3">
      <div class="img_one" data-aos="fade-up" data-aos-duration="2000">
        <img src="../static/img/filmin/PELIS_1.png" alt="" />
      </div>
      <div class="img_two" data-aos="fade-up" data-aos-duration="2000">
        <img src="../static/img/filmin/PELIS_2.png" alt="" />
      </div>
      <div class="img_three" data-aos="fade-up" data-aos-duration="2000">
        <img src="../static/img/filmin/PELIS_3.png" alt="" />
      </div>
      <div class="img_three" data-aos="fade-up" data-aos-duration="2000">
        <img src="../static/img/filmin/PELIS_4.png" alt="" />
      </div>
    </div> -->
    <div class="texto_corrido_inicial inicio_cam_bus">
      <h3 class="subtitle">AMIGOS: Nueva experiencia.</h3>
      Se le ofrece al usuario una nueva experiencia, la acción “mis amigos”.
      Poder agregar a personas conocidas a traves un nombre de usuario y
      recomendar contenido sin salirse de la app, asi como ver recomendaciones
      directas o puntos en común con tu amigo.
      <span
        class="iconify iconify_2"
        data-icon="akar-icons:arrow-left"
        data-inline="false"
      ></span>
    </div>
    <div class="img_filmin_4">
      <div class="img_one" data-aos="fade-up" data-aos-duration="2000">
        <img src="/img/filmin/AMIGOS_1.png" alt="" />
      </div>
      <div class="img_two" data-aos="fade-up" data-aos-duration="2000">
        <img src="/img/filmin/AMIGOS_2.png" alt="" />
      </div>
      <div class="img_three" data-aos="fade-up" data-aos-duration="2000">
        <img src="/img/filmin/AMIGOS_3.png" alt="" />
      </div>
    </div>
    <div class="texto_corrido_inicial">
      <span
        class="iconify iconify_3"
        data-icon="akar-icons:arrow-right"
        data-inline="false"
      ></span>
      <h3 class="subtitle">FILMIN KIDS: más seguro.</h3>
      Ahora FILMIN Kids pasa al menu principal. Su color principal cambia para
      convertirse en morado, dando un mejor reconocimiento del cambio de
      contenido y de usuario. Se bloquean todos los botones a excepción del de
      inicio o “return” superior. Si desde “Perfil” se ha configurado
      previamente un pin, este se preguntará siempre que se quiera salir de Kids
      desde los botones accesibles.

    </div>
     <div class="img_filmin_5">
      <div class="img_one" data-aos="fade-up" data-aos-duration="2000">
        <img src="/img/filmin/KIDS_1.png" alt="" />
      </div>
      <div class="img_two" data-aos="fade-up" data-aos-duration="2000">
        <img src="/img/filmin/KIDS_2.png" alt="" />
      </div>
      <div class="img_three" data-aos="fade-up" data-aos-duration="2000">
        <img src="/img/filmin/KIDS_3.png" alt="" />
      </div>
    </div>
    <div class="buttons_link">
      <a href="https://www.figma.com/file/qQ9Z8RBOW9laR918dF5mVt/REDISE%C3%91O-FILMIN?node-id=117%3A0" class="button_link_a button_blue">VER TRABAJO COMPLETO</a>
      <a href="https://www.figma.com/proto/qQ9Z8RBOW9laR918dF5mVt/REDISE%C3%91O-FILMIN?page-id=249%3A18556&node-id=327%3A4845&viewport=618%2C592%2C0.03671981766819954&scaling=min-zoom" class="button_link_a button_pink">VER PROTOTIPO COMPLETO</a>
    </div>
    <div class="happy_path">
      <div class="title">HAPPY PARTHS</div>
      <video src="/img/filmin/happy_path.mp4" autoplay loop></video>
      <video src="/img/filmin/happy_2.mp4" autoplay loop></video>
    </div>
  </div>
</template>

<script>

import Header from "../components/Header.vue";
import Title from "../components/Title.vue";

// SWIPPER
import "swiper/components/pagination/pagination.min.css";
import { directive } from "vue-awesome-swiper";

import SwiperCore, {
  Pagination
} from 'swiper/core';

SwiperCore.use([Pagination]);
// *******

export default {
  components: { Header, Title },
  // data() {
  //   return {
  //     title: '<span class="pink">Rediseño</span> FILMIN app.',
  //   };
  // },

  // SWIPPER
  name: "Slider",
  // computed: {
  //     swiper() {
  //       return this.$refs.mySwiper.$swiper
  //     }
  //   },
  //   mounted() {
  //     console.log('Current Swiper instance object', this.swiper)
  //     this.swiper.slideTo(3, 1000, false)
  //   },
  data() {
    return {
      title: '<span class="pink">Rediseño</span> FILMIN app.',
      banners: ["/img/filmin/PELIS_1.png", "/img/filmin/PELIS_2.png", "/img/filmin/PELIS_3.png", "/img/filmin/PELIS_4.png"],
      swiperOption: {
        
          pagination: {
                el: '.swiper-pagination',
                type: 'bullets',
                //clickable: true
              },
        breakpoints: {
            // 1024: {
            //   slidesPerView: 4,
            //   spaceBetween: 0
            // },
            361 : {
              slidesPerView: 1,
              freeMode: true,
              
              // spaceBetween: 30,
              //centeredSlidesBounds: true
            },
            568: {
              slidesPerView: 4,
              spaceBetween: 30,
              centeredSlides: true,
              freeMode: false,
              
            },
           
            // 530: {
            //   slidesPerView: 4,
            //   spaceBetween: 20,
            //   centeredSlides: true,
            // }
          }
      },
    };
  },
};
</script>

<style lang="scss" scoped >
.container_body {
  // overflow-x: hidden;
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
    .blue {
      font-style: oblique;
      color: #066772;
    }
    &.inicio_cam_bus {
      grid-column-start: 2;
      grid-column-end: 3;
      padding: 0;
      margin-top: 4rem;
      margin-left: 9rem;

      // display: flex;
      // flex-direction: column;
      // align-items: flex-end;

      text-align: right;
    }
    &.pelis_filtr {
      grid-column-start: 1;
      grid-column-end: 3;
    }
    .subtitle {
      font-size: 1.25rem;
      margin: 0 0 0.5rem 0;
    }
    .iconify_2 {
      color: #066772;
      margin: 0 32rem 0 0;
    }
    .iconify_3{
      color: #066772;
      margin: 0rem 0 0 22rem;
    }
  }
  .img_filmin_1 {
    margin-left: 10rem;
    margin-top: -6rem;
    width: 15rem;
    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: center;
    }
  }
  .img_filmin_2 {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-top: -26rem;
    width: 17rem;
    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: center;
    }

    .img_two {
      margin-top: -22rem;
      margin-left: 8rem;
      width: 17rem;
    }
    .img_three {
      margin-top: -22rem;
      margin-left: 16rem;
      width: 17rem;
    }
  }
  .mySwiper {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-top: 2rem;
    margin-left: 3rem;
    width: 100%;
    height: 100%;
    position: relative;
    .swiper-wrapper{
      width: 100%;
      height: 100%;
      display: flex;
      margin-bottom: 2.5rem;
      .swiper-slide{
        text-align: center;
        font-size: 18px;
        background: #fff;
        /* Center slide text vertically */
        display: -webkit-box;
        display: -ms-flexbox;
        display: -webkit-flex;
        display: flex;
        -webkit-box-pack: center;
        -ms-flex-pack: center;
        -webkit-justify-content: center;
        justify-content: center;
        -webkit-box-align: center;
        -ms-flex-align: center;
        -webkit-align-items: center;
        align-items: center;
        width: 60%;
        img {
          display: block;
          width: 100%;
          //height: 100%;
          //object-fit: cover;
          object-position: center;
        }
      }
    }
    .swiper-pagination{

      .swiper-pagination-bullet{
       background: #066772 !important;
       background-color: #066772 !important;

          &.swiper-pagination-bullet-active{
            background: #ec695e !important;
            background-color: #ec695e !important;
          }
      }
    }

  }
  .img_filmin_4 {
     grid-column-start: 1;
    grid-column-end: 3;

    margin-top: -8rem;
    margin-left: 10rem;
    width: 19rem;
    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: center;
    }

    .img_two {
      margin-top: -22rem;
      margin-left: 8rem;
      width: 17rem;
    }
    .img_three {
      margin-top: -22rem;
      width: 17rem;
    }
  }
  .img_filmin_5 {
    margin-top: -26rem;
    margin-left: 5rem;
    width: 19rem;
    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: center;
    }

    .img_two {
      margin-top: -22rem;
      margin-left: 8rem;
      width: 17rem;
    }
    .img_three {
      margin-top: -17rem;
      width: 17rem;
    }
  }
  .buttons_link{
    margin-left: 10rem;
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
        margin-bottom: 1rem;
        background-color: #EC695E;
        &:hover{
          opacity: 100%;
        }
      }
    } 
    
  }
  .happy_path{
    margin-top: 2.5rem ;
    grid-column-start: 1;
    grid-column-end: 3;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;
    .title{
      margin-bottom: 2rem;
      display: flex;
      justify-content: center;
      font-size: 1.5rem;
      color: #066772;
      font-weight: bold;
    }
    video{
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: center;
      margin-bottom:1rem ;
    }
  }
}
@media screen and (max-width: 1340px) {
  .container_body {
      margin: 2.5rem 6rem 1rem 6rem;
      display: grid;
      grid-template-columns: 50% 50%;
      .titulo {
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
        .blue {
          font-style: oblique;
          color: #066772;
        }
        &.inicio_cam_bus {
          grid-column-start: 2;
          grid-column-end: 3;
          padding: 0;
          margin-top: 4rem;
          margin-left: 0rem;

          // display: flex;
          // flex-direction: column;
          // align-items: flex-end;

          text-align: right;
        }
        &.pelis_filtr {
          grid-column-start: 1;
          grid-column-end: 3;
        }
        .subtitle {
          font-size: 1.25rem;
          margin: 0 0 0.5rem 0;
        }
        .iconify_2 {
          color: #066772;
          margin: 0 32rem 0 0;
        }
        .iconify_3{
          color: #066772;
          margin: 0rem 0 0 22rem;
        }
  }
    .img_filmin_1 {
    margin-left: 10rem;
    margin-top: -6rem;
    width: 15rem;
  }
  .img_filmin_2 {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-top: -26rem;
    width: 17rem;

    .img_two {
      margin-top: -22rem;
      margin-left: 8rem;
      width: 17rem;
    }
    .img_three {
      margin-top: -22rem;
      margin-left: 16rem;
      width: 17rem;
    }
  }
  .mySwiper {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-top: 2rem;
    margin-left: 3rem;
    width: 100%;
    height: 100%;
    position: relative;
    .swiper-wrapper{
      width: 100%;
      height: 100%;
      display: flex;
      margin-bottom: 2.5rem;
      .swiper-slide{
        text-align: center;
        font-size: 18px;
        background: #fff;
        /* Center slide text vertically */
        display: -webkit-box;
        display: -ms-flexbox;
        display: -webkit-flex;
        display: flex;
        -webkit-box-pack: center;
        -ms-flex-pack: center;
        -webkit-justify-content: center;
        justify-content: center;
        -webkit-box-align: center;
        -ms-flex-align: center;
        -webkit-align-items: center;
        align-items: center;
        width: 60%;
      }
    }
    .swiper-pagination{

      .swiper-pagination-bullet{
       background: #066772 !important;

          &.swiper-pagination-bullet-active{
            background: #ec695e !important;
          }
      }
    }

  }
  .img_filmin_4 {
     grid-column-start: 1;
    grid-column-end: 3;

    margin-top: -8rem;
    margin-left: 10rem;
    width: 19rem;

    .img_two {
      margin-top: -22rem;
      margin-left: 8rem;
      width: 17rem;
    }
    .img_three {
      margin-top: -22rem;
      width: 17rem;
    }
  }
  .img_filmin_5 {
    margin-top: -26rem;
    margin-left: 5rem;
    width: 19rem;

    .img_two {
      margin-top: -22rem;
      margin-left: 8rem;
      width: 17rem;
    }
    .img_three {
      margin-top: -17rem;
      width: 17rem;
    }
  }
  .buttons_link{
    margin-left: 10rem;
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
        margin-bottom: 1rem;
        background-color: #EC695E;
        &:hover{
          opacity: 100%;
        }
      }
    }
    
  }
  .happy_path{
    margin-top: 2.5rem ;
    grid-column-start: 1;
    grid-column-end: 3;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;
  }
  }
}

@media screen and (max-width: 1190px) {
  .container_body {
      margin: 2.5rem 6rem 1rem 6rem;
      display: grid;
      grid-template-columns: 50% 50%;
      .titulo {
      }
  
    .texto_corrido_inicial {
    position: relative;
    margin-top: 2rem;
    width: 30rem;
        .texto_into {
          margin-left: 0rem;
          position: absolute;
          top: 8rem;
          right: -14rem;
          .iconify_1 {
            color: #066772;
            margin: 0 0 0 19rem;
          }
        }
        .blue {
          font-style: oblique;
          color: #066772;
        }
        &.inicio_cam_bus {
          grid-column-start: 2;
          grid-column-end: 3;
          padding: 0;
          margin-top: 4rem;
          margin-left: 0rem;

          // display: flex;
          // flex-direction: column;
          // align-items: flex-end;

          text-align: right;
        }
        &.pelis_filtr {
          grid-column-start: 1;
          grid-column-end: 3;
        }
        .subtitle {
          font-size: 1.25rem;
          margin: 0 0 0.5rem 0;
        }
        .iconify_2 {
          color: #066772;
          margin: 0 32rem 0 0;
        }
        .iconify_3{
          color: #066772;
          margin: 0rem 0 0 22rem;
        }
  }
    .img_filmin_1 {
    margin-left: 14rem;
    margin-top: -6rem;
    width: 15rem;
  }
  .img_filmin_2 {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-top: -26rem;
    margin-left: -3rem;
    width: 17rem;

    .img_two {
      margin-top: -22rem;
      margin-left: 8rem;
      width: 17rem;
    }
    .img_three {
      margin-top: -22rem;
      margin-left: 16rem;
      width: 17rem;
    }
  }
  .mySwiper {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-top: 2rem;
    margin-left: 3rem;
    width: 100%;
    height: 100%;
    position: relative;
    .swiper-wrapper{
      width: 100%;
      height: 100%;
      display: flex;
      margin-bottom: 2.5rem;
      .swiper-slide{
        text-align: center;
        font-size: 18px;
        background: #fff;
        /* Center slide text vertically */
        display: -webkit-box;
        display: -ms-flexbox;
        display: -webkit-flex;
        display: flex;
        -webkit-box-pack: center;
        -ms-flex-pack: center;
        -webkit-justify-content: center;
        justify-content: center;
        -webkit-box-align: center;
        -ms-flex-align: center;
        -webkit-align-items: center;
        align-items: center;
        width: 60%;
        
      }
    }
    .swiper-pagination{

      .swiper-pagination-bullet{
       background: #066772 !important;

          &.swiper-pagination-bullet-active{
            background: #ec695e !important;
          }
      }
    }

  }
  .img_filmin_4 {
     grid-column-start: 1;
    grid-column-end: 3;

    margin-top: -8rem;
    margin-left: 2rem;
    width: 19rem;

    .img_two {
      margin-top: -22rem;
      margin-left: 8rem;
      width: 17rem;
    }
    .img_three {
      margin-top: -22rem;
      width: 17rem;
    }
  }
  .img_filmin_5 {
    margin-top: -26rem;
    margin-left: 5rem;
    width: 19rem;

    .img_two {
      margin-top: -22rem;
      margin-left: 8rem;
      width: 17rem;
    }
    .img_three {
      margin-top: -17rem;
      width: 17rem;
    }
  }
  .buttons_link{
    margin-left: 0rem;
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
        margin-bottom: 1rem;
        background-color: #EC695E;
        &:hover{
          opacity: 100%;
        }
      }
    }
    
  }
  .happy_path{
    margin-top: 2.5rem ;
    grid-column-start: 1;
    grid-column-end: 3;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;
  }
  }
}

@media screen and (max-width: 1090px) {
  .container_body {
      margin: 2.5rem 6rem 1rem 6rem;
      display: grid;
      grid-template-columns: 50% 50%;
      .titulo {
      }
  
    .texto_corrido_inicial {
    position: relative;
    margin-top: 2rem;
    width: 30rem;
        .texto_into {
          margin-left: 0rem;
          position: absolute;
          top: 8rem;
          right: -14rem;
          .iconify_1 {
            color: #066772;
            margin: 0 0 0 19rem;
          }
        }
        .blue {
          font-style: oblique;
          color: #066772;
        }
        &.inicio_cam_bus {
          grid-column-start: 2;
          grid-column-end: 3;
          padding: 0;
          margin-top: 4rem;
          margin-left: 0rem;

          // display: flex;
          // flex-direction: column;
          // align-items: flex-end;

          text-align: right;
        }
        &.pelis_filtr {
          grid-column-start: 1;
          grid-column-end: 3;
        }
        .subtitle {
          font-size: 1.25rem;
          margin: 0 0 0.5rem 0;
        }
        .iconify_2 {
          color: #066772;
          margin: 0 32rem 0 0;
        }
        .iconify_3{
          color: #066772;
          margin: 0rem 0 0 22rem;
        }
  }
    .img_filmin_1 {
    margin-left: 14rem;
    margin-top: -6rem;
    width: 15rem;
  }
  .img_filmin_2 {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-top: -26rem;
    margin-left: -3rem;
    width: 17rem;

    .img_two {
      margin-top: -22rem;
      margin-left: 8rem;
      width: 17rem;
    }
    .img_three {
      margin-top: -22rem;
      margin-left: 16rem;
      width: 17rem;
    }
  }
  .mySwiper {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-top: .5rem;
    margin-left: 3rem;
    width: 100%;
    height: 100%;
    position: relative;
    .swiper-wrapper{
      width: 100%;
      height: 100%;
      display: flex;
      margin-bottom: 2.5rem;
      .swiper-slide{
        height: 100%;
        width: 275px !important;
        
      }
    }
    .swiper-pagination{

      .swiper-pagination-bullet{
       background: #066772 !important;

          &.swiper-pagination-bullet-active{
            background: #ec695e !important;
          }
      }
    }

  }
  .img_filmin_4 {
     grid-column-start: 1;
    grid-column-end: 3;

    margin-top: -8rem;
    margin-left: 2rem;
    width: 19rem;

    .img_two {
      margin-top: -22rem;
      margin-left: 8rem;
      width: 17rem;
    }
    .img_three {
      margin-top: -22rem;
      width: 17rem;
    }
  }
  .img_filmin_5 {
    margin-top: -26rem;
    margin-left: 5rem;
    width: 19rem;

    .img_two {
      margin-top: -22rem;
      margin-left: 8rem;
      width: 17rem;
    }
    .img_three {
      margin-top: -17rem;
      width: 17rem;
    }
  }
  .buttons_link{
    margin-left: 0rem;
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
        margin-bottom: 1rem;
        background-color: #EC695E;
        &:hover{
          opacity: 100%;
        }
      }
    }
    
  }
  .happy_path{
    margin-top: 2.5rem ;
    grid-column-start: 1;
    grid-column-end: 3;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;
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
    position: relative;
    margin-top: 2rem;
    width: 30rem;
        .texto_into {
          margin-left: 0rem;
          position: absolute;
          top: 8rem;
          right: 0rem;
          width: 25rem;
          .iconify_1 {
            color: #066772;
            margin: 0 0 0 19rem;
          }
        }
        .blue {
          font-style: oblique;
          color: #066772;
        }
        &.inicio_cam_bus {
          grid-column-start: 2;
          grid-column-end: 3;
          padding: 0;
          margin-top: 4rem;
          margin-left: 0rem;
          width: 25rem;

          // display: flex;
          // flex-direction: column;
          // align-items: flex-end;

          text-align: right;
        }
        &.pelis_filtr {
          grid-column-start: 1;
          grid-column-end: 3;
        }
        .subtitle {
          font-size: 1.25rem;
          margin: 0 0 0.5rem 0;
        }
        .iconify_2 {
          color: #066772;
          margin: 0 20rem 0 0;
        }
        .iconify_3{
          color: #066772;
          margin: 0rem 0 0 22rem;
        }
  }
    .img_filmin_1 {
    margin-left: 10rem;
    margin-top: 0rem;
    width: 10rem;
  }
  .img_filmin_2 {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-top: -19rem;
    margin-left: 0rem;
    width: 17rem;

    .img_two {
      margin-top: -22rem;
      margin-left: 8rem;
      width: 17rem;
    }
    .img_three {
      margin-top: -22rem;
      margin-left: 16rem;
      width: 17rem;
    }
  }
  .mySwiper {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-top: .5rem;
    margin-left: 3rem;
    width: 100%;
    height: 100%;
    position: relative;
    .swiper-wrapper{
      width: 100%;
      height: 100%;
      display: flex;
      margin-bottom: 2.5rem;
      .swiper-slide{
        height: 100%;
        width: 275px !important;
        
      }
    }
    .swiper-pagination{

      .swiper-pagination-bullet{
       background: #066772 !important;

          &.swiper-pagination-bullet-active{
            background: #ec695e !important;
          }
      }
    }

  }
  .img_filmin_4 {
     grid-column-start: 1;
    grid-column-end: 3;

    margin-top: -8rem;
    margin-left: 2rem;
    width: 19rem;

    .img_two {
      margin-top: -22rem;
      margin-left: 8rem;
      width: 17rem;
    }
    .img_three {
      margin-top: -22rem;
      width: 17rem;
    }
  }
  .img_filmin_5 {
    margin-top: -26rem;
    margin-left: 0rem;
    width: 19rem;

    .img_two {
      margin-top: -22rem;
      margin-left: 8rem;
      width: 17rem;
    }
    .img_three {
      margin-top: -17rem;
      width: 17rem;
    }
  }
  .buttons_link{
    margin-left: 0rem;
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
        margin-bottom: 1rem;
        background-color: #EC695E;
        &:hover{
          opacity: 100%;
        }
      }
    }
    
  }
  .happy_path{
    margin-top: 2.5rem ;
    grid-column-start: 1;
    grid-column-end: 3;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;
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
    position: relative;
    margin-top: 2rem;
    width: 30rem;
        .texto_into {
          margin-left: 0rem;
          position: absolute;
          top: 8rem;
          right: 0rem;
          width: 25rem;
          .iconify_1 {
            color: #066772;
            margin: 0 0 0 19rem;
          }
        }
        .blue {
          font-style: oblique;
          color: #066772;
        }
        &.inicio_cam_bus {
          grid-column-start: 2;
          grid-column-end: 3;
          padding: 0;
          margin-top: 4rem;
          margin-left: 0rem;
          width: 25rem;

          // display: flex;
          // flex-direction: column;
          // align-items: flex-end;

          text-align: right;
        }
        &.pelis_filtr {
          grid-column-start: 1;
          grid-column-end: 3;
        }
        .subtitle {
          font-size: 1.25rem;
          margin: 0 0 0.5rem 0;
        }
        .iconify_2 {
          color: #066772;
          margin: 0 20rem 0 0;
        }
        .iconify_3{
          color: #066772;
          margin: 0rem 0 0 22rem;
        }
  }
    .img_filmin_1 {
    margin-left: 10rem;
    margin-top: 0rem;
    width: 10rem;
  }
  .img_filmin_2 {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-top: -19rem;
    margin-left: 0rem;
    width: 17rem;

    .img_two {
      margin-top: -22rem;
      margin-left: 8rem;
      width: 17rem;
    }
    .img_three {
      margin-top: -22rem;
      margin-left: 16rem;
      width: 17rem;
    }
  }
  .mySwiper {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-top: .5rem;
    margin-left: 0rem;
    width: 100%;
    height: 100%;
    position: relative;
    .swiper-wrapper{
      width: 100%;
      height: 100%;
      display: flex;
      margin-left: -10rem;
      margin-bottom: 2.5rem;
      .swiper-slide{
        height: 100%;
        width: 275px !important;
        
      }
    }
    .swiper-pagination{

      .swiper-pagination-bullet{
       background: #066772 !important;

          &.swiper-pagination-bullet-active{
            background: #ec695e !important;
          }
      }
    }

  }
  .img_filmin_4 {
     grid-column-start: 1;
    grid-column-end: 3;

    margin-top: -8rem;
    margin-left: 2rem;
    width: 19rem;

    .img_two {
      margin-top: -22rem;
      margin-left: 8rem;
      width: 17rem;
    }
    .img_three {
      margin-top: -22rem;
      width: 17rem;
    }
  }
  .img_filmin_5 {
    margin-top: -26rem;
    margin-left: 0rem;
    width: 19rem;

    .img_two {
      margin-top: -22rem;
      margin-left: 8rem;
      width: 17rem;
    }
    .img_three {
      margin-top: -17rem;
      width: 17rem;
    }
  }
  .buttons_link{
    margin-left: 0rem;
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
        margin-bottom: 1rem;
        background-color: #EC695E;
        &:hover{
          opacity: 100%;
        }
      }
    }
    
  }
  .happy_path{
    margin-top: 2.5rem ;
    grid-column-start: 1;
    grid-column-end: 3;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;
  }
  }
}

@media screen and (max-width: 847px) {
  .container_body {
      margin: 2.5rem 1rem 1rem 1rem;
      display: grid;
      grid-template-columns: 50% 50%;
      .titulo {

      }
  
    .texto_corrido_inicial {
    position: relative;
    margin-top: 2rem;
    width: 30rem;
        .texto_into {
          margin-left: 0rem;
          position: absolute;
          top: 8rem;
          right: 0rem;
          width: 25rem;
          .iconify_1 {
            color: #066772;
            margin: 0 0 0 19rem;
          }
        }
        .blue {
          font-style: oblique;
          color: #066772;
        }
        &.inicio_cam_bus {
          grid-column-start: 2;
          grid-column-end: 3;
          padding: 0;
          margin-top: 4rem;
          margin-left: -1rem;
          width: 25rem;

          // display: flex;
          // flex-direction: column;
          // align-items: flex-end;

          text-align: right;
        }
        &.pelis_filtr {
          grid-column-start: 1;
          grid-column-end: 3;
        }
        .subtitle {
          font-size: 1.25rem;
          margin: 0 0 0.5rem 0;
        }
        .iconify_2 {
          color: #066772;
          margin: 0 20rem 0 0;
        }
        .iconify_3{
          color: #066772;
          margin: 0rem 0 0 22rem;
        }
  }
    .img_filmin_1 {
    margin-left: 10rem;
    margin-top: 0rem;
    width: 10rem;
  }
  .img_filmin_2 {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-top: -19rem;
    margin-left: 0rem;
    width: 17rem;
    .img_one {
      width: 14rem;
    }
    .img_two {
      margin-top: -20rem;
      margin-left: 5rem;
      width: 14rem;
    }
    .img_three {
      margin-top: -20rem;
      margin-left: 11rem;
      width: 14rem;
    }
  }
  .mySwiper {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-top: .5rem;
    margin-left: 0rem;
    width: 100%;
    height: 100%;
    position: relative;
    .swiper-wrapper{
      width: 100%;
      height: 100%;
      display: flex;
      margin-left: -10rem;
      margin-bottom: 2.5rem;
      .swiper-slide{
        height: 100%;
        width: 215px !important;
        
      }
    }
    .swiper-pagination{

      .swiper-pagination-bullet{
       background: #066772 !important;

          &.swiper-pagination-bullet-active{
            background: #ec695e !important;
          }
      }
    }

  }
  .img_filmin_4 {
     grid-column-start: 1;
    grid-column-end: 3;

    margin-top: -8rem;
    margin-left: 2rem;
    width: 19rem;
    .img_one{
     width: 14rem;
    }
    .img_two {
      margin-top: -20rem;
      margin-left: 5rem;
      width: 14rem;
    }
    .img_three {
      margin-top: -19rem;
      width: 14rem;
    }
  }
  .img_filmin_5 {
    margin-top: -26rem;
    margin-left: 0rem;
    width: 19rem;
    .img_one{
     width: 14rem;
    }
    .img_two {
      margin-top: -20rem;
      margin-left: 5rem;
      width: 14rem;
    }
    .img_three {
      margin-top: -15rem;
      width: 14rem;
    }
  }
  .buttons_link{
    margin-left: 0rem;
    margin-top: 1.5rem;
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
        margin-bottom: 1rem;
        background-color: #EC695E;
        &:hover{
          opacity: 100%;
        }
      }
    }
    
  }
  .happy_path{
    margin-top: 2.5rem ;
    grid-column-start: 1;
    grid-column-end: 3;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;
  }
  }
}

@media screen and (max-width: 777px) {
  .container_body {
      margin: 2.5rem 1rem 1rem 1rem;
      display: grid;
      grid-template-columns: 50% 50%;
      .titulo {
        
      }
  
    .texto_corrido_inicial {
    position: relative;
    margin-top: 2rem;
    width: 30rem;
        .texto_into {
          margin-left: 0rem;
          position: absolute;
          top: 8rem;
          right: 0rem;
          left: 0rem;
          width: 25rem;
          .iconify_1 {
            color: #066772;
            margin: 0 0 0 19rem;
            display: none;
          }
        }
        .blue {
          font-style: oblique;
          color: #066772;
        }
        &.inicio_cam_bus {
          grid-column-start: 1;
          grid-column-end: 3;
          padding: 0;
          margin-top: 4rem;
          margin-left: 0rem;
          width: 25rem;

          // display: flex;
          // flex-direction: column;
          // align-items: flex-end;

          text-align: left;
        }
        &.pelis_filtr {
          grid-column-start: 1;
          grid-column-end: 3;
        }
        .subtitle {
          font-size: 1.25rem;
          margin: 0 0 0.5rem 0;
        }
        .iconify_2 {
          color: #066772;
          margin: 0 20rem 0 0;
          display: none;
        }
        .iconify_3{
          color: #066772;
          margin: 0rem 0 0 22rem;
          display: none;
        }
  }
    .img_filmin_1 {
      grid-column-start: 1;
      grid-column-end: 3;
    margin-left: 25rem;
    margin-top: 7rem;
    width: 10rem;
  }
  .img_filmin_2 {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-top: 0rem;
    margin-left: 13rem;
    width: 17rem;
    .img_one {
      width: 14rem;
    }
    .img_two {
      margin-top: -20rem;
      margin-left: 5rem;
      width: 14rem;
    }
    .img_three {
      margin-top: -20rem;
      margin-left: 11rem;
      width: 14rem;
    }
  }
  .mySwiper {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-top: .5rem;
    margin-left: 0rem;
    width: 100%;
    height: 100%;
    position: relative;
    
    .swiper-wrapper{
      max-width: 100%;
      height: 100%;
      display: flex;
      margin-left: 0rem;
      margin-bottom: 2.5rem;
      // transform: translate3d(-516px, 0px, 0px) !important;
      .swiper-slide{
        height: 100%;
        width: 265px !important;
        
      }
    }
    .swiper-pagination{

      .swiper-pagination-bullet{
       background: #066772 !important;

          &.swiper-pagination-bullet-active{
            background: #ec695e !important;
          }
      }
    }

  }
  .img_filmin_4 {
    grid-column-start: 1;
    grid-column-end: 3;

    margin-top: 0rem;
    margin-left: 18rem;
    width: 19rem;
    .img_one{
     width: 14rem;
    }
    .img_two {
      margin-top: -20rem;
      margin-left: 5rem;
      width: 14rem;
    }
    .img_three {
      margin-top: -19rem;
      width: 14rem;
    }
  }
  .img_filmin_5 {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-top: 0rem;
    margin-left: 18rem;
    width: 19rem;
    .img_one{
     width: 14rem;
    }
    .img_two {
      margin-top: -20rem;
      margin-left: 5rem;
      width: 14rem;
    }
    .img_three {
      margin-top: -15rem;
      width: 14rem;
    }
  }
  .buttons_link{
    grid-column-start: 1;
    grid-column-end: 3;
    margin-left: 0rem;
    margin-top: 1.5rem;
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
        margin-bottom: 1rem;
        background-color: #EC695E;
        &:hover{
          opacity: 100%;
        }
      }
    }
    
  }
  .happy_path{
    margin-top: 2.5rem ;
    grid-column-start: 1;
    grid-column-end: 3;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;
  }
  }
}

@media screen and (max-width: 637px) {
  .container_body {
      margin: 2.5rem 1rem 1rem 1rem;
      display: grid;
      grid-template-columns: 50% 50%;
      .titulo {
        
      }
  
    .texto_corrido_inicial {
    position: relative;
    margin-top: 2rem;
    width: 30rem;
        .texto_into {
          margin-left: 0rem;
          position: absolute;
          top: 8rem;
          right: 0rem;
          left: 0rem;
          width: 25rem;
          .iconify_1 {
            color: #066772;
            margin: 0 0 0 19rem;
            display: none;
          }
        }
        .blue {
          font-style: oblique;
          color: #066772;
        }
        &.inicio_cam_bus {
          grid-column-start: 1;
          grid-column-end: 3;
          padding: 0;
          margin-top: 4rem;
          margin-left: 0rem;
          width: 25rem;

          // display: flex;
          // flex-direction: column;
          // align-items: flex-end;

          text-align: left;
        }
        &.pelis_filtr {
          grid-column-start: 1;
          grid-column-end: 3;
        }
        .subtitle {
          font-size: 1.25rem;
          margin: 0 0 0.5rem 0;
        }
        .iconify_2 {
          color: #066772;
          margin: 0 20rem 0 0;
          display: none;
        }
        .iconify_3{
          color: #066772;
          margin: 0rem 0 0 22rem;
          display: none;
        }
  }
    .img_filmin_1 {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-left: 13rem;
    margin-top: 7rem;
    width: 10rem;
  }
  .img_filmin_2 {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-top: 0rem;
    margin-left: 5rem;
    width: 17rem;
    .img_one {
      width: 14rem;
    }
    .img_two {
      margin-top: -20rem;
      margin-left: 5rem;
      width: 14rem;
    }
    .img_three {
      margin-top: -20rem;
      margin-left: 11rem;
      width: 14rem;
    }
  }
  .mySwiper {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-top: .5rem;
    margin-left: 0rem;
    width: 100%;
    height: 100%;
    position: relative;
    .swiper-wrapper{
      width: 100%;
      height: 100%;
      display: flex;
      margin-left: 0rem;
      margin-bottom: 2.5rem;
      .swiper-slide{
        height: 100%;
        width: 235px !important;
        
      }
    }
    .swiper-pagination{

      .swiper-pagination-bullet{
       background: #066772 !important;

          &.swiper-pagination-bullet-active{
            background: #ec695e !important;
          }
      }
    }

  }
  .img_filmin_4 {
    grid-column-start: 1;
    grid-column-end: 3;

    margin-top: 0rem;
    margin-left: 9rem;
    width: 19rem;
    .img_one{
     width: 14rem;
    }
    .img_two {
      margin-top: -20rem;
      margin-left: 5rem;
      width: 14rem;
    }
    .img_three {
      margin-top: -19rem;
      width: 14rem;
    }
  }
  .img_filmin_5 {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-top: 0rem;
    margin-left: 9rem;
    width: 19rem;
    .img_one{
     width: 14rem;
    }
    .img_two {
      margin-top: -20rem;
      margin-left: 5rem;
      width: 14rem;
    }
    .img_three {
      margin-top: -15rem;
      width: 14rem;
    }
  }
  .buttons_link{
    grid-column-start: 1;
    grid-column-end: 3;
    margin-left: 0rem;
    margin-top: 1.5rem;
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
        margin-bottom: 1rem;
        background-color: #EC695E;
        &:hover{
          opacity: 100%;
        }
      }
    }
    
  }
  .happy_path{
    margin-top: 2.5rem ;
    grid-column-start: 1;
    grid-column-end: 3;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;
  }
  }
}

@media screen and (max-width: 530px) {
  .container_body {
      margin: 2.5rem 1rem 1rem 1rem;
      display: grid;
      grid-template-columns: 50% 50%;
      .titulo {
        
      }
  
    .texto_corrido_inicial {
    position: relative;
    margin-top: 2rem;
    width: 20rem;
        .texto_into {
          margin-left: 0rem;
          position: absolute;
          top: 10rem;
          right: 0rem;
          left: 0rem;
          width: 20rem;
          .iconify_1 {
            color: #066772;
            margin: 0 0 0 19rem;
            display: none;
          }
        }
        .blue {
          font-style: oblique;
          color: #066772;
        }
        &.inicio_cam_bus {
          grid-column-start: 1;
          grid-column-end: 3;
          padding: 0;
          margin-top: 4rem;
          margin-left: 0rem;
          width: 20rem;

          // display: flex;
          // flex-direction: column;
          // align-items: flex-end;

          text-align: left;
        }
        &.pelis_filtr {
          grid-column-start: 1;
          grid-column-end: 3;
        }
        .subtitle {
          font-size: 1.25rem;
          margin: 0 0 0.5rem 0;
        }
        .iconify_2 {
          color: #066772;
          margin: 0 20rem 0 0;
          display: none;
        }
        .iconify_3{
          color: #066772;
          margin: 0rem 0 0 22rem;
          display: none;
        }
  }
    .img_filmin_1 {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-left: 13rem;
    margin-top: 7rem;
    width: 10rem;
  }
  .img_filmin_2 {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-top: 0rem;
    margin-left: 5rem;
    width: 17rem;
    .img_one {
      width: 14rem;
    }
    .img_two {
      margin-top: -20rem;
      margin-left: 5rem;
      width: 14rem;
    }
    .img_three {
      margin-top: -20rem;
      margin-left: 11rem;
      width: 14rem;
    }
  }
  .mySwiper {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-top: .5rem;
    margin-left: 0rem;
    width: 100%;
    height: 100%;
    position: relative;
    .swiper-wrapper{
      width: 100%;
      height: 100%;
      display: flex;
      margin-left: 2rem;
      margin-bottom: 2.5rem;
      .swiper-slide{
        height: 100%;
        width: 235px !important;
        
      }
    }
    .swiper-pagination{
      display: none;
      .swiper-pagination-bullet{
       background: #066772 !important;

          &.swiper-pagination-bullet-active{
            background: #ec695e !important;
          }
      }
    }

  }
  .img_filmin_4 {
    grid-column-start: 1;
    grid-column-end: 3;

    margin-top: 0rem;
    margin-left: 9rem;
    width: 19rem;
    .img_one{
     width: 14rem;
    }
    .img_two {
      margin-top: -20rem;
      margin-left: 5rem;
      width: 14rem;
    }
    .img_three {
      margin-top: -19rem;
      width: 14rem;
    }
  }
  .img_filmin_5 {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-top: 0rem;
    margin-left: 9rem;
    width: 19rem;
    .img_one{
     width: 14rem;
    }
    .img_two {
      margin-top: -20rem;
      margin-left: 5rem;
      width: 14rem;
    }
    .img_three {
      margin-top: -15rem;
      width: 14rem;
    }
  }
  .buttons_link{
    grid-column-start: 1;
    grid-column-end: 3;
    margin-left: 0rem;
    margin-top: 1.5rem;
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
        margin-bottom: 1rem;
        background-color: #EC695E;
        &:hover{
          opacity: 100%;
        }
      }
    }
    
  }
  .happy_path{
    margin-top: 2.5rem ;
    grid-column-start: 1;
    grid-column-end: 3;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;
    video{
      width: 140%;
      height: 140%;
      object-fit: cover;
      object-position: center;
      margin-bottom:1rem ;
    }
  }
  }
}
@media screen and (max-width: 430px) {
  .container_body {
      margin: 2.5rem 1rem 1rem 1rem;
      display: grid;
      grid-template-columns: 50% 50%;
      .titulo {
        
      }
  
    .texto_corrido_inicial {
    position: relative;
    margin-top: 2rem;
    width: 20rem;
        .texto_into {
          margin-left: 0rem;
          position: absolute;
          top: 10rem;
          right: 0rem;
          left: 0rem;
          width: 20rem;
          .iconify_1 {
            color: #066772;
            margin: 0 0 0 19rem;
            display: none;
          }
        }
        .blue {
          font-style: oblique;
          color: #066772;
        }
        &.inicio_cam_bus {
          grid-column-start: 1;
          grid-column-end: 3;
          padding: 0;
          margin-top: 4rem;
          margin-left: 0rem;
          width: 20rem;

          // display: flex;
          // flex-direction: column;
          // align-items: flex-end;

          text-align: left;
        }
        &.pelis_filtr {
          grid-column-start: 1;
          grid-column-end: 3;
        }
        .subtitle {
          font-size: 1.25rem;
          margin: 0 0 0.5rem 0;
        }
        .iconify_2 {
          color: #066772;
          margin: 0 20rem 0 0;
          display: none;
        }
        .iconify_3{
          color: #066772;
          margin: 0rem 0 0 22rem;
          display: none;
        }
  }
    .img_filmin_1 {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-left: 4rem;
    margin-top: 7rem;
    width: 10rem;
  }
  .img_filmin_2 {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-top: 0rem;
    margin-left: -.5rem;
    width: 17rem;
    .img_one {
      width: 12rem;
    }
    .img_two {
      margin-top: -17rem;
      margin-left: 4rem;
      width: 12rem;
    }
    .img_three {
      margin-top: -17rem;
      margin-left: 8rem;
      width: 12rem;
    }
  }
  .mySwiper {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-top: .5rem;
    margin-left: 0rem;
    width: 100%;
    height: 100%;
    position: relative;
    .swiper-wrapper{
      width: 100%;
      height: 100%;
      display: flex;
      margin-left: 2rem;
      margin-bottom: 2.5rem;
      .swiper-slide{
        height: 100%;
        width: 195px !important;
        
      }
    }
    .swiper-pagination{

      .swiper-pagination-bullet{
       background: #066772 !important;

          &.swiper-pagination-bullet-active{
            background: #ec695e !important;
          }
      }
    }

  }
  .img_filmin_4 {
    grid-column-start: 1;
    grid-column-end: 3;

    margin-top: 0rem;
    margin-left: 0rem;
    width: 19rem;
    .img_one{
     width: 14rem;
    }
    .img_two {
      margin-top: -20rem;
      margin-left: 5rem;
      width: 14rem;
    }
    .img_three {
      margin-top: -19rem;
      width: 14rem;
    }
  }
  .img_filmin_5 {
    grid-column-start: 1;
    grid-column-end: 3;
    margin-top: 0rem;
    margin-left: 0rem;
    width: 19rem;
    .img_one{
     width: 14rem;
    }
    .img_two {
      margin-top: -20rem;
      margin-left: 5rem;
      width: 14rem;
    }
    .img_three {
      margin-top: -15rem;
      width: 14rem;
    }
  }
  .buttons_link{
    grid-column-start: 1;
    grid-column-end: 3;
    margin-left: 0rem;
    margin-top: 1.5rem;
    width: 100%;
    display: flex;
    flex-direction: column;
    .button_link_a{
      display: flex;
      justify-content: center;
      align-items: center;

      color: white;
      padding: .75rem 2rem;
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
        margin-bottom: 1rem;
        background-color: #EC695E;
        &:hover{
          opacity: 100%;
        }
      }
    }
    
  }
  .happy_path{
    margin-top: 2.5rem ;
    grid-column-start: 1;
    grid-column-end: 3;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;
    video{
      width: 210%;
      height: 210%;
      object-fit: cover;
      object-position: center;
      margin-bottom:1rem ;
    }
  }
  }
}



// 530px - width: 20rem; de los textos iniciales
</style>
