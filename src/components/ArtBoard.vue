<script setup>
import ArtBoardCard from "./cards/ArtBoardCard.vue";
import RocketImgOne from "../assets/icons/icon-rocket-1.svg.svg"
import RocketImgTwo from "../assets/icons/icon-rocket-1.svg (1).svg"
import RocketImgThree from "../assets/icons/icon-rocket-1.svg (2).svg"
</script>

<template>
    <section>
        <ArtBoardCard head="Swift Idea Generation:" txt="Obtain ideas swiftly for compelling value propositions that articulate your product’s value clearly, ensuring your messaging resonates with your target audience." :cardIcon="RocketImgThree"/>
        <ArtBoardCard head="Rapid Marketing Iteration" txt="Test and iterate various marketing ideas rapidly. Optimize for higher conversions, ensure your messaging is strategically aligned, and drive more sales than ever before." :cardIcon="RocketImgTwo"/>
        <ArtBoardCard head="Boosted Conversions:" txt="With Rocketyzer, users have experienced an increase in conversions by 2 to 3 times. Transform your marketing efforts and see tangible growth." :cardIcon="RocketImgOne"/>
    </section>
</template>

<style scoped>
section {
    width: 100%;
    display: flex;
    align-items: center;
    gap: 30px;
    justify-content: space-between;
    flex-wrap: wrap;
}
</style>