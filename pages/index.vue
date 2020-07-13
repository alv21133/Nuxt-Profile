<template>
  <div>
    <navbar />
    <div class="centainer mt-5">
      <Logo />
      <h5 class="title text-dark">
        yudibest-profile
      </h5>
    </div>
    <div class="wave">
      <img src="~/assets/wave2.svg" alt="wait.." class="mt-3" />
    </div>
  </div>
</template>
<script>
export default {
  id: 'index',
  data: () => ({
    select: 'default',
  }),
}
</script>
<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  justify-content: center;
  align-items: center;
  text-align: center;
}

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
  margin-top: auto;
}
</style>
