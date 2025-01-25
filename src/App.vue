<script setup>
import BigNPara from "./components/HeadNParagraph.vue";
import Header from "./components/Header.vue";
import HeroImage from "./assets/images/CleanShot 2023-12-14 at 21.56 1.png";
import PrimaryButton from "./components/btn/PrimaryButton.vue"
import ArtBoard from "./components/ArtBoard.vue"
</script>

<template>
  <Header />

  <main class="container hero-section">
    <BigNPara
      head1="Turn Product Insights into"
      head2="Compelling Value Propositions"
      txt="Rocketyzer takes your product insights, adds a dash of magic, and voilà! You get irresistible value propositions and marketing collateral that truly resonate with customers."
    />

    <PrimaryButton txt="Begin the magic" link="#" />

    <img class="hero-img" :src="HeroImage" alt="dashboard-screenshot" />
  </main>

  <main class="container">
    <ArtBoard />
  </main>
</template>

<style scoped>
.hero-section {
  display: flex;
  gap: 45px;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.hero-img {
  width: 100%;
}
</style>
