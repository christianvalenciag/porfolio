<template>
   
     <h2 class="title_class" v-html="titleprop"></h2>
  
</template>

<script>

export default {
    props: ["titleprop"]
}
</script>

<style lang="scss">
.title_class{
    margin: 0;
    font-size: 3rem;
    color: black;
    width: 40rem;
    /* .azul{

    }
    .pink{

    } */
}

.pink{
  color: #EC695E;
}
.blue{
  color: #066772;
}


</style>