<template>
  <div>
    <app-navbar />
    <Nuxt />
  </div>
</template>
<script>
import AppNavbar from '../components/AppNavbar.vue'
export default {
  components: { AppNavbar }
}
</script>

<style lang="scss">

$ieee-orange: #FFA300;
$ieee-blue: #00629b;
$ieee-cyan: #00b5e2;
$ieee-black: #000000;
$ieee-white: #ffffff;
$ieee-grey: #75787b;
:root{
  font-family: 'Lexend Deca',sans-serif;
}

*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  text-decoration: none;
  list-style: none;
}
section{
  height: 100vh;
}
a:visited{
  color: $ieee-black;
}
a:hover{
  color:$ieee-black;
}
</style>
