<script setup>
defineProps({
  head: {
    type: String,
  },
  txt: {
    type: String,
  },
});
</script>

<template>
  <main class="card-container">
    <div class="card-hover">
      <div class="card">
        <h3>{{ head }}</h3>
        <p>{{ txt }}</p>
      </div>
    </div>
  </main>
</template>

<style scoped>
.card-container {
  position: relative;
}

.card-container:hover .card-hover {
  background-image: linear-gradient(90deg, #45efe5 0%, #ccf652 90%);
}
.card-container:hover .card {
  background: #212121;
}

.card-hover {
  background: transparent;
  transition: all 0.3s ease;
  border-radius: 10px;
  padding: 1px;
}

.card {
  border-radius: 10px;
  border: 1px #2b3254 solid;
  width: 370px;
  height: 470px;
  padding: 30px;
  gap: 30px;
  background: #0e0e0e;
  display: flex;
  flex-direction: column;
  z-index: 1000000;
}

h3 {
  font-family: Inter;
  font-size: 32px;
  font-weight: 600;
  line-height: 38px;
  letter-spacing: -0.9599999785423279px;
  text-align: left;
  text-underline-position: from-font;
  text-decoration-skip-ink: none;
  color: var(--vt-white);
}

p {
  font-family: Inter;
  font-size: 16px;
  font-weight: 400;
  line-height: 24px;
  letter-spacing: -0.41999998688697815px;
  text-align: left;
  text-underline-position: from-font;
  text-decoration-skip-ink: none;
  color: #8c929e;
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
    width: 230px;
    padding: 20px;
    height: 340px;
  }
}
</style>
