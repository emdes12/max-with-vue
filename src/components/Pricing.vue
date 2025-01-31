<script setup>
import PricingCard from "./cards/PricingCard.vue";
</script>

<template>
    <div class="container">
        <PricingCard head="Value Proposition Map" txt="A structured representation of your product’s value proposition. Ideal for internal sharing and collaboration with marketing agencies for a unified understanding and approach."/>
        <PricingCard head="Landing Page Prototypes" txt="Ready-to-implement prototypes tailored to your product, ensuring you hit the ground running with your campaigns."/>
        <PricingCard head="Advertisements" txt="Engaging visual and textual ads designed to capture attention across various online platforms, ensuring consistent messaging and brand presence."/>
    </div>
</template>

<style scoped>
.container {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    align-items: center;
    justify-content: space-between;
}
</style>