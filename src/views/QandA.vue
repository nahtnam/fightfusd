<template>
  <div>
    <section class="hero">
      <div class="hero-body">
        <div class="container">
          <h1 class="title">
            2018 SFNA Report Questions and Concerns
          </h1>
          <h2 class="subtitle">
            Several questions and concerns with respect to 2018 SFNA report that need to be addressed by the FUSD Board.
          </h2>
        </div>
      </div>
    </section>
    <div v-for="question in this.questions" :key="question.title">
      <hr>
      <section class="section">
        <div class="container">
          <h1 class="title no-pad-bottom">{{ question.title }}</h1>
          <br>
          <h2 class="subtitle content" v-html="question.description">
          </h2>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
import questions from '@/assets/data/questions';

export default {
  data() {
    return {
      questions,
    };
  },
};
</script>
