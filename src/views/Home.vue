<template>
  <AppHeader />

  <div class="main__container">
    <div class="hero-main">
      <div class="hero-text">
        <h1>Front-End React Developer</h1>
        <img
          src="/static/media/waving.1bae5fcfb51082b5c2b4.png"
          alt="waving_hand"
        />
        <p>
          Hi, I'm Stefan Topalovic. A passionate Front-end React Developer based
          in Belgrade, Serbia. 📍
        </p>
        <span>
          <a
            aria-label="linkedin"
            rel="noreferrer"
            target="_blank"
            href="https://www.linkedin.com/in/stefan-topalovic-dev/"
          >
            <i class="fa-brands fa-linkedin"></i>
          </a>
          <a
            aria-label="github"
            rel="noreferrer"
            target="_blank"
            href="https://github.com/stefvndev"
          >
            <i class="fa-brands fa-github"></i>
          </a>
        </span>
      </div>
      <div class="hero-img"></div>
    </div>
  </div>
</template>

<script setup>
import AppHeader from '@/components/AppHeader.vue'
</script>
<style>
.main__container {
  margin-block-start: 18rem;
  margin:  auto;
  max-width: 107rem;
  padding: 0 4rem;
}
</style>
