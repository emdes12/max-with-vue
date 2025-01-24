<script setup>
import PrimaryButton from "./btn/PrimaryButton.vue";
import NavBar from "./NavBar.vue";
import Logo from "../assets/icons/Link → logo-rocketyzer.svg.svg";
</script>

<template>
  <header>
    <div class="container">
      <a href="#">
        <img :src="Logo" alt="" />
      </a>

      <NavBar />
      <PrimaryButton txt="Get started free" link="#" />
    </div>
  </header>
</template>

<style scoped>
header {
  width: 100vw;
}

.container {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

@media (min-width: 1024px) {
}
</style>
