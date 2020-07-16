<template>
  <div>
    <div class="text-left">
      <b-img
        width="200"
        height="200"
        src="~/assets/images/my.jpg"
        rounded="circle"
        alt="Circle image"
        class="NuxtLogo"
        @click="click1"
      ></b-img>
      <transition name="fadeDown">
        <b-card
          v-show="count == 1"
          title="Card title "
          sub-title="Card subtitle"
          class="rotate"
          border-variant="white"
        >
          <b-card-text>
            {{ count }}
          </b-card-text>
          <b-card-text>A second paragraph of text in the card.</b-card-text>

          <a href="#" class="card-link">Card link</a>
          <b-link href="#" class="card-link">Another link</b-link>
        </b-card>
      </transition>
      <transition name="fadeDown">
        <b-card
          v-show="count == 2"
          title="Card title "
          sub-title="Card subtitle"
          class="rotate"
          border-variant="white"
        >
          <b-card-text>
            {{ count }}
          </b-card-text>
          <b-card-text>A second paragraph of text in the card.</b-card-text>

          <a href="#" class="card-link">Card link</a>
          <b-link href="#" class="card-link">Another link</b-link>
        </b-card>
      </transition>
    </div>
  </div>
</template>
<script>
export default {
  data: () => ({
    count: 2,
  }),
  methods: {
    click1() {
      if (this.count === 1) {
        this.count = '(*&^*'
        setTimeout(() => {
          this.count = 2
        }, 200)
      } else {
        this.count = '(*&^*'
        setTimeout(() => {
          this.count = 1
        }, 200)
      }
    },
  },
}
</script>
<style>
.NuxtLogo {
  animation: 1s appear;
  margin: auto;
  z-index: 15;
  margin-top: 200px;
  margin-bottom: -200px;
}

@keyframes appear {
  0% {
    opacity: 0;
  }
}

.rotate {
  position: absolute;
  left: 210px;
  top: 290px;
}
</style>
