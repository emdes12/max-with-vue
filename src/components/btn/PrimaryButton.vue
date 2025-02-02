<script setup>
defineProps({
  txt: {
    type: String,
    default: "Pry Button",
    required: true,
  },
  link: {
    type: String,
    required: true,
  },
  widTH: {
    type: String,
    Default: "max-content",
  },
});
</script>

<template>
  <a :href="link">
    <button :style="'width: ' + widTH">
      {{ txt }}
    </button>
  </a>
</template>

<style scoped>
button {
  border: 1px solid var(--vt-white);
  background-color: transparent;
  padding: 18px 25px;
  font-family: Inter;
  font-size: 16px;
  font-weight: 700;
  line-height: 16.96px;
  color: var(--vt-white);
  letter-spacing: -0.6399999856948853px;
  text-align: center;
  text-underline-position: from-font;
  border-radius: 32px;
  text-decoration-skip-ink: none;
  cursor: pointer;
  transition: all 0.3s ease-in-out;
}

button:hover {
  color: var(--vt-black);
  background-image: linear-gradient(90deg, #45EFE5 0%, #CCF652 90%);
  border: none;
}
</style>
