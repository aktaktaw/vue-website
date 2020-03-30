<template>
  <div class="container">
    <div class="bg-intro">
      <Particle/>
      <div class="stack-icon">
        <h1>Our Stacks</h1>
          <br/>
          <div class="icon-list">
            <img src="@/assets/nodejs-icon.svg" class="icon" alt="">
            <img src="@/assets/react.svg" class="icon" alt="">
            <img src="@/assets/vue-9.svg" class="icon" alt="">
            <img src="@/assets/docker-1.svg" class="icon-md" alt="">
            <img src="@/assets/postgresql.svg" class="icon" alt="">
            <img src="@/assets/mongodb.svg" class="icon-md" alt="">
            <img src="@/assets/rabbitmq.svg" class="icon" alt="">  
          </div>
      </div>
    </div>
    <br/>
    <section>
      <h1 class="sub-title">Web Developments</h1>
      <div class="web-dev-container">
        
        <div>
            <h3>Project 1</h3>
            <img class="mobile-mockup" src="@/assets/iphone.jpg" alt="">
          </div>
          <div>
            <h3>Project 1</h3>
            <img class="mobile-mockup" src="@/assets/iphone.jpg" alt="">
          </div>
          <div>
            <h3>Project 1</h3>
            <img class="mobile-mockup" src="@/assets/iphone.jpg" alt="">
          </div>  
          <div>
            <h3>Project 1</h3>
            <img class="mobile-mockup" src="@/assets/iphone.jpg" alt="">
          </div>  
      </div>
    </section>
    <br>
    <section>
      <h1 class="sub-title">Mobile Developments</h1>
      <div class="mobile-dev-container">
        
        <div>
            <h3>Project 1</h3>
            <img class="mobile-mockup" src="@/assets/projects/project1.png" alt="">
          </div>
          <div>
            <h3>Project 1</h3>
            <img class="mobile-mockup" src="@/assets/projects/project1.png" alt="">
          </div>
          <div>
            <h3>Project 1</h3>
            <img class="mobile-mockup" src="@/assets/projects/project1.png" alt="">
          </div>
          <div>
            <h3>Project 1</h3>
            <img class="mobile-mockup" src="@/assets/projects/project1.png" alt="">
          </div>  
      </div>
    </section>
    <br>
    <section>
      <h1 class="sub-title">IOT Developments</h1>
      <div class="iot-container">   
        <div>
            <h3>Project 1</h3>
          </div> 
      </div>
    </section>
    <footer>
      All Rights Reserved &copy; {{new Date().getFullYear()}}
    </footer>
  </div>
</template>

<script>
import Particle from '@/components/xfero/Particle'
//import VueCoreVideoPlayer from 'vue-core-video-player';

export default {
  name:"Content",
  components:{
    Particle,
    //VueCoreVideoPlayer
  }
}
</script>

<style scoped>
footer{
    position: absolute;
    height:2.5rem;
    right: 0;
    bottom: 0;
    left: 0;
    padding: 1rem;
    background-color: #333;
    color: white;
    text-align: center;
    font-size: small;
}

.sub-title{
  padding-top: 20px;
  padding-bottom: 20px;
  text-align: center;
  font-size: 2em;
  font-weight: 80;
  background-color: #1eafe5;
}

.web-dev-container,
.mobile-dev-container,
.iot-container{
  max-width: 100vw;
  max-height: 30vh;
  background-color: white;
  margin: auto;
  display:grid;
  grid-template-columns: auto auto auto auto;
  padding: 100px;
  padding-bottom: 200px;
}

.web-dev-container>div,
.mobile-dev-container >div,
.iot-container>div{
  background-color: white;
  text-align: center;
  font-size: 30px;
}

.container{
  position: relative;
  min-height: 50vh;
}

h1{
  font-size: 80px;
  /*position: absolute;*/
}
.bg-intro{
  background-color:#1eafe5;
  height: 50%;
  background-size: cover;
  padding-top: 10rem;
  padding-bottom: 10rem;
  overflow: hidden;
}

.icon{
  width: 50px;
  height: 50px;
}

.mobile-mockup{
  width: 300px;
  height: 300px;
}

.icon-md{
  width: 120px;
  height: 50px;
}

.icon-list{
    background-color: whitesmoke;
    min-height: 10vh;
    box-shadow: 5px 10px 20px #333;
    border: 1px solid;
    border-radius: 50px;
    padding-top: 10px;
    
}

.stack-icon{
  position: absolute;
  z-index: 10;
  top: 10%; 
  left: 20%;
  right: 20%;
  text-align: center;
  text-transform: uppercase;
  color: white;
  z-index: 999;

}

.stack-icon img{
  padding: 20px 20px;
  transition: transform .2s;
}

.icon:hover, .icon-md:hover{
  transform:scale(1.2);
}

</style>