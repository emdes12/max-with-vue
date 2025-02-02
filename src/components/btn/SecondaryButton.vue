<script setup>
defineProps({
  txt: {
    type: String,
    default: "Sec Button",
    required: true,
  },
  link: {
    type: String,
    required: true,
  },
});
</script>

<template>
  <a :href="link">
    <button>
      {{ txt }}
    </button>
  </a>
</template>

<style scoped>
button {
  border: 1px solid var(--vt-black);
  background-color: transparent;
  padding: 18px 25px;
  font-family: Inter;
  font-size: 16px;
  font-weight: 700;
  line-height: 16.96px;
  color: var(--vt-black);
  letter-spacing: -0.6399999856948853px;
  text-align: center;
  text-underline-position: from-font;
  border-radius: 32px;
  text-decoration-skip-ink: none;
  cursor: pointer;
  transition: all 0.3s ease-in-out;
}

button:hover {
  color: #CCF652;
  background-color: var(--vt-black);
  border: none;
}
</style>
