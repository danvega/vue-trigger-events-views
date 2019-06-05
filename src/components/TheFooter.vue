<template>
  <div class="footer">
    <p>{{ status }}</p>
  </div>
</template>

<script>
export default {
  name: "the-footer",
  props: {
    status: String
  }
};
</script>

<style scoped>
.footer {
  background-color: lightgray;
  padding: 10px;
}
p {
  font-size: 1em;
  font-style: italic;
}
</style>
