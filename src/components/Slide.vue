<template>
  <div class="container">
      <div class="landing left">
          <h1>
              <router-link to="/project">Developments</router-link>
          </h1>
      </div>
      <div class="landing right">
          <h1>
              <router-link to="/">Game Server</router-link>
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
h1 router-link{
    text-decoration: none;
    text-decoration-line: unset;
    color: #ffffff;
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
  background: #bf6654;
  box-shadow: 0 50vw 0 50vw rgba(0, 0, 0, 0);
}

.left:hover {
  flex-basis: 150%;
  background: saturate(#bf6654, 25);
  box-shadow: 0 50vw 0 50vw rgba(0, 0, 0, 0.7);
  color: rgb(255, 255, 255);
  z-index: 500;
}
.right {
  flex-basis: 50%;
  background: #3d7299;
  box-shadow: 0 -50vw 0 50vw rgba(0, 0, 0, 0);
}

.right:hover {
  flex-basis: 150%;
  background: saturate(#3d7299, 25);
  box-shadow: 0 -50vw 0 50vw rgba(0, 0, 0, 0.7);
  color: rgb(255, 255, 255);
  z-index: 500;
}
</style>
