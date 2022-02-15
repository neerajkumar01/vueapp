<template>
  <section>
    <h3>id name email</h3>
    <h4 v-for="user in users" v-bind:key="user.id">
      <p style="border: 1px black solid">
        {{ user.id }}&nbsp;{{ user.name }}&nbsp;{{ user.email }}
      </p>
    </h4>
  </section>
</template>

<script>
export default {
  name: "Fordirective",
  data() {
    return {
      users: [
        { id: 1, name: "aaa", email: "aaa@gmail.com" },
        { id: 2, name: "bbb", email: "bbb@gmail.com" },
        { id: 3, name: "ccc", email: "ccc@gmail.com" },
        { id: 4, name: "ddd", email: "ddd@gmail.com" },
      ],
    };
  },
};
</script>