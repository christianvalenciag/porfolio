<template>
  <div class="container_body">
    <Title class="titulo" :titleprop="title"> </Title>
    <div class="texto_corrido_inicial">
      Soy Gallego, tengo 22 años y estoy en tercero de carrera de Diseño Gráfico
      en la Escuela Superior de Diseño de Madrid (ESDM).
    </div>
    <div class="img_sobre_mi">
      <img src="/cv.jpg" alt="" />
    </div>
    <div class="texto_corrido_foto">
      <div class="subtitle">¿Qué puedo aportar?</div><br />
      Como estudiante mi experiencia no es muy amplia pero mi interés por el
      mundo UI y Product Design hace que invierta tiempo en esta disciplina y
      mucho empeño
      <br /><br />
      <span class="blue">Cuento con amplios conocimientos de prototipado, así como de
      herramientas para llevarlo a cabo, como pueden ser Figma o ProtoPie, este
      último para las animaciones</span>
      <br /><br />
      Gracias a mis competencias programando, estoy
      familiarizado con los lenguajes HTML, CSS, JS, PHP y también con el manejo
      de WordPress. Así pues, entiendo cómo el BackEnd se enfrenta a nuestros
      diseños y soy consciente de la dificultad que ciertos diseños tienen,
      desde el punto de vista de producción.
      <br /><br />
      Me gusta saber que somos capaces
      de, en un mundo totalmente digitalizado, aportar lo imprescindible para
      que los usuarios se sientan cómodos con el mundo digital y contribuir a
      que sus experiencias sean más agradables.
      <br /><br />
      <span class="blue">Soy una persona con una gran
      interés por aprender y crecer en el ámbito.</span>
      <br /><br />
      <div class="contact">
          <NuxtLink class="leer_mas_nuxt" to="contacto">Contacto<span class="iconify" data-icon="akar-icons:circle-plus" data-inline="false"></span> </NuxtLink>
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
        'Sobre mi,<br /> <span class="blue">Christian Valencia</span>, un diseñador <span class="pink">gráfico & UX UI</span>.',
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
    margin-top: 2rem;
    width: 30rem;
  }
  .img_sobre_mi{
    margin-top: 2rem;
    width: 100%;
    img{
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: center;
    }
  }
  .texto_corrido_foto{
    margin-top: 3rem;
    margin-left: 2.5rem;
    width: 80%;
    .subtitle{
      font-size: 1.35rem;
      font-weight: bold;
    }
    .blue{
      font-weight: bold;
    }
    .contact{
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
@media screen and (max-width: 800px) {
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
        width: 30rem;
      }
      .img_sobre_mi{
        
        margin-top: 2rem;
        width: 100%;
        img{
          width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;
        }
      }
      .texto_corrido_foto{
        
        margin-top: 3rem;
        margin-left: 1rem;
        width: 90%;
        .subtitle{
          font-size: 1.35rem;
          font-weight: bold;
        }
        .blue{
          font-weight: bold;
        }
        .contact{
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
@media screen and (max-width: 700px) {
    .container_body {
    margin: 2.5rem 1rem 1rem 1rem;
    display: grid;
    grid-template-columns: 50% 50%;
      .titulo {
        grid-column-start: 1;
        grid-column-end: 3;
        font-size: 2rem;
          width: 100%;
      }
      .texto_corrido_inicial {
        grid-column-start: 1;
        grid-column-end: 3;
        margin-top: 2rem;
        width: 100%;
      }
      .img_sobre_mi{
        grid-column-start: 1;
        grid-column-end: 3;
        margin-top: 2rem;
        width: 100%;
        img{
          width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: center;
        }
      }
      .texto_corrido_foto{
        grid-column-start: 1;
        grid-column-end: 3;
        margin-top: 3rem;
        margin-left: 0rem;
        width: 100%;
        .subtitle{
          font-size: 1.35rem;
          font-weight: bold;
        }
        .blue{
          font-weight: bold;
        }
        .contact{
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