<template>
  <div>
    <p v-if="signup.error.length">
      <b v-for="e in signup.error" v-bind:key="e.id">{{ e }} <br /></b>
    </p>
    <form @submit="login">
      <input
        type="text"
        placeholder="enter your name"
        v-model="signup.username"
      />
      <br /><br />
      <input
        type="password"
        placeholder="enter the password"
        v-model="signup.password"
      />
      <br /><br />
      <button type="submit">submit</button>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      signup: {
        error: [],
        username: null,
        password: null,
      },
    };
  },
  methods: {
    // signupUser() {
    //   console.warn(this.signup);
    // },
    login(e) {
      //   this.signup.error = [];
      if (this.signup.username && this.signup.password) {
        console.warn("no errors");
      }
      if (!this.signup.username) {
        this.signup.error.push("enter the user name");
        // console.warn("no username");
      }
      if (!this.signup.password) {
        this.signup.error.push("please enter password");
        // console.warn("no password");
      }
      console.warn("errors", this.signup.error);
      e.preventDefault();
    },
  },
};
</script>