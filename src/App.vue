<template>
  <Header />
  <MySwiper />
  <CardList />

  <section class="section con02"></section>

  <Footer />
</template>

<script>
import Header from '@/components/Header.vue';
import Footer from '@/components/Footer.vue';
import CardList from '@/components/CardList.vue';
import MySwiper from '@/components/Slide.vue'


export default {
  components: {
    Header,
    Footer,
    CardList,
    MySwiper,
},
};
</script>

