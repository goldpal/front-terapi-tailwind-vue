<template>
  <navbar></navbar>
  <router-view />
</template>

<script>
import Navbar from "@/components/Navbar.vue";
export default {
  name: "Wrapper",
  components: { Navbar },
};
</script>

<style></style>
