<template>
  <div class="home">
    <header>
      <router-link to="/">
        <img src="@/assets/xfero.svg" alt="">
      </router-link>    
    </header>
    <Slide/>
  </div>
</template>

<script>
// @ is an alias to /src
import Slide from '@/components/Slide'

export default {
  name: 'Home',
  components: {
    Slide
  }
}
</script>

<style scoped>
img{
  padding-top: 10px;
  padding-bottom: 10px;
  max-height: 7vh;
}
header{
  text-align: center;
  background-color: #222;
  color:#fff;
  padding: auto;
}

h2{
    position: relative;
    margin: 0 auto;
    text-transform: uppercase;    
    font-weight: 500;
    font-size: 2vw;
}
</style>
