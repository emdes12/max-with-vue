<script setup>
import BigNPara from "./components/HeadNParagraph.vue";
import Header from "./components/Header.vue";
import HeroImage from "./assets/images/CleanShot 2023-12-14 at 21.56 1.png";
import AbsImg from "./assets/images/Ready to Elevate Your Marketing Game_.png";
import PrimaryButton from "./components/btn/PrimaryButton.vue";
import ArtBoard from "./components/ArtBoard.vue";
import HowItWorks from "./components/HowItWorks.vue";
import OutputList from "./components/OutputList.vue";
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

  <main class="container" id="about">
    <BigNPara
      head2="Iterative Marketing"
      head1="The Challenge of Today's"
      txt="In today’s fast-paced business environment, continuously crafting and refining value propositions, then iterating them into effective marketing collateral, becomes a relentless cycle."
    />
  </main>

  <section class="abs-works">
    <div class="container">
      <img class="img-abs" :src="AbsImg" alt="overlaping/overflowing text" />
      <BigNPara
        flD="column-reverse"
        head2="Works"
        id="how-it-work"
        head1="How It"
        txt="Rocketyzer’s AI-powered platform revolutionizes the creation of value propositions, blending consistency, efficiency, and compelling results. Dive into a methodologically sound approach that turns your insights into impactful marketing messages."
      />
    </div>
  </section>

  <section class="processes">
    <HowItWorks />
  </section>

  <main class="bg-color-2">
    <div class="container" id="outputs">
      <BigNPara
        head1="What You Get"
        head2="Iterative With Rocketyzer"
        txt="From structured value propositions to ready-to-use marketing collateral, Rocketyzer equips you with a comprehensive set of tools to elevate your marketing game."
      />
    </div>
    <div class="bg-color-2">
      <OutputList />
    </div>
  </main>

  <main id="why-us">
    <BigNPara head1="Why"
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

#about {
  padding-bottom: 287px;
}

section.abs-works {
  background: linear-gradient(180deg, #272b3f 0%, #0e0e0f 100%);
  height: 702px;
  padding-top: 287px;
  position: relative;
}

.img-abs {
  max-width: 800px;
  width: 100%;
  position: absolute;
  left: 50%;
  top: 0%;
  transform: translate(-50%, -50%);
}

.bg-color-2 {
  background-color: #0e0e0e;
}

.processes {
  background: #0e0e0f;
  width: 100%;
}
</style>
