<template>
  <div class="container">
      <div class="landing left">
          <h1>
              <router-link class="nav" to="/xfero">Developments</router-link>
          </h1>
      </div>
      <div class="landing right">
          <h1>
              <router-link class="nav" to="/">Game Server</router-link>
          </h1>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>

.container{
    margin:0;
    display: flex;
    width: 100%;
    height: 100vh;
}

h1{
    position: relative;
    margin: 0 auto;
    text-transform: uppercase;    
    font-weight: 900;
    font-size: 2vw;
}

.nav{
    text-decoration: none;
    color: #ffffff;
    border-style: solid;
    border-color: white;
    padding: 30px;
}

h1:before {
  content: "";
  height: .3vw;
  width: 0;
  position: absolute;
  bottom: -.1vw;
  transition: 500ms all ease-in-out;
  left: 50%;
  transform: translateX(-50%);
}

.landing {
  display: flex;
  transition: 500ms all ease-in-out;
  z-index: 1;
  height: 100%;
  align-content: center;
  align-items: center;
}

.landing:hover > h1:before {
  width: 100%;
  background-color: #fff;
  opacity: 1;
}

.left {
  flex-basis: 50%;
  background: darkslategrey;
  box-shadow: 0 50vw 0 50vw rgba(0, 0, 0, 0);
}

.left:hover {
  flex-basis: 130%;
  background: saturate(#bf6654, 25);
  box-shadow: 0 50vw 0 50vw rgba(0, 0, 0, 0.5);
  color: rgb(255, 255, 255);
  z-index: 500;
}
.right {
  flex-basis: 50%;
  background: #3d7299;
  box-shadow: 0 -50vw 0 50vw rgba(0, 0, 0, 0);
}

.right:hover {
  flex-basis: 130%;
  background: saturate(#3d7299, 25);
  box-shadow: 0 50vw 0 50vw rgba(0, 0, 0, 0.5);
  color: rgb(255, 255, 255);
  z-index: 500;
}
</style>
