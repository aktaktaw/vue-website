<template>
  <div class="home">
    <header>
      <h2>Our Website</h2>
    </header>
    <Slide/>
    <footer>
      xfero.xyz copyright &copy; {{new Date().getFullYear()}}
    </footer>
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
header{
  text-align: center;
  background-color: #333;
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

footer {
    position: relative;
    right: 0;
    bottom: 0;
    left: 0;
    padding: 1rem;
    background-color: #333;
    color: white;
    text-align: center;
    font-size: x-small;
}
</style>
