<template>
  <nav class="navbar is-white has-shadow" id="main-navbar">
    <div class="container">
      <div class="navbar-brand">
        <router-link class="navbar-item has-text-weight-bold" to="/">
          <span class="is-size-5">Fight FUSD</span>
        </router-link>

        <div class="navbar-burger burger" :class="{ 'is-active': active }" @click="toggleMenu">
          <span></span>
          <span></span>
          <span></span>
        </div>
      </div>

      <div class="navbar-menu" :class="{ 'is-active': active }">
        <div class="navbar-end">
          <router-link to="/" class="navbar-item" active-class="is-active" @click.native="closeMenu" exact>Home</router-link>
          <router-link to="/multi-story" class="navbar-item" active-class="is-active" @click.native="closeMenu">Second Story Restriction</router-link>
          <router-link to="/qanda" class="navbar-item" active-class="is-active" @click.native="closeMenu">Q and A</router-link>
          <router-link to="/contact" class="navbar-item" active-class="is-active" @click.native="closeMenu">Contact</router-link>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Navigation',
  data() {
    return {
      active: false,
    };
  },
  methods: {
    closeMenu() {
      this.active = false;
    },
    toggleMenu() {
      this.active = !this.active;
    },
  },
};
</script>
