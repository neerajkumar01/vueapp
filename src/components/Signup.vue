<template>
  <div class="">
    <input type="text" placeholder="enter your name" />
    <br /><br />
    <input type="password" placeholder="enter the password" />

    <br /><br />

    <input type="checkbox" name="hobby" id="cricket" />
    <label for="cricket">cricket</label>
    <input type="checkbox" name="hobby" id="sketing" />
    <label for="sketing">sketing</label>

    <br /><br />

    <input type="radio" name="gender" id="male" value="male" />male
    <input type="radio" name="gender" id="female" value="female" />female
  </div>
</template>

<script>
export default {
  name: "Signup",
};
</script>