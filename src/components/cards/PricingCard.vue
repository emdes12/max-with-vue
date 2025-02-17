<script setup>
import PrimaryButton from "../btn/PrimaryButton.vue";

defineProps({
  head: {
    type: String,
  },
  txt: {
    type: String,
  },
  featuredArr: {
    type: Array,
  },
  outputArr: {
    type: Array,
  },
  btnText: {
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
        <PrimaryButton widTH="100%" :txt="btnText" link="#" />
        <div class="line"></div>
        <ul>
          <h5>Features</h5>
          <li v-for="(feat, index) in featuredArr" :key="index">{{ feat }}</li>
        </ul>
        <ul>
          <h5>Outputs</h5>
          <li v-for="(output, index) in outputArr" :key="index">
            {{ output }}
          </li>
        </ul>
      </div>
    </div>
  </main>
</template>

<style scoped>
.line {
  width: 100%;
  height: 1px;
  margin: 30px 0;
  background: #f5e9032e;
}

ul {
  list-style-image: url("../../assets/icons/icon-rocketyzer-4.svg.svg");
  color: var(--vt-white);
  padding-inline-start: 30px;
  min-height: 90px;
}

li {
  font-family: Inter;
  font-size: 16px;
  font-weight: 500;
  line-height: 22px;
  letter-spacing: -0.3199999928474426px;
  text-align: left;
  text-underline-position: from-font;
  text-decoration-skip-ink: none;
}

h5 {
  font-family: Inter;
  font-size: 16px;
  font-weight: 700;
  line-height: 22px;
  letter-spacing: -0.3199999928474426px;
  text-align: left;
  text-underline-position: from-font;
  text-decoration-skip-ink: none;
}

.card-container {
  position: relative;
}

.card-container:hover .card-hover {
  background-image: linear-gradient(90deg, #45efe5 0%, #ccf652 90%);
}

.card-hover {
  background: transparent;
  transition: all 0.3s ease;
  border-radius: 10px;
  padding: 2px;
}

.card {
  border-radius: 10px;
  border: 1px #2b3254 solid;
  width: 350px;
  height: 810px;
  padding: 30px;
  gap: 30px;
  background: var(--vt-black);
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
  h5 {
    font-size: 14px;
    line-height: 18px
  }

  h3 {
    font-size: 24px;
    line-height: 27px
  }

  span, p {
    font-size: 12px;
    line-height: 16px;
  }

  .card {
    height: 650px;
  }
}
</style>
