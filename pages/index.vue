<template>
  <div class="container_body">
    <Title 
      class="titulo" 
      :titleprop="title"></Title>
    <div class="texto_corrido_inicial">
      Estudiando diseño gráfico, me he dado cuenta que mi pasión es crear diseño de interfaces para que usuarios y el mundo digital, conecten entre ellos. Busco crear productos digitales teniendo en cuenta todos sus procesos para conseguir un diseño sólido, una buena experiencia e interface.
    </div>
    <div class="text_relative">
        <div class="texto_lateral_index">
            <div class="titulo_text_l">ALGUNOS TRABAJOS UX/UI</div>
            <div class="text_l">
              Estos son algunos de mis proyectos con los que mejor me siento teniendo en cuenta mi calidad de estudiante.
            </div>
             <div class="arrow" data-aos="fade-down-left" data-aos-duration="2000"><span class="iconify" data-icon="carbon:arrow-down-left" data-inline="false"></span></div>
        </div>
    </div>
    <div class="texto_plus_rosa" data-aos="fade-right"
     data-aos-offset="300"
     data-aos-easing="ease-in-sine">
    Esta web está diseñada y programada íntegramente por mí. Navegad como si de un trabajo más se tratase.
    </div>
    <div></div>
    <div></div>
    <div class="imgs">
      <div class="img_filmin" data-aos="fade-up" data-aos-duration="2000">
        <img src="/img/home.png" alt="">
      </div>
      <div class="text_filmin">
        <div class="title_filmin">
          Rediseño
        </div>
        <div class="texto">
          de la app de FILMIN y su identidad.
        </div>
        <div class="leer_mas">
          <NuxtLink class="leer_mas_nuxt" to="filmin">Leer más <span class="iconify" data-icon="akar-icons:circle-plus" data-inline="false"></span> </NuxtLink>
        </div>
      </div>
    </div>
    <div class="imgs_2">
      <div class="img_filmin" data-aos="fade-up" data-aos-duration="2000">
        <img src="/img/marte_1.png" alt="">
      </div>
      <div class="text_filmin">
        <div class="title_filmin">
          Diseño y programación
        </div>
        <div class="texto">
          de una app del tiempo de Marte.

        </div>
        <div class="leer_mas">
          <NuxtLink class="leer_mas_nuxt" to="marte">Leer más <span class="iconify" data-icon="akar-icons:circle-plus" data-inline="false"></span> </NuxtLink>
        </div>
      </div>
      <div class="contact">
          <NuxtLink class="leer_mas_nuxt" to="contacto">Contacto<span class="iconify" data-icon="akar-icons:circle-plus" data-inline="false"></span> </NuxtLink>
      </div>
    </div>
  </div>
  
</template>

<script>
import Header from '../components/Header.vue'
import Title from '../components/Title.vue'
export default {

  components: { Header, Title },
  data(){
    return {
        title: 'Hola, soy <br> <span class="blue">Christian Valencia</span>, diseñador <span class="pink">gráfico & UX UI</span>, basado en Madrid.',
      }
    
  }
  
}
</script>

<style lang="scss" scoped>

.container_body {
  // overflow-x: hidden;
  margin: 2.5rem 6rem 1rem 6rem;
  display: grid;
  grid-template-columns: 50% 50%;
  .titulo{
    grid-column-start: 1;
    grid-column-end: 3;
  }
  .texto_corrido_inicial{
    margin-top: 2rem;
    width: 30rem;
  }
  .texto_plus_rosa{
    margin-top: 1rem;
    width: 30rem;
    color: #EC695E;
    font-style: oblique;
  }
  .text_relative{
    position: relative;
    .texto_lateral_index{
    position: absolute;
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    bottom: -6rem;
    right: .001rem;
    .titulo_text_l{
      margin: 0;
      padding: 0;
      font-size: 1.5rem;
      font-weight: bold;
    }
    .text_l{
      text-align: right;
      width: 20rem;
    }
    .arrow{
      color: #EC695E;
      width: 2rem;
      .iconify{
        width: 100%;
        height: 100%;
      }
    }
  }
  }
  .imgs{
    position: relative;
      .img_filmin{
        position: absolute;
        top: -10rem;
        right: 16rem;
        width: 30rem;
        img{
          width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;
        }
      }
      .text_filmin{
        position: absolute;
        top: 10rem;
        left: 20rem;
        .title_filmin{
          color: #066772;
          font-size: 1.2rem;

        }
        .texto{
          width: 10rem;
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
    .imgs_2{
    position: relative;
      .img_filmin{
        position: absolute;
        top: 16rem;
        left: 17rem;
        width: 18rem;
        img{
          width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;
        }
      }
      .text_filmin{
        position: absolute;
        top: 14rem;
        left: 11rem;
        .title_filmin{
          color: #066772;
          font-size: 1.2rem;

        }
        .texto{
          width: 10rem;
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
      .contact{
        position: absolute;
        top: 48rem;
        left: 37rem;
        color: #EC695E;
          .leer_mas_nuxt{
            position: relative;
            color: #EC695E;
            .iconify{
              position: absolute;
              top: .2rem;
              left: 4rem;
            }
            &:hover{
              color: #066772;
            }
          }
      } 
    }
  
}
// tablet
  @media screen and (max-width: 1384px) {
      .container_body {
        margin: 2.5rem 6rem 1rem 6rem;
        display: grid;
        grid-template-columns: 50% 50%;
        .titulo{
          grid-column-start: 1;
          grid-column-end: 3;
        }
        .imgs{
          position: relative;
          .img_filmin{
            position: absolute;
            top: -10rem;
            right: 11rem;
            width: 30rem;
            img{
              width: 100%;
              height: 100%;
              object-fit: cover;
              object-position: center;
            }
          }
          .text_filmin{
            position: absolute;
            top: 10rem;
            left: 22rem;
            .title_filmin{
              color: #066772;
              font-size: 1.2rem;

            }
            .texto{
              width: 10rem;
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
// tablet
  @media screen and (max-width: 1224px) {
      .container_body {
        margin: 2.5rem 6rem 1rem 6rem;
        display: grid;
        grid-template-columns: 50% 50%;
        .titulo{
          grid-column-start: 1;
          grid-column-end: 3;
        }
        .imgs{
          position: relative;
          .img_filmin{
            position: absolute;
            top: -5rem;
            right: 8rem;
            width: 30rem;
            img{
              width: 100%;
              height: 100%;
              object-fit: cover;
              object-position: center;
            }
          }
          .text_filmin{
            position: absolute;
            top: 7rem;
            left: 18rem;
            
          }  
        }
        .imgs_2{
          position: relative;
        .img_filmin{
          position: absolute;
          top: 16rem;
          left: 10rem;
          width: 18rem;
          img{
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: center;
          }
        }
        .text_filmin{
          position: absolute;
          top: 14rem;
          left: 4rem;
          
        }
        .contact{
          position: absolute;
          top: 48rem;
          left: 30rem;
          color: #EC695E;
            .leer_mas_nuxt{
              position: relative;
              color: #EC695E;
              .iconify{
                position: absolute;
                top: .2rem;
                left: 4rem;
              }
              &:hover{
                color: #066772;
              }
            }
        } 
      }
      }
    
  }
// tablet
  @media screen and (max-width: 1124px) {
      .container_body {
        margin: 2.5rem 6rem 1rem 6rem;
        display: grid;
        grid-template-columns: 50% 50%;
        .titulo{
          grid-column-start: 1;
          grid-column-end: 3;
        }
        .imgs{
          position: relative;
          .img_filmin{
            position: absolute;
            top: -1rem;
            right: 7rem;
            width: 25rem;
            img{
              width: 100%;
              height: 100%;
              object-fit: cover;
              object-position: center;
            }
          }
          .text_filmin{
            position: absolute;
            top: 7rem;
            left: 18rem;
            
          }  
        }
        .imgs_2{
          position: relative;
        .img_filmin{
          position: absolute;
          top: 16rem;
          left: 10rem;
          width: 16rem;
          img{
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: center;
          }
        }
        .text_filmin{
          position: absolute;
          top: 14rem;
          left: 4rem;
          
        }
        .contact{
          position: absolute;
          top: 48rem;
          left: 30rem;
          color: #EC695E;
            .leer_mas_nuxt{
              position: relative;
              color: #EC695E;
              .iconify{
                position: absolute;
                top: .2rem;
                left: 4rem;
              }
              &:hover{
                color: #066772;
              }
            }
        } 
      }
      }
    
  }  
// tablet
  @media screen and (max-width: 1064px) {
      .container_body {
        margin: 2.5rem 6rem 1rem 6rem;
        display: grid;
        grid-template-columns: 50% 50%;
        .titulo{
          grid-column-start: 1;
          grid-column-end: 3;
        }
        .imgs{
          position: relative;
          .img_filmin{
            position: absolute;
            top: -1rem;
            right: 11rem;
            width: 25rem;
            img{
              width: 100%;
              height: 100%;
              object-fit: cover;
              object-position: center;
            }
          }
          .text_filmin{
            position: absolute;
            top: 7rem;
            left: 13rem;
            
          }  
        }
        .imgs_2{
          position: relative;
        .img_filmin{
          position: absolute;
          top: 16rem;
          left: 5rem;
          width: 16rem;
          img{
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: center;
          }
        }
        .text_filmin{
          position: absolute;
          top: 14rem;
          left: 0rem;
          
        }
        .contact{
          position: absolute;
          top: 48rem;
          left: 30rem;
          color: #EC695E;
            .leer_mas_nuxt{
              position: relative;
              color: #EC695E;
              .iconify{
                position: absolute;
                top: .2rem;
                left: 4rem;
              }
              &:hover{
                color: #066772;
              }
            }
        } 
      }
      }
    
  }
// tablet
  @media screen and (max-width: 1024px) {
      .container_body {
        margin: 2.5rem 2rem 1rem 2rem;
        display: grid;
        grid-template-columns: 50% 50%;
        .titulo{
          grid-column-start: 1;
          grid-column-end: 3;
        }
        .imgs{
          position: relative;
          .img_filmin{
            position: absolute;
            top: -1rem;
            right: 13rem;
            width: 25rem;
            img{
              width: 100%;
              height: 100%;
              object-fit: cover;
              object-position: center;
            }
          }
          .text_filmin{
            position: absolute;
            top: 7rem;
            left: 13rem;
            
          }  
        }
        
      }
    
  } 
// tablet
  @media screen and (max-width: 954px) {
      .container_body {
        margin: 2.5rem 1rem 1rem 1rem;
        display: grid;
        grid-template-columns: 50% 50%;
        .titulo{
          grid-column-start: 1;
          grid-column-end: 3;
          font-size: 2rem;
          width: 30rem;
        }
        .texto_corrido_inicial{
          margin-top: 2rem;
          width: 30rem;
        }
        .texto_plus_rosa{
          margin-top: 1rem;
          width: 30rem;
          color: #EC695E;
          font-style: oblique;
        }
        .text_relative{
          position: relative;
          .texto_lateral_index{
          position: absolute;
          display: flex;
          flex-direction: column;
          align-items: flex-end;
          bottom: -13rem;
          right: .001rem;
          .titulo_text_l{
            margin: 0;
            padding: 0;
            font-size: 1.5rem;
            font-weight: bold;
          }
          .text_l{
            text-align: right;
            width: 20rem;
          }
          .arrow{
            color: #EC695E;
            width: 2rem;
            .iconify{
              width: 100%;
              height: 100%;
            }
          }
        }
        }
        .imgs{
          position: relative;
          .img_filmin{
            position: absolute;
            top: 2rem;
            right: 18rem;
            width: 20rem;
            img{
              width: 100%;
              height: 100%;
              object-fit: cover;
              object-position: center;
            }
          }
          .text_filmin{
            position: absolute;
            top: 10rem;
            left: 9rem;
            
          }  
        }
        .imgs_2{
          position: relative;
        .img_filmin{
          position: absolute;
          top: 16rem;
          left: 7rem;
          width: 12rem;
          img{
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: center;
          }
        }
        .text_filmin{
          position: absolute;
          top: 13rem;
          left: 0rem;
          
        }
        .contact{
          position: absolute;
          top: 38rem;
          left: 20rem;
          color: #EC695E;
            .leer_mas_nuxt{
              position: relative;
              color: #EC695E;
              .iconify{
                position: absolute;
                top: .2rem;
                left: 4rem;
              }
              &:hover{
                color: #066772;
              }
            }
        } 
      }
      }
    
  }
    @media screen and (max-width: 850px) {
      .container_body {
        margin: 2.5rem 1rem 1rem 1rem;
        display: grid;
        grid-template-columns: 50% 50%;
        .titulo{
          grid-column-start: 1;
          grid-column-end: 3;
          font-size: 2rem;
          width: 30rem;
        }
        .texto_corrido_inicial{
          margin-top: 2rem;
          width: 30rem;
        }
        .texto_plus_rosa{
          margin-top: 1rem;
          width: 30rem;
          color: #EC695E;
          font-style: oblique;
        }
        .text_relative{
          position: relative;
          .texto_lateral_index{
          position: absolute;
          display: flex;
          flex-direction: column;
          align-items: flex-end;
          bottom: -13rem;
          right: .001rem;
          .titulo_text_l{
            margin: 0;
            padding: 0;
            font-size: 1.5rem;
            font-weight: bold;
          }
          .text_l{
            text-align: right;
            width: 20rem;
          }
          .arrow{
            color: #EC695E;
            width: 2rem;
            .iconify{
              width: 100%;
              height: 100%;
            }
          }
        }
        }
        .imgs{
          position: relative;
          .img_filmin{
            position: absolute;
            top: 2rem;
            right: 14rem;
            width: 20rem;
            img{
              width: 100%;
              height: 100%;
              object-fit: cover;
              object-position: center;
            }
          }
          .text_filmin{
            position: absolute;
            top: 10rem;
            left: 9rem;
            
          }  
        }
        .imgs_2{
          position: relative;
        .img_filmin{
          position: absolute;
          top: 16rem;
          left: 7rem;
          width: 12rem;
          img{
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: center;
          }
        }
        .text_filmin{
          position: absolute;
          top: 13rem;
          left: 0rem;
          
        }
        .contact{
          position: absolute;
          top: 38rem;
          left: 20rem;
          color: #EC695E;
            .leer_mas_nuxt{
              position: relative;
              color: #EC695E;
              .iconify{
                position: absolute;
                top: .2rem;
                left: 4rem;
              }
              &:hover{
                color: #066772;
              }
            }
        } 
      }
      }
    
  }
  // tablet
  @media screen and (max-width: 775px) {
      .container_body {
        margin: 2.5rem 2rem 1rem 2rem;
        display: grid;
        grid-template-columns: 50% 50%;
        .titulo{
          grid-column-start: 1;
          grid-column-end: 3;
          font-size: 2rem;
          width: 30rem;
        }
        .texto_corrido_inicial{
          margin-top: 2rem;
          width: 30rem;
        }
        .texto_plus_rosa{
          margin-top: 1rem;
          width: 30rem;
          color: #EC695E;
          font-style: oblique;
        }
        .text_relative{
          position: relative;
          .texto_lateral_index{
          position: absolute;
          display: flex;
          flex-direction: column;
          align-items: flex-end;
          bottom: -13rem;
          right: .001rem;
          .titulo_text_l{
            margin: 0;
            padding: 0;
            font-size: 1.5rem;
            font-weight: bold;
          }
          .text_l{
            text-align: right;
            width: 20rem;
          }
          .arrow{
            color: #EC695E;
            width: 2rem;
            .iconify{
              width: 100%;
              height: 100%;
            }
          }
        }
        }
        .imgs{
          position: relative;
          .img_filmin{
            position: absolute;
            top: 7rem;
            right: 8rem;
            width: 20rem;
            img{
              width: 100%;
              height: 100%;
              object-fit: cover;
              object-position: center;
            }
          }
          .text_filmin{
            position: absolute;
            top: 13rem;
            left: 10.5rem;
            
          }  
        }
        .imgs_2{
          position: relative;
        .img_filmin{
          position: absolute;
          top: 23rem;
          left: 7rem;
          width: 12rem;
          img{
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: center;
          }
        }
        .text_filmin{
          position: absolute;
          top: 19rem;
          left: 0rem;
          
        }
        .contact{
          position: absolute;
          top: 45rem;
          left: 20rem;
          color: #EC695E;
            .leer_mas_nuxt{
              position: relative;
              color: #EC695E;
              .iconify{
                position: absolute;
                top: .2rem;
                left: 4rem;
              }
              &:hover{
                color: #066772;
              }
            }
        } 
      }
      }
    
  }
  @media screen and (max-width: 722px) {
      .container_body {
        margin: 2.5rem 2rem 1rem 2rem;
        display: grid;
        grid-template-columns: 50% 50%;
        .titulo{
          grid-column-start: 1;
          grid-column-end: 3;
          font-size: 2rem;
          width: 30rem;
        }
        .texto_corrido_inicial{
          margin-top: 2rem;
          width: 30rem;
        }
        .texto_plus_rosa{
          margin-top: 1rem;
          width: 30rem;
          color: #EC695E;
          font-style: oblique;
        }
        .text_relative{
          position: relative;
          .texto_lateral_index{
          position: absolute;
          display: flex;
          flex-direction: column;
          align-items: flex-end;
          bottom: -13rem;
          right: .001rem;
          .titulo_text_l{
            margin: 0;
            padding: 0;
            font-size: 1.5rem;
            font-weight: bold;
          }
          .text_l{
            text-align: right;
            width: 20rem;
          }
          .arrow{
            color: #EC695E;
            width: 2rem;
            .iconify{
              width: 100%;
              height: 100%;
            }
          }
        }
        }
        .imgs{
          position: relative;
          .img_filmin{
            position: absolute;
            top: 7rem;
            right: 6rem;
            width: 20rem;
            img{
              width: 100%;
              height: 100%;
              object-fit: cover;
              object-position: center;
            }
          }
          .text_filmin{
            position: absolute;
            top: 13rem;
            left: 10.5rem;
            
          }  
        }
        .imgs_2{
          position: relative;
        .img_filmin{
          position: absolute;
          top: 23rem;
          left: 7rem;
          width: 12rem;
          img{
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: center;
          }
        }
        .text_filmin{
          position: absolute;
          top: 19rem;
          left: 0rem;
          
        }
        .contact{
          position: absolute;
          top: 45rem;
          left: 20rem;
          color: #EC695E;
            .leer_mas_nuxt{
              position: relative;
              color: #EC695E;
              .iconify{
                position: absolute;
                top: .2rem;
                left: 4rem;
              }
              &:hover{
                color: #066772;
              }
            }
        } 
      }
      }
    
  }
    @media screen and (max-width: 722px) {
      .container_body {
        margin: 2.5rem 2rem 1rem 2rem;
        display: grid;
        grid-template-columns: 50% 50%;
        .titulo{
          grid-column-start: 1;
          grid-column-end: 3;
          font-size: 2rem;
          width: 30rem;
        }
        .texto_corrido_inicial{
          margin-top: 2rem;
          width: 30rem;
        }
        .texto_plus_rosa{
          margin-top: 1rem;
          width: 30rem;
          color: #EC695E;
          font-style: oblique;
        }
        .text_relative{
          position: relative;
          .texto_lateral_index{
          position: absolute;
          display: flex;
          flex-direction: column;
          align-items: flex-end;
          bottom: -13rem;
          right: .001rem;
          .titulo_text_l{
            margin: 0;
            padding: 0;
            font-size: 1.5rem;
            font-weight: bold;
          }
          .text_l{
            text-align: right;
            width: 20rem;
          }
          .arrow{
            color: #EC695E;
            width: 2rem;
            .iconify{
              width: 100%;
              height: 100%;
            }
          }
        }
        }
        .imgs{
          position: relative;
          .img_filmin{
            position: absolute;
            top: 7rem;
            right: 5rem;
            width: 18rem;
            img{
              width: 100%;
              height: 100%;
              object-fit: cover;
              object-position: center;
            }
          }
          .text_filmin{
            position: absolute;
            top: 13rem;
            left: 10.5rem;
            
          }  
        }
        .imgs_2{
          position: relative;
        .img_filmin{
          position: absolute;
          top: 23rem;
          left: 5.5rem;
          width: 11rem;
          img{
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: center;
          }
        }
        .text_filmin{
          position: absolute;
          top: 19rem;
          left: 0rem;
          
        }
        .contact{
          position: absolute;
          top: 45rem;
          left: 20rem;
          color: #EC695E;
            .leer_mas_nuxt{
              position: relative;
              color: #EC695E;
              .iconify{
                position: absolute;
                top: .2rem;
                left: 4rem;
              }
              &:hover{
                color: #066772;
              }
            }
        } 
      }
      }
    
  }
// tlf
  @media screen and (max-width: 600px) {
      .container_body {
        margin: 2.5rem 1rem 1rem 1rem;
        display: grid;
        grid-template-columns: 50% 50%;
        .titulo{
          grid-column-start: 1;
          grid-column-end: 3;
          font-size: 1.8rem;
          width: 22rem;
        }
        .texto_corrido_inicial{
          margin-top: 2rem;
          width: 21rem;
        }
        .texto_plus_rosa{
          margin-top: 1rem;
          width: 20rem;
          color: #EC695E;
          font-style: oblique;
        }
        .text_relative{
          position: relative;
          .texto_lateral_index{
          position: absolute;
          display: flex;
          flex-direction: column;
          align-items: flex-end;
          bottom: -15rem;
          right: .001rem;
          .titulo_text_l{
            margin: 0;
            padding: 0;
            font-size: 1.2rem;
            font-weight: bold;
          }
          .text_l{
            text-align: right;
            width: 20rem;
          }
          .arrow{
            color: #EC695E;
            width: 1.5rem;
            .iconify{
              width: 100%;
              height: 100%;
            }
          }
        }
        }
        .imgs{
          position: relative;
          .img_filmin{
            position: absolute;
            top: 9rem;
            right: 0rem;
            width: 15rem;
            img{
              width: 100%;
              height: 100%;
              object-fit: cover;
              object-position: center;
            }
          }
          .text_filmin{
            position: absolute;
            top: 24.5rem;
            left: -10rem;
            .title_filmin{
              color: #066772;
              font-size: 1.1rem;

          }
            .texto{
              width: 9rem;
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
        .imgs_2{
          position: relative;
        .img_filmin{
          position: absolute;
          top: 33rem;
          left: 0rem;
          width: 10rem;
          img{
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: center;
          }
        }
        .text_filmin{
          position: absolute;
          top: 36rem;
          left: 10.5rem;
          .title_filmin{
          color: #066772;
          font-size: 1.1rem;

          }
          .texto{
            width: 10rem;
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
        .contact{
          position: absolute;
          top: 52rem;
          left: 10.5rem;
          color: #EC695E;
            .leer_mas_nuxt{
              position: relative;
              color: #EC695E;
              .iconify{
                position: absolute;
                top: .2rem;
                left: 4rem;
              }
              &:hover{
                color: #066772;
              }
            }
        } 
      }
      }
    
  }
</style>
