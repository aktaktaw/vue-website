<template>
  <div class="container">
      <Header/>
      <Content/>
      <Footer/>
  </div>
</template>

<script>
import Header from '@/components/xfero/Header'
import Content from '@/components/xfero/Content'
import Footer from '@/components/xfero/Footer'

export default {
  name: 'Home',
  components: {
    Header,
    Content,
    Footer
  }

}
</script>

<style>

</style>