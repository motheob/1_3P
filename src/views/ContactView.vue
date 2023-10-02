<template>
  <div class="contact-form">
    <h1>Get in touch!</h1>
    <p>You can reach me at:</p>
    <ul class="contact-info">
      <li>Email: mboikhutso@deakin.edu.au</li>
      <li>GitHub: <a href="https://github.com/motheob" target="_blank">motheob</a></li>
    </ul>

    <h2>Send Feedback</h2>
    <form @submit.prevent="submitFeedback">
      <label for="name">Name:</label>
      <input type="text" id="name" v-model="feedback.name" required>

      <label for="email">Email:</label>
      <input type="email" id="email" v-model="feedback.email" required>

      <label for="message">Message:</label>
      <textarea id="message" v-model="feedback.message" required></textarea>

      <Button @click="submitFeedback">Submit</Button>
    </form>

    <div v-if="feedbackSubmitted">
      <p>Thank you for your feedback!</p>
      <p>Your message:</p>
      <p>Name: {{ feedback.name }}</p>
      <p>Email: {{ feedback.email }}</p>
      <p>Message: {{ feedback.message }}</p>
    </div>
  </div>
</template>

<script>
import Button from '@/components/Button.vue'

export default {
  name: 'ContactView',
  components: {
    Button,
  },
  data() {
    return {
      email: 'mboikhutso@deakin.edu.au',
      github: 'https://www.github.com/motheob',
      feedback: {
        name: '',
        email: '',
        message: '',
      },
      feedbackSubmitted: false,
    };
  },
  methods: {
    submitFeedback() {
      this.feedbackSubmitted = true;
    },
  },
};
</script>

<style scoped>
.contact-info {
  list-style: none;
  padding: 0;
}

.contact-form {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
  text-align: center;
}

label {
  font-weight: bold;
  display: block;
}

input[type="text"],
input[type="email"],
textarea {
  width: 100%;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 3px;
}

button {
  background-color: #6e7e8d;
  color: #fafaf7;
  padding: 10px 20px;
  border: none;
  cursor: pointer;
  border-radius: 3px;
}
</style>