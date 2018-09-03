<template>
  <section class="hero">
    <div class="hero-body">
      <div class="container">
        <div class="columns">
          <div class="column is-two-thirds">
            <h1 class="title">
              Support Fremont Homeowner's Movement Against Increased FUSD Developer Fees
            </h1>
            <hr>
            <h2 class="subtitle is-4">
              Fremont Unified School District (FUSD) has increased the developer fees from $5.70 to $26.11 per square feet, within a span of 1 year.
            </h2>
            <h2 class="subtitle is-4 bold">
              These fees are applicable for existing home owners if you are adding 500 or more SQ. FT. to YOUR existing home.
            </h2>
            <h2 class="subtitle is-4">
              We need your help to remove the increase in developer fees for existing homeowners only, leaving the high fees for new residential builders. Please sign the petition, join the Google Group, and try to attend the events listed.
            </h2>
            <h2 class="subtitle is-4">
              <b><u>Public Hearing:</u></b> FUSD has posted notice of public hearing to regarding proposed adoption of developer fees for the year 2018. Any comments with respect to this need to be sent in writing by May 10th, 2018. Please send your comments to Raul Parungao (<u>rparungao@fremont.k12.ca.us</u>).
              <br>We have analyzed the SFNA report and have compiled few questions and concerns mentioned below.
              <br><b>Major concern</b> is: FUSD has done the calculation with an intent to bring the developer fees as high as possible, which is reflected in the SFNA report.
              <br>Please send your comments by May 10th, 2018 to have an impact on opposing these fees and to reduce the fees.
              <br>Refer to <a href="https://www.fremont.k12.ca.us/Page/216">Notice Public hearing</a>
              <br>Refer to <a href="https://www.fremont.k12.ca.us/cms/lib/CA01000848/Centricity/Domain/6/SFNA_Fremont_1718_Fn.pdf">2018 SFNA Report</a>
              <br><br>There is public hearing on May 11th 7:30 AM at the following location
              <br>4210 Technology Drive, Fremont, CA 94538
              <br>Please attend this meeting to oppose the level 2 developer fees for existing home owners doing addition
              <br>Note the meeting is early morning at 7:30 AM on May 11th.
            </h2>
            <h2 class="subtitle is-4 bold">
            </h2>
            <h2 class="subtitle is-6">
              If you have any questions, do not hesitate to post in the Google Group or contact us through the <a href="/contact">contact page</a>.
            </h2>

            <hr>

            <h2 class="subtitle is-4">
              2018 SFNA Report Questions and Concerns - <a href="/qanda" class="button is-link">View All</a>
            </h2>
            <nav class="panel">
              <Modal v-for="question in this.questions" :key="question.title" :title="question.title">
                <div v-html="question.description"></div>
              </Modal>
            </nav>
          </div>
          <div class="column is-one-quarter">
            <!-- <div class="title is-4">Upcoming Events</div>
            <div class="subtitle is-5">
              <for(event in input.events)>
                <br>
                <div class="title is-5 no-pad-bottom">${event.title}</div>
                <p class="no-pad-bottom is-size-7">
                  <br>
                  <strong>${event.description}</strong>
                  <br>
                  <br>
                  <strong>${event.date.format('l')}, ${event.date.calendar()}</strong>
                  <br>
                  ${event.location}
                  <br>
                  <br>
                  <a class="button is-primary is-small is-fullwidth" href="${event.link}" target="_blank">Add to Google Calendar</a>
                </p>
              </for>
            </div> -->
            <a href="https://groups.google.com/forum/#!forum/fremont-homeowners/join" target="_blank" class="button is-large is-success">
              Join the Google Group
            </a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import questions from '@/assets/data/questions';
import Modal from '@/components/Modal.vue';

export default {
  data() {
    return {
      questions,
    };
  },
  components: {
    Modal,
  },
};
</script>
