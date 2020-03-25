<template>
  <div class="container">
    <div class="bg-intro">
      <div class="stack-icon">
        <Particle/>
        <h1>Our Stacks</h1>
        <br/>
        <img src="@/assets/nodejs-icon.svg" class="icon" alt="">
        <img src="@/assets/react.svg" class="icon" alt="">
        <img src="@/assets/vue-9.svg" class="icon" alt="">
        <img src="@/assets/docker-1.svg" class="icon-md" alt="">
        <img src="@/assets/postgresql.svg" class="icon" alt="">
        <img src="@/assets/mongodb.svg" class="icon-md" alt="">
        <img src="@/assets/rabbitmq.svg" class="icon" alt="">
      </div>
    </div>
    <div class="web-dev">
      <h1>Web Development</h1>
    </div>
    <div class="mobile-dev">
      <h1>Mobile Development</h1>
    </div>
    <div class="iot">
      <h1>Internet of Things</h1>
    </div>
  </div>
</template>

<script>
import Particle from '@/components/Particle'

export default {
  name:"Content",
  components:{
    Particle
  }
}
</script>

<style scoped>
h1{
  font-size: 100px;
}
.bg-intro{
  background-color:#1FAFe5;;
  height: 80%;
  background-size: cover;
  position: relative;
  padding-top: 10rem;
  padding-bottom: 10rem;
}

.icon{
  width: 50px;
  height: 50px;
}

.icon-md{
  width: 120px;
  height: 50px;
}

.stack-icon{
  text-align: center;
  color: rgb(9, 41, 53);

}

.stack-icon img{
  padding: 0 20px;
}


</style>