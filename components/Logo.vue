<template>
  <div>
    <div class="text-center">
      <b-img
        width="200"
        height="200"
        src="~/assets/images/my.jpg"
        rounded="circle"
        alt="Circle image"
        class="NuxtLogo"
      ></b-img>
    </div>
  </div>
</template>

<style>
.NuxtLogo {
  animation: 1s appear;
  margin: auto;
  z-index: 15;
}

@keyframes appear {
  0% {
    opacity: 0;
  }
}
</style>
