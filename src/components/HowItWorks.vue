<script setup>
import HiwCard from "./cards/HiwCard.vue";
</script>

<template>
  <main>
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

  <div class="icony-textt"></div>
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

.icony-textt {
    margin-top: 25px;
    padding: 30px;
    background: var(--vt-black);
}
</style>
