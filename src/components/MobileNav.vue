<script setup>
</script>

<template>
 <nav>
  <ul class="container">
    <a href="#about">
      <li>About</li>
    </a><a href="#how-it-work">
      <li>How it works</li>
    </a><a href="#outputs">
      <li>Outputs</li>
    </a><a href="#pricing">
      <li>Pricing</li>
    </a>
  </ul>
 </nav>
</template>

<style scoped>
nav {
  position: absolute;
  top: 130px;
  left: 0;
  right: 0;
  width: 100%;
  display: grid;
  height: -webkit-fill-available;
  background-color: var(--body-bg);
  padding: 20px;
}
nav ul {
  list-style-type: none;
  display: flex;
  align-items: start;
  width: 100%;
  justify-content: flex-start;
  gap: 29px;
  flex-direction: column;
}

a {
  text-decoration: none;
  color: var(--vt-white);
  font-family: Inter;
font-size: 16px;
font-weight: 700;
line-height: 17px;
letter-spacing: -0.6399999856948853px;
text-align: left;
text-underline-position: from-font;
text-decoration-skip-ink: none;
padding: 8px 12px;
border-radius: 5px;
background-color: transparent;
}

a:hover {
  background-color: var(--vt-white);
  color: var(--body-bg);
}
</style>
