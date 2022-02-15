<template>
  <div>
    <h1 v-if="show">HELLO FROM HOME component</h1>
    <h1 v-else>show this</h1>
    <h6 v-if="show">
      <button v-on:click="display">button</button>
    </h6>
    <h6 v-else:>
      <button v-on:click="display">this</button>
    </h6>
  </div>
</template>

<script>
export default {
  name: "Home",
  props: {},
  data() {
    return {
      show: true,
    };
  },
  methods: {
    display() {
      this.show = !this.show;
    },
  },
};
</script>
