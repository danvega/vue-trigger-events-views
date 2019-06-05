<template>
  <div id="app">
    <router-view @updateStatus="updateStatus" class="content"/>
    <the-footer :status="status"/>
  </div>
</template>

<script>
import TheFooter from "./components/TheFooter";

export default {
  name: "App",
  components: {
    TheFooter
  },
  data() {
    return {
      status: "This is the default status message"
    };
  },
  methods: {
    updateStatus(status) {
      this.status = status;
    }
  }
};
</script>

<style>
body {
  margin: 0;
  padding: 0;
}
#app {
  height: 100vh;
  width: 100vw;
}
.content {
  padding: 10px;
}
h1 {
  font-size: 1.3em;
  text-transform: uppercase;
}
</style>
