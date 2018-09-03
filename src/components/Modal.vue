<template>
  <div>
    <nav class="panel">
      <a class="panel-block" v-on:click="show = true">
        {{ title }}
      </a>
      <div v-bind:class="{ 'modal': true, 'is-active': show }">
        <div class="modal-background"></div>
        <div class="modal-card">
          <header class="modal-card-head">
            <p class="modal-card-title" style="word-wrap: break-word; flex-shrink: 1;">{{ title }}</p>
            <button class="delete" aria-label="close" v-on:click="show = false"></button>
          </header>
          <section class="modal-card-body">
            <div class="content">
              <slot />
            </div>
          </section>
          <footer class="modal-card-foot">
            <button class="button is-success" v-on:click="show = false">Close</button>
          </footer>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  props: ['title'],
  data() {
    return {
      show: false,
    };
  },

  created() {
    if (process.browser) {
      document.addEventListener('keyup', this.close);
    }
  },

  methods: {
    close(e) {
      if (e.keyCode === 27) {
        this.show = false;
      }
    },
  },
};
</script>
