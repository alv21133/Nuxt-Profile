<template>
  <div
    :class="{
      def: true,
      customColor: select === 'default',
      customColor2: select === 'custom',
    }"
  >
    <navbar />
    <div class="container">
      <Logo />
      <h1 class="title">
        yudibest-profile
      </h1>
    </div>
    <div class="text-center d-flex">
      <button @click="select = 'default'" class="btn btn-info ml-3">
        Original
      </button>
      <button @click="select = 'custom'" class="btn btn-info ml-2">
        Custom
      </button>
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
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #5a4a4a;
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
  background: rgb(255, 212, 179);
  background: linear-gradient(
    140deg,
    rgba(255, 212, 179, 1) 0%,
    rgba(255, 0, 9, 1) 100%
  );
}
</style>
