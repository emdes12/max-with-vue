<script setup>
</script>

<template>
 <nav>
  <ul>
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
nav ul {
  list-style-type: none;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 29px;
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
padding: 8px 10px;
border-radius: 12px;
background-color: transparent;
}

a:hover {
  background-color: var(--vt-white);
  color: var(--body-bg);
}
</style>
