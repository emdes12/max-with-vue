<script setup>
import OutputCard from "./cards/outputCard.vue";
</script>

<template>
    <div class="container">
        <OutputCard head="Value Proposition Map" txt="A structured representation of your product’s value proposition. Ideal for internal sharing and collaboration with marketing agencies for a unified understanding and approach."/>
        <OutputCard head="Landing Page Prototypes" txt="Ready-to-implement prototypes tailored to your product, ensuring you hit the ground running with your campaigns."/>
        <OutputCard head="Advertisements" txt="Engaging visual and textual ads designed to capture attention across various online platforms, ensuring consistent messaging and brand presence."/>
        <OutputCard head="Slide Deck Prototypes" txt="Engaging and compelling slide decks that articulate your product’s value, ready for presentations and pitches."/>
        <OutputCard head="Sales Pitches" txt="Crafted pitches that resonate, ensuring you capture attention and drive interest from the get-go."/>
        <OutputCard head="Hero Messages for A/B Test" txt="Multiple hero messages tailored for your landing pages' first screens. Test, iterate, and boost your conversions with compelling headlines."/>
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