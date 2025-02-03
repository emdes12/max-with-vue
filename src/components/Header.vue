<script setup>
import { ref } from "vue"
import PrimaryButton from "./btn/PrimaryButton.vue";
import NavBar from "./NavBar.vue";
import MobileNav from "./MobileNav.vue";
import Logo from "../assets/icons/Link → logo-rocketyzer.svg.svg";

let isActive = ref("hamburger");
let isMenu = ref(false);

const toggleActive = () => {
  isActive.value = isActive.value === "hamburger" ? "hamburger is-active" : "hamburger";
  isMenu.value = !isMenu.value
}
</script>

<template>
  <header>
    <div class="container">
      <a href="#">
        <img :src="Logo" alt="" />
      </a>

      <NavBar class="show-desktop" />

      <div class="menu-icon show-mobile">
        <div class="three col" @click="toggleActive">
          <div :class="isActive" id="hamburger-1">
            <span class="line"></span>
            <span class="line"></span>
            <span class="line"></span>
          </div>
        </div>
      </div>

      <PrimaryButton  class="show-desktop" txt="Get started free" link="#" />

      <MobileNav class="show-mobile" v-show="isMenu" />
    </div>
  </header>
</template>

<style scoped>
header {
  width: 100vw;
}

.container {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.show-mobile {
  display: none;
}

.row .three{
  padding: 80px 30px;
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
  background-color: #2c3e50;
  color: #ecf0f1;
  text-align: center;
}

.hamburger .line{
  width: 50px;
  height: 5px;
  background-color: #ecf0f1;
  display: block;
  margin: 8px auto;
  -webkit-transition: all 0.3s ease-in-out;
  -o-transition: all 0.3s ease-in-out;
  transition: all 0.3s ease-in-out;
}

.hamburger:hover{
  cursor: pointer;
}

#hamburger-1.is-active .line:nth-child(2){
  opacity: 0;
}

#hamburger-1.is-active .line:nth-child(1){
  -webkit-transform: translateY(13px) rotate(45deg);
  -ms-transform: translateY(13px) rotate(45deg);
  -o-transform: translateY(13px) rotate(45deg);
  transform: translateY(13px) rotate(45deg);
}

#hamburger-1.is-active .line:nth-child(3){
  -webkit-transform: translateY(-13px) rotate(-45deg);
  -ms-transform: translateY(-13px) rotate(-45deg);
  -o-transform: translateY(-13px) rotate(-45deg);
  transform: translateY(-13px) rotate(-45deg);
}

@media (max-width: 850px) {
  .show-mobile {
    display: block;
  }

  .show-desktop {
    display: none;
  }
}
</style>
