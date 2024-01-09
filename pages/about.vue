<template>
  This is about page 
</template>

<script>
export default {
  mounted() {
    window.addEventListener("wheel", this.handleWheelEvent);
  },
  beforeUnmount() {
    window.removeEventListener("wheel", this.handleWheelEvent);
  },
  methods: {
    handleWheelEvent(event) {
      // Check if scrolling down (positive deltaY value)
      if (event.deltaY > 0) {
        this.$router.push("/connect");
      } 
    },
  },
};
</script>