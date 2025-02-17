<script setup>
import SecondaryButton from "./btn/SecondaryButton.vue";
import Logo from "../assets/icons/Link → logo-rocketyzer.svg.svg";
</script>

<template>
  <main class="container">
    <div class="flex-cta">
      <div class="caption">
        <h2>Ready to Elevate</h2>
        <h3>Your Marketing Game?</h3>
      </div>
      <SecondaryButton txt="Get Started for Free" link="#" />
    </div>
  </main>

  <main class="container">
    <div class="foot-copyright">
      <a href="#">
        <img :src="Logo" alt="" />
      </a>
      <div class="line"></div>
      <div class="copyright">
        <p>© 2023 Rocketyzer. All rights reserved.</p>
        <div class="special-links">
            <a href="#">Privacy Policy</a>
            <a href="#">Terms and & Conditions</a>
        </div>
      </div>
    </div>
  </main>
</template>

<style scoped>
.flex-cta {
  width: 100%;
  flex-direction: column;
  border-radius: 12px;
  gap: 30px;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 50px;
  background: #ccf652;
}

h3, h2 {
  font-family: Manrope;
  font-size: 71px;
  font-weight: 600;
  line-height: 71px;
  letter-spacing: -2.130000114440918px;
  text-align: center;
  text-underline-position: from-font;
  text-decoration-skip-ink: none;
}

h2 {
    color: #292B3F;
}

h3 {
    color: #292B3F66;
}

.foot-copyright {
  display:flex;
  flex-direction: column;
  gap: 30px;
  padding-top: 30px;
}

.foot-copyright img {
  width: 100px;
}

.line {
  width: 100%;
  height: 1px;
  background-image: linear-gradient(90deg, #292B3F66, #292B3F);
}

.copyright {
  display: flex;
  align-items: center;
  color: #aaa;
  gap: 30px;
  justify-content: space-between;
}

.special-links {
  display:flex;
  align-items: center;
  justify-content: center;
  gap: 20px;
}

.special-links a {
  color: #aaa;
  transition: all 0.2s ease;
}

.special-links a:hover {
  color: #fff;
}

@media (max-width: 850px) {
  .copyright {
    justify-content: center;
    flex-direction: column;
    font-size: 12px;
  }
  
  img {
    width: 100px;
  }

  h2, h3 {
    font-size: 45px;
    line-height: 45px;
  }
}
</style>
