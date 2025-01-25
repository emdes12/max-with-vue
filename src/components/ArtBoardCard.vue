<script setup>
defineProps({
  head: {
    type: String,
    required: true,
  },
  cardIcon: {
    type: String,
    required: true,
  },
  txt: {
    type: String,
    required: true,
  },
});
</script>

<template>
  <div class="card">
    <div class="card-head">
      <h3>{{ head }}</h3>
      <img :src="cardIcon" alt="artboard cardIcon" />
    </div>
    <span>{{ txt }}</span>
  </div>
</template>

<style scoped>
.card {
  background: var(--vt-art-card-bg);
  padding: 30px;
  width: 384px;
  height: 258px;
  border-radius: 10px;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: space-between;
}

.card:hover {
    background-color: var(--vt-art-card-bg-hover);
}

.card-head {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  gap: 20px;
}

span {
  font-family: Inter;
  font-size: 16px;
  font-weight: 400;
  line-height: 24px;
  letter-spacing: -0.41999998688697815px;
  text-align: left;
  text-underline-position: from-font;
  text-decoration-skip-ink: none;
  color: var(--vt-light-bg-color);
}

h3 {
  font-family: Inter;
  font-size: 26px;
  font-weight: 600;
  line-height: 29px;
  letter-spacing: -0.7799999713897705px;
  text-align: left;
  text-underline-position: from-font;
  text-decoration-skip-ink: none;
  color: var(--vt-white);
}
</style>
