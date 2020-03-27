<template>
  <div class="container">
      <Header/>
      <Content/>
  </div>
</template>

<script>
import Header from '@/components/xfero/Header'
import Content from '@/components/xfero/Content'

export default {
  name: 'Home',
  components: {
    Header,
    Content,
  }

}
</script>

<style>

</style>