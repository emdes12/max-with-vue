<script setup>
defineProps({
  head: {
    type: String,
    required: true,
  },
  tag1: {
    type: String,
    required: false,
  },
  tag2: {
    type: String,
    required: false,
  },
  tag3: {
    type: String,
    required: false,
  },
  tag4: {
    type: String,
    required: false,
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
      <p class="tag1">{{ tag1 }}</p>
      <p class="tag2">{{ tag2 }}</p>
      <p class="tag3">{{ tag3 }}</p>
      <p class="tag4">{{ tag4 }}</p>
    </div>
    <span>{{ txt }}</span>
  </div>
</template>

<style scoped>
.card {
  background: var(--vt-art-card-bg);
  padding: 30px;
  width: 264px;
  height: 262px;
  border-radius: 10px;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: space-between;
  position: relative;
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

p {
  font-family: Inter;
  font-size: 16px;
  font-weight: 400;
  line-height: 24px;
  position: absolute;
  top: 30px;
  right: 30px;
  letter-spacing: -0.41999998688697815px;
  text-align: left;
  text-underline-position: from-font;
  text-decoration-skip-ink: none;
}

p.tag1 {
  color: #46efe4;
}

p.tag2 {
  color: #7bf2ab;
}

p.tag3 {
  color: #b0f571;
}

p.tag4 {
  color: #ccf652;
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
  width: 100px;
  line-height: 38px;
  letter-spacing: -0.7799999713897705px;
  text-align: left;
  text-underline-position: from-font;
  text-decoration-skip-ink: none;
  color: var(--vt-white);
}

@media (max-width: 850px) {
  h3 {
    font-size: 18px;
    line-height: 31px
  }

  span, p {
    font-size: 12px;
    line-height: 16px;
  }

  .card {
    width: 182px;
    height: 180px;
  }
}
</style>
