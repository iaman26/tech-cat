<template>
  <div class="header">
    <div class="container">
      <a href="/" class="header__logo">
        <img src="~/assets/img/logo.png" alt="" />
      </a>
      <div class="mobile-btn" @click="onHeader()" :class="{ active: isHeader }">
        <svg
          class="default"
          xmlns="http://www.w3.org/2000/svg"
          width="40"
          height="40"
          viewBox="0 0 40 40"
          fill="none"
        >
          <path
            d="M8.3335 8.33333H20.0002H31.6668"
            stroke="#F8F7FF"
            stroke-width="4"
            stroke-linecap="round"
          />
          <path
            d="M8.3335 20H31.6668"
            stroke="#F8F7FF"
            stroke-width="4"
            stroke-linecap="round"
          />
          <path
            d="M8.3335 31.6667H20.0002H31.6668"
            stroke="#F8F7FF"
            stroke-width="4"
            stroke-linecap="round"
          />
        </svg>
        <svg
          class="close"
          xmlns="http://www.w3.org/2000/svg"
          width="40"
          height="40"
          viewBox="0 0 40 40"
          fill="none"
        >
          <path
            d="M8.3335 8.33333L20.0002 20L31.6668 8.33333"
            stroke="#F8F7FF"
            stroke-width="4"
            stroke-linecap="round"
          />
          <path
            d="M8.3335 31.6667L20.0002 20L31.6668 31.6667"
            stroke="#F8F7FF"
            stroke-width="4"
            stroke-linecap="round"
          />
        </svg>
      </div>
      <div class="header__links" :class="{ active: isHeader }">
        <a href="/" class="links__link">Home</a>
        <a href="#about" class="links__link">About</a>
        <a href="#tokenomics" class="links__link">Tokenomics</a>
        <a href="https://myrothedog.com/MyroWP.pdf" class="links__link"
          >Whitepaper</a
        >
        <a href="#social" class="links__link">Socials</a>
        <a href="#" target="_blank" class="links__btn">Join Telegram</a>
        <div class="social__links">
          <a href="#" target="_blank">
            <img src="~/assets/img/social_x.png" alt="" />
          </a>
          <a href="#" target="_blank">
            <img src="~/assets/img/social_tg.png" alt="" />
          </a>
        </div>
      </div>
    </div>
  </div>
</template>
<script setup>
let isHeader = ref(false)
function onHeader() {
  isHeader.value = !isHeader.value
}
</script>
