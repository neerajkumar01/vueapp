<template>
  <div class="">
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

    <input type="checkbox" value="male" id="cricket" v-model="signup.hobbies" />
    <label for="cricket">cricket</label>
    <input
      type="checkbox"
      value="female"
      id="skating"
      v-model="signup.hobbies"
    />
    <label for="skating">skating</label>

    <br /><br />

    <input
      type="radio"
      name="gender"
      id="male"
      value="male"
      v-model="signup.gender"
    />male
    <input
      type="radio"
      name="gender"
      id="female"
      value="female"
      v-model="signup.gender"
    />female
    <br />
    <br />
    <button v-on:click="signupUser">submit</button>
  </div>
</template>

<script>
export default {
  name: "Signup",
  data() {
    return {
      signup: {
        username: null,
        password: null,
        hobbies: [],
        gender: null,
      },
    };
  },
  methods: {
    signupUser() {
      console.warn(this.signup);
    },
  },
};
</script>