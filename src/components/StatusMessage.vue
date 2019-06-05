<template>
  <div class="update-status">
    <p>Please enter a message below to update the status message.</p>
    <input type="text" v-model="status">
    <button @click="$emit('updateStatus',status)">Update Status</button>
  </div>
</template>

<script>
export default {
  name: "status-message",
  data() {
    return {
      status: ""
    };
  }
};
</script>

<style scoped>
.update-status {
  background-color: rgb(141, 204, 141);
  padding: 10px;
}
input {
  font-size: 20px;
}
button {
  margin: 10px 0 0 10px;
}
</style>
