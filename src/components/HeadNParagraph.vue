<script setup>
defineProps({
  head1: {
    type: String,
    default: "Header",
    required: true,
  },
  head2: {
    type: String,
    default: "Header2",
    required: true,
  },
  txt: {
    type: String,
    default:
      "Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum ",
    required: true,
  },
  flD: {
    type: String,
    default: "column",
  },
});
</script>

<template>
  <div class="flex" :style="'flex-direction: ' + flD">
    <div class="head">
      <h1 class="head1">{{ head1 }}</h1>
      <h1 class="head2">{{ head2 }}</h1>
    </div>
    <p>
      {{ txt }}
    </p>
  </div>
</template>

<style scoped>
.flex {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 30px;
}
.head {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}

h1 {
  font-family: Manrope;
  font-size: 71px;
  font-weight: 600;
  line-height: 71px;
  letter-spacing: -2.130000114440918px;
  text-align: center;
  text-underline-position: from-font;
  text-decoration-skip-ink: none;
}

.head1 {
  color: var(--vt-white);
}

.head2 {
  background: linear-gradient(90deg, #45efe5 0%, #ccf652 85%);
  -webkit-text-fill-color: transparent;
  -webkit-background-clip: text;
}

p {
  font-family: Manrope;
  font-size: 18px;
  font-weight: 500;
  line-height: 27px;
  letter-spacing: -0.3199999928474426px;
  text-align: center;
  text-underline-position: from-font;
  text-decoration-skip-ink: none;
  color: var(--vt-white);
  max-width: 520px;
}
</style>
