<template>
  <div>
    <section class="hero is-primary">
      <div class="hero-body">
        <div class="container has-text-centered">
          <h1 class="title">
            Contact Us
          </h1>
        </div>
      </div>
    </section>
    <section class="section">
      <div class="container">
        <form action="https://hooks.zapier.com/hooks/catch/2526061/rkscdk/" target="_blank" method="POST">
          <div class="field">
            <label class="label">Name*</label>
            <div class="control">
              <input name="name" class="input" type="text" placeholder="Your Name">
            </div>
          </div>

          <div class="field">
            <label class="label">Your Email*</label>
            <div class="control">
              <input name="email" class="input" type="email" placeholder="Your Email Address">
            </div>
          </div>

          <div class="field">
            <label class="label">Phone Number</label>
            <div class="control">
              <input name="phone" class="input" type="text" placeholder="Your Phone Number">
            </div>
          </div>

          <div class="field">
            <label class="label">Message*</label>
            <div class="control">
              <textarea name="message" class="textarea" placeholder="Your Message"></textarea>
            </div>
          </div>

          <div class="field">
            <div class="control">
              <button type="submit" class="button is-primary">Submit</button>
            </div>
          </div>
        </form>
      </div>
    </section>
  </div>
</template>

<script>
export default {
};
</script>
