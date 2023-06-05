<template>
  <MyNavbar></MyNavbar>
  <MyLanding></MyLanding>
  <MyProduct></MyProduct>
  <MyPlayLocation></MyPlayLocation>
  <MyFeatured></MyFeatured>
  <MyFooter></MyFooter>
</template>

<script>
import MyNavbar from './components/MyNavbar.vue'
import MyLanding from './components/MyLanding.vue'
import MyProduct from './components/MyProduct.vue'
import MyPlayLocation from './components/MyPlayLocation.vue'
import MyFeatured from './components/MyFeatured.vue'
import MyFooter from './components/MyFooter.vue'

export default {
  name: 'App',
  components: {
    MyNavbar,
    MyLanding,
    MyProduct,
    MyPlayLocation,
    MyFeatured,
    MyFooter
}
}
</script>

<style>
:root {
  --swiper-navigation-size: 24px;
  --swiper-navigation-color:#fff;
  --swiper-navigation-sides-offset: 10px;
}

#app {
  font-family: POSIS, Helvetica, Arial, sans-serif;
  text-align: center;
}

html, body {
  margin: 0;
}

section{
  width: 100%;
}

ul {
    list-style: none;
    padding: 0;
}

a {
  text-decoration: none;
  color: inherit;
}

p {
  font-size: 14px;
}

h3, p, h2, h4 {
  letter-spacing: 0.1rem;
}

img {
    width: 100%;
    height: auto;
}

* {
  box-sizing: border-box;
}
</style>
