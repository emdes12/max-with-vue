<script setup>
import HiwCard from "./cards/HiwCard.vue";
</script>

<template>
  <div class="contain">
    <main class="container">
      <HiwCard
        head="Your Insights"
        tag1="Input"
        txt="Provide details about your product, customers, and competitors."
      />
      <HiwCard
        head="Deep Drive"
        tag2="Analysis"
        txt="Our AI analyzes your inputs for optimal results."
      />
      <HiwCard
        head="Tailored Recommendation"
        tag3="Suggestions"
        txt="Benefit from suggestions to refine your messaging."
      />
      <HiwCard
        head="Final Delivery"
        tag4="Output"
        txt="Get value propositions & marketing collateral ready for action."
      />
    </main>

    <img src="../assets/icons/div.t396__artboard.svg" alt="atom-mask" />
  </div>
  <!-- <div class="icony-textt container">
    <div class="illustrations">
      <img src="../assets/images/Group_53.png.png" alt="left and top" /><img
        src="../assets/images/Group_62.svg.png"
        alt="middle and center"
      /><img
        src="../assets/images/Group_54.svg fill.png"
        alt="right and bottom"
      />
    </div>
    <div class="illustration-text">
      <div class="left">Your Input</div>
      <img src="../assets/icons/Arrow_3.svg.svg" />
      <div class="midcent">Rocketyzer's Magic</div>
      <img src="../assets/icons/Arrow_3.svg.svg" />
      <div class="botmright">Value Proportion & Maarketing Collateral</div>
    </div>
  </div> -->
</template>

<style scoped>
main {
  width: 100%;
  display: flex;
  align-items: center;
  gap: 20px;
  justify-content: space-between;
  flex-wrap: wrap;
}

img {
  width: 100%;
}

.contain {
  display: flex;
  flex-direction: column;
  gap: 30px;
  padding-bottom: 3rem;
}

/* .icony-textt {
  margin-top: 25px;
  padding: 30px;
  background: var(--vt-black);
} */

/* .illustrations {
  display: flex;
  align-items: center;
  width: 100%;
  justify-content: space-between;
}

.illustration-text {
  color: var(--vt-white);
  font-family: Inter;
  font-size: 26px;
  font-weight: 600;
  line-height: 29px;
  letter-spacing: -0.7799999713897705px;
  text-align: left;
  text-underline-position: from-font;
  text-decoration-skip-ink: none;
  display: flex;
  align-items: center;
  width: 100%;
  justify-content: space-between;
}

.left {
  text-align: left;
}

.midcent {
  text-align: center;
}

.botmright {
  text-align: right;
} */
</style>
