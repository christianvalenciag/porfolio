<template>
  <div>
    <div class="header">
      <div class="arrow_div" 
      
      @click="$router.go(-1)">
          <span v-if="$nuxt.$route.path!='/'" class="iconify" data-icon="dashicons:arrow-left-alt2" data-inline="false"></span>
      </div>
      <div class="marca"><img src="/MARCA.PNG" alt="logo" /></div>
      <div class="menu_icon" @click="openmenu">
          <span class="iconify" data-icon="gg:menu-right" data-inline="false"></span>
      </div>
    </div>
    <div class="menu"  :class="isOpen ? 'menu_open' : ''">
      <div class="exit" @click="closemenu"><span class="iconify" data-icon="maki:cross-11" data-inline="false"></span></div>
      <div class="item_menu" @click="closemenu"><li><NuxtLink to="/">UX / UI</NuxtLink></li></div>
      <div class="item_menu" @click="closemenu"><li><NuxtLink to="d_grafico">DISEÑO GRÁFICO</NuxtLink></li></div>
      <div class="item_menu" @click="closemenu"><li><NuxtLink to="sobre_mi">SOBRE MI</NuxtLink></li></div>
      <div class="item_menu" @click="closemenu"><li><NuxtLink to="contacto">CONTACTO</NuxtLink></li></div>
    </div>
  </div>

  <!-- <nav>
        <ul>
            <li><NuxtLink to="/">PAGINA 1</NuxtLink></li>
            <li><NuxtLink to="/page2">PAGINA 2</NuxtLink></li>
            <li><NuxtLink to="/page3">PAGINA 3</NuxtLink></li>
        </ul>
    </nav> -->
</template>

<script>
export default {
  data(){
    return {
        isOpen: false,
      }
    
  },

  methods: {
    openmenu(){
      this.isOpen = !this.isOpen;
    },
    closemenu(){
      this.isOpen = !this.isOpen;
    }
  }

};
</script>

<style lang="scss">
.header {
  padding: 2.5rem 2rem;
  display: flex;
  justify-content: space-between;
  .arrow_div{
    width: 1.5rem;
    .iconify{
      width: 100%;
      height: 100%;
    }
  }
  .marca {
    width: 3rem;
    height: 3rem;
    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: center;
    }
  }
  .menu_icon{
    width: 1.5rem;
    .iconify{
      width: 100%;
      height: 100%;
    }
  }
}
.menu {
    visibility: hidden;
    z-index: 1;
    position: absolute;
    top: -.00005rem;
    background: rgba(1, 122, 136, 0.616);
    backdrop-filter: blur(15px); // Como hacer un blur con nuxt y que lo pillen los navegadores
    height: 100%;
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    color: white;
    font-family: Arial, Helvetica, sans-serif;
    font-weight: bold;
    padding: 6rem 0;

    &.menu_open{
      visibility: visible;
    }
    .exit{
        margin-bottom: 8.25rem ;
        width: 1.5rem;
        .iconify{
          font-size: 3rem;
          width: 100%;
          height: 100%;
        }
    }
    .item_menu {
        padding: 2rem;
        li{
          a{
             color: white;
          }
        }
      }
}
@media screen and (max-width: 600px){
  .header {
     padding: 2.5rem 1rem 1.5rem 1rem;
     .arrow_div{
          width: 1.2rem;
          .iconify{
            width: 100%;
            height: 100%;
          }
        }
     .menu_icon{
       width: 1.2rem;
        .iconify{
          width: 100%;
          height: 100%;
        }
      }
  }
}
</style>
