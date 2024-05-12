<template>
  <section class="section con01">
    <div class="inner">
      <ul class="card_box">
        <li v-for="(card, index) in cards" :key="index">
          <Card :card="card" />
        </li>
      </ul>
    </div>
  </section>
</template>

<script setup>
import Card from '@/components/Card.vue';
import img1 from '@/assets/img1.jpg'
import img2 from '@/assets/img2.jpg'
import img3 from '@/assets/img3.jpg'
import img4 from '@/assets/img4.jpg'

const cards = [
  {
    imgSrc: img1,
    alt: '카드이미지',
    title: 'Lorem ipsum dolor sit amet,',
    content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.',
    subText: 'Lorem ipsum dolor sit amet,',
  },
  {
    imgSrc: img2,
    alt: '카드이미지',
    title: 'Lorem ipsum dolor sit amet,',
    content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.',
    subText: 'Lorem ipsum dolor sit amet,',
  },
  {
    imgSrc: img3,
    alt: '카드이미지',
    title: 'Lorem ipsum dolor sit amet,',
    content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.',
    subText: 'Lorem ipsum dolor sit amet,',
  },
  {
    imgSrc:img4,
    alt: '카드이미지',
    title: 'Lorem ipsum dolor sit amet,',
    content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.',
    subText: 'Lorem ipsum dolor sit amet,',
  },
];
</script>

<style scoped>
/* 필요한 스타일을 추가하세요 */
</style>