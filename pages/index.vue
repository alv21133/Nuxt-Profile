<template>
  <div>
    <navbar style="z-index: 100;" />
    <div class="parent">
      <!-- <vue-particles
        color="#001eff"
        :particleOpacity="1.7"
        :particlesNumber="20"
        shapeType="edge"
        :particleSize="4"
        linesColor="#001eff"
        :linesWidth="1"
        :lineLinked="true"
        :lineOpacity="1.4"
        :linesDistance="180"
        :moveSpeed="3"
        :hoverEffect="true"
        hoverMode="grab"
        :clickEffect="true"
        clickMode="push"
        class="particle"
      /> -->
      <div class="box">
        <Logo />
        <b-img
          class="triangle"
          src="~/assets/triangle6.png"
          fluid
          alt="Responsive image"
        ></b-img>
      </div>
    </div>

    <!-- <div class="wave">
      <img src="~/assets/wave1.svg" alt="wait.." class="mt-3" />
    </div> -->
  </div>
</template>
<script>
import Vue from 'vue'
import VueParticles from '~/node_modules/vue-particles'
Vue.use(VueParticles)

export default {
  id: 'index',
  data: () => ({
    select: 'default',
  }),
}
</script>
<style>
.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 50px;
  color: #292828;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  display: flex;
}

@keyframes color1 {
  from {
    top: 50%;
  }
  to {
    top: 0%;
    background: rgb(248, 226, 65);
    background: linear-gradient(
      149deg,
      rgba(248, 226, 65, 1) 0%,
      rgba(4, 252, 255, 1) 100%
    );
  }
}
.def {
  max-height: 1px;
}
.customColor {
  animation: color1 0s;
  animation-fill-mode: forwards;
  transition: ease-in 0.3s;
  max-height: 1200px;
}

.customColor2 {
  margin-top: -2px;
  min-height: 500px;
  background: rgb(255, 212, 179);
  background: linear-gradient(
    0deg,
    rgba(255, 212, 179, 0) 0%,
    rgba(80, 0, 202, 1) 100%
  );
}

.wave {
  z-index: 5;
}
.particle {
  position: absolute;
  width: 100%;
  z-index: -1;
}

.triangle {
  z-index: -100;
  position: relative;
  top: -260px;
}

.parent {
  display: grid;
  place-items: center;
}

.box {
  width: clamp(100%, 50%, 46ch);
  display: flex;
  flex-direction: column;
}
</style>
