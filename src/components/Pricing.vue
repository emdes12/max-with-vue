<script setup>
import PricingCard from "./cards/PricingCard.vue";
const freeFeaturesArray = ['Step-by-step wizard guide', 'AI-Based Analysis and Recommendations']
const freeOutputArray = ['Value Proposition Statement']
const nine9FeatureArray = ['Step-by-step wizard guide', 'AI-Based Analysis and Recommendations']
const nine9OutputArray = ['Value Proposition Statement', 'Proposition Map', 'Copy for Landing Pages, SLide Decks, Sales Pitches, Ads.', 'Set of Hero Messages for A/B Testing']
const customFeatureArray = ['step-by-step wizard guide', 'AI-Supervised: Reviewed by a Professional Marketer and a Copywriter']
const customOutputArray = ['Value Proposition Statement', 'Proposition Map', 'Copy for Landing Pages, SLide Decks, Sales Pitches, Ads.', 'Set of Hero Messages for A/B Testing']
</script>

<template>
    <div class="container">
        <PricingCard cardName="Free" sub="per month" head="$0" txt="Perfect for individuals or startups looking for a quick value proposition." btnText="Get Started for Free" :outputArr="freeOutputArray" :featuredArr="freeFeaturesArray"/>
        <PricingCard cardName="Pro" sub="per month" head="$99" txt="For businesses that need comprehensive marketing collateral." btnText="Strat Free Trail" :featuredArr="nine9FeatureArray" :outputArr="nine9OutputArray"/>
        <PricingCard cardName="Custom" head="Custom" txt="The ultimate package with an added human touch for perfection." btnText="Contact us for a Custom Quote" :featuredArr="customFeatureArray" :outputArr="customOutputArray"/>
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