<template>
  <div class="container_body">
    <Title class="titulo" :titleprop="title"> </Title>
    <div class="contactos">
      <div class="num">
        <span class="iconify" data-icon="carbon:phone-filled" data-inline="false"></span>
        <div class="texti">+34 722 702 180</div>
      </div>
      <div class="email">
        <span class="iconify" data-icon="clarity:email-solid" data-inline="false"></span>
        <div class="texti">christianvalenciaglez@gmail.com</div>
      </div>
    </div>
    <div class="img_marca" data-aos="fade-up" data-aos-duration="2000">
      <img src="/MARCANAME.png" alt="" />
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
      title: '<span class="pink">Contacto</span>',
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
  .contactos{
    grid-column-start: 1;
    grid-column-end: 3;
    margin-left: 10rem;
    margin-top: 5rem;
    .num{
      margin-bottom: 1.5rem;
      font-size: 1.25rem;
      display: flex;
      .iconify{
        font-size: 1.75rem;
        margin-right: 1rem;
      }
    }
    .email{
      margin-bottom: 1.5rem;
      font-size: 1.25rem;
      display: flex;
      .iconify{
        font-size: 1.75rem;
        margin-right: 1rem;
      }
    }
  }
  .img_marca{
    margin-top: 5rem;
    margin-left: -13rem;
    display: flex;
    justify-content: center;
    align-items: center;
    grid-column-start: 2;
    grid-column-end: 3;
    width: 25rem;
    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: center;
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
  }
  .contactos{
    grid-column-start: 1;
    grid-column-end: 3;
    margin-left: 0rem;
    margin-top: 5rem;
    .num{
      margin-bottom: 1.5rem;
      font-size: 1rem;
      display: flex;
      .iconify{
        font-size: 1.5rem;
        margin-right: 1rem;
      }
    }
    .email{
      margin-bottom: 1.5rem;
      font-size: 1rem;
      display: flex;
      .iconify{
        font-size: 1.5rem;
        margin-right: 1rem;
      }
    }
  }
  .img_marca{
    margin-top: 5rem;
    margin-left: -7.5rem;
    display: flex;
    justify-content: center;
    align-items: center;
    grid-column-start: 2;
    grid-column-end: 3;
    width: 15rem;
    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: center;
    }
  }
}
}
</style>