<template>
  <div class="home">
    <h1>Hello</h1>
    <h1 v-if="graduated">{{ student }}</h1>
    <h1 v-else>"They didn't graduate"</h1>
    <!-- only displays the info conditionally -->
    <!-- Used normally for a login and logout button-->
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "Home",
  components: {},
  data() {
    return {
      student: "Harry",
      graduated: true,
    };
  },
};
</script>
<style scoped>
h1 {
  color: red;
}
</style>
