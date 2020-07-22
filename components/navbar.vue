<template>
  <b-navbar toggleable="lg" type="light">
    <b-navbar-brand href="#" class="text-dark">yudibest</b-navbar-brand>

    <b-navbar-toggle target="nav-collapse" class="text-dark"
      >Moblie</b-navbar-toggle
    >
    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item href="#"></b-nav-item>
      </b-navbar-nav>
      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <b-nav-item class="text-light">Experience</b-nav-item>
        <b-nav-item>About</b-nav-item>
        <b-nav-item-dropdown text="koko" right>
          <b-dropdown-item href="#">EN</b-dropdown-item>
          <b-dropdown-item href="#">ES</b-dropdown-item>
          <b-dropdown-item href="#">RU</b-dropdown-item>
          <b-dropdown-item href="#">FA</b-dropdown-item>
        </b-nav-item-dropdown>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>

<script>
export default {
  id: 'navbar',
}
</script>

<style scoped>
.navbar-inner {
  background: transparent;
}
</style>
