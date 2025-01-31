<script setup>
import { ref } from "vue";
import Img1Tab from "../assets/images/image 9.png";

const tab1 = ref("active")
const tab2 = ref("")
const tab3 = ref("")
const tab4 = ref("")
const tabCorrespondImage = ref(Img1Tab)
</script>

<template>
  <main>
    <div class="navtab">
      <ul>
        <li :class="tab1">
          <h4>Advance AI Engine</h4>
          <p>Get relatime feedback & suggestions.</p>
        </li>
        <li :class="tab2">
          <h4>Wizard-Driven Interface</h4>
          <p>
            A Step-by-step guide to crafting your value propositions and
            messaging.
          </p>
        </li>
        <li :class="tab3">
          <h4>Comprehensive Output Data</h4>
          <p>
            From value propositions to marketing collateral, we’ve got you
            covered.
          </p>
        </li>
        <li :class="tab4">
          <h4>Value Proposition Toolkits Integrations</h4>
          <p>Ensuring methodoligucal consistency and effectiveness</p>
        </li>
      </ul>
    <div class="tabimg">
      <img :src="tabCorrespondImage" alt="tabeimage" />
    </div>
    </div>
  </main>
</template>

<style scoped>
.navtab {
  display: grid;
  width: 100%;
  grid-template-columns: 470px 1fr;
  grid-template-rows: 1fr;
  place-items: center;
}

ul {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 10px;
  /* background: orange; */
}

.tabimg {
  /* background: yellow; */
}

li {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: flex-start;
  width: 470px;
  padding: 30px;
  gap: 12px;
  border-radius: 12px;
  cursor: pointer;
  transition: all 0.2 linear;
}

h4 {
  font-family: Inter;
  font-size: 26px;
  font-weight: 600;
  line-height: 28.6px;
  letter-spacing: -0.7799999713897705px;
  text-align: left;
  text-underline-position: from-font;
  text-decoration-skip-ink: none;
  color: #525565;
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

img {
  width: 100%;
}

li.active {
  background: #CCF652;
}

li.active p, 
li.active h4{
  color: #292B3F;
}

li:hover {
  background: #CCF652;
}

li:hover p, 
li:hover h4{
  color: #292B3F;
}
</style>
