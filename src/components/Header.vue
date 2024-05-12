<template>
  <header>
    <div class="inner">
      <h1>
        <a href="javascript:;">
          <img :src="logo" alt="Logo" />
        </a>
      </h1>
      <nav>
        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Contact</a></li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script setup>
import logo from "@/assets/logo.svg";
</script>
