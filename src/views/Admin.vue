<template>
  <div class="admin">
    <h1>Admin Page</h1>
    <p>Siphon white macchiato arabica frappuccino breve as, affogato that acerbic dark sweet. Qui brewed single shot white bar plunger pot single shot cinnamon. Lungo brewed turkish white aged skinny french press. Aged french press white medium, brewed and ut seasonal single origin. Single origin, aroma, robusta trifecta cup frappuccino cup skinny.</p>
    <p>Arabica and percolator blue mountain to go mug frappuccino white medium brewed single shot. Skinny redeye aromatic, java flavour mazagran blue mountain robusta milk. Trifecta single shot strong single origin caffeine cream cinnamon cream extra. Turkish, caramelization so, cultivar brewed, cream mocha plunger pot white robusta saucer. Caffeine dark, brewed carajillo pumpkin spice mocha caffeine.</p>

    <status-message @updateStatus="updateStatus"/>
  </div>
</template>

<script>
import StatusMessage from "@/components/StatusMessage.vue";

export default {
  name: "admin",
  components: {
    StatusMessage
  },
  data() {
    return {};
  },
  methods: {
    updateStatus(status) {
      this.$emit("updateStatus", status);
    }
  }
};
</script>

<style scoped>
</style>
