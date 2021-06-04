<template>
  <div class="container">
    <Header />
    <Nuxt />
  </div>
</template>

<style>
body {
    margin: 0;
    padding: 0;
    overflow-x: hidden;
    max-width: 1424px;
    
}
li {
    list-style: none;
}
a {
    text-decoration: none;
}
ul {
    margin: 0;
    padding: 0;
}
html {
  font-family:
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
/* .container{

  margin-bottom: 6rem;
} */
.container_body {
  margin: 2.5rem 6rem 6rem 6rem;
  padding-bottom: 6rem;
  display: grid;
  grid-template-columns: 50% 50%;
} 
</style>
