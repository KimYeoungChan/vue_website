<template>
  <footer>
    <div class="inner">
      <div class="f_logo">
        <h1>
          <a href="javascript:;">
            <img :src="footerLogo" alt="Footer Logo" />
          </a>
        </h1>
        <div class="copy_box">
          <p>Copyrights 2024. 테스트 All Rights Reserved</p>
        </div>
      </div>
    </div>
  </footer>
</template>

<script setup>
import footerLogo from '@/assets/f_logo.png';
</script>

<style scoped>
/* Add your footer styles here */
</style>