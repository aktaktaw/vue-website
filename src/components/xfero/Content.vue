<template>
  <div class="container">
    <div class="bg-intro">
      <Particle/>
      <div class="stack-icon">
        <h1 class="title">Our Stacks</h1>
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
    <div class="web-dev">
      <div class="row">
        <div class="col">
          <div class="content">
            <h3>Project 1</h3>
            <img src="@/assets/nodejs-icon.svg" class="icon" alt="Nodejs" style="width:100%">
          </div>
        </div>  
      </div>
    </div>
    <div class="mobile-dev">
      <h1>Mobile Development</h1>
    </div>
    <div class="iot">
      <h1>Internet of Things</h1>
    </div>
    <Footer/>
  </div>
</template>

<script>
import Particle from '@/components/xfero/Particle'
import Footer from '@/components/xfero/Footer'
export default {
  name:"Content",
  components:{
    Footer,
    Particle
  }
}
</script>

<style scoped>
.col{
  float: left;
  width: 25%;
}

.row{
  margin: 8px -15px;
}

.row,
.row > .col{
  padding: 8px;
}

.row:after{
  content: "";
  display: table;
  clear: both;
}

@media screen and(max-width: 600px){
  .col{
    width:100%;
    display: block;
    margin-bottom: 20px;
  }
}

.content{
  align-items: center;
  padding:10px;
}
.web-dev{
  max-width: 100vw;
  background-color: white;
  margin: auto;
  box-sizing: border-box;
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
  top: 20%; 
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

img:hover{
  transform:scale(1.2);
}

</style>