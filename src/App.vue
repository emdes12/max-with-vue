<script setup>
import BigNPara from "./components/HeadNParagraph.vue";
import Header from "./components/Header.vue";
import HeroImage from "./assets/images/CleanShot 2023-12-14 at 21.56 1.png";
import AbsImg from "./assets/images/Ready to Elevate Your Marketing Game_.png";
import PrimaryButton from "./components/btn/PrimaryButton.vue";
import ArtBoard from "./components/ArtBoard.vue";
import HowItWorks from "./components/HowItWorks.vue";
import OutputList from "./components/OutputList.vue";
import WhyUsBox from "./components/WhyUsBox.vue";
import Pricing from "./components/Pricing.vue";
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

  <main class="container overflow-below" id="about">
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
    <div class="why"></div>
    <div class="container">
      <BigNPara head1="Why Rocketyzer" head2="Stands Out" />
      <WhyUsBox />
    </div>
  </main>

  <main class="container overflow-below">
    <BigNPara
      flD2="column-reverse"
      head2="Secret Sauce"
      head1="The Value Proposition Toolkits"
      txt="While the digital landscape is flooded with automated copy generators, Rocketyzer stands apart. Our foundation is the proven methodology of the Value Proposition Toolkit."
    />
  </main>

  <section class="abs-works">
    <div class="container">
      <img class="img-abs" :src="AbsImg" alt="overlaping/overflowing text" />
      <BigNPara
        txt="Dive deep into a methodological approach that ensures every word aligns with your product’s core value, setting you apart in the market."
      />
    </div>
  </section>

    <main class="vprop">
      <div class="prop-value-desc container">
        <div class="details">
          <h4>
            The Value Proposition Toolkit is a carefully designed methodology
            that explores the nuances of product value, target customers, and
            market differentiation.
          </h4>
          <p>
            By integrating this toolkit, Rocketyzer ensures that every value
            proposition and piece of marketing collateral is rooted in a deep
            understanding of the product’s core value and its resonance with the
            target audience.
          </p>
        </div>
        <img
          src="./assets/images/Group_154.svg fill.png"
          alt="dialogue windows"
        />
      </div>
    </main>

    <main id="pricing">
      <div class="container">
        <BigNPara  head1="Pricing" head2="Plans" />

        <Pricing />
      </div>
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

.overflow-below {
  padding-bottom: 287px;
}

.vprop, #pricing {
  background: #0E0E0E;
  width: 100%;
  padding-bottom: 3rem;
}

.prop-value-desc {
  background: linear-gradient(180deg, rgba(39, 43, 63, 0.67) 0%, #383e5c 100%);
  border-radius: 12px;
  padding: 40px;
  display: flex;
  flex-wrap: wrap-reverse;
  width: 100%;
  align-items: center;
  justify-content: center;
}

.details {
  width: 340px;
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.details p {
  font-family: Inter;
  font-size: 16px;
  font-weight: 500;
  line-height: 22px;
  letter-spacing: -0.3199999928474426px;
  text-align: left;
  text-underline-position: from-font;
  text-decoration-skip-ink: none;
  color: #8c929e;
}

.details h4 {
  font-family: Inter;
  font-size: 32px;
  font-weight: 600;
  line-height: 38px;
  letter-spacing: -0.9599999785423279px;
  text-align: left;
  text-underline-position: from-font;
  text-decoration-skip-ink: none;
  color: var(--vt-white);
}

#why-us {
  position: relative;
}

#why-us .container {
  top: -40px;
}

.why {
  right: 0;
  background-image: linear-gradient(180deg, #0e0e0f 0%, #272b3f 100%);
  width: 100%;
  height: 207px;
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
