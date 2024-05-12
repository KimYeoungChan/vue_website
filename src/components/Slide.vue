<template>
  <swiper :navigation="true" :modules="modules" class="mySwiper">
    <swiper-slide v-for="(slide, index) in slides" :key="index">
      <div class="inner">
        <div class="txt_box">
          <h3>{{ slide.title }}</h3>
          <p>{{ slide.description }}</p>
        </div>
      </div>
      <div class="img_box">
        <img :src="slide.image" alt="대체_텍스트" />
      </div>
    </swiper-slide>
  </swiper>
</template>
<script>
import main from '@/assets/main.jpg'
import { ref } from 'vue';
import { Swiper, SwiperSlide } from 'swiper/vue';
import 'swiper/css';
import 'swiper/css/navigation';
import { Navigation } from 'swiper/modules';

export default {
  data() {
    return {
      slides: [
        { title: 'Slide 1', description: 'Description for slide 1', image: main },
        { title: 'Slide 2', description: 'Description for slide 2', image: main },
        { title: 'Slide 3', description: 'Description for slide 3', image: main }
      ],
      modules: [] // Define your modules if needed
    };
  },
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    const modules = [Navigation];
    const mainImage = ref(main);

    return {
      modules,
      main: mainImage,
    };
  },
};
</script>

<style>

.swiper-button-prev, .swiper-button-next {
  color: #fff !important;
}

.mySwiper {
  height: 750px;
  position: relative;
}

.swiper-slide .inner {
  display: flex;
  justify-content: flex-start;
  align-items: center;
  height: 100%;
}

.swiper-slide .txt_box {
  position: relative;
  z-index: 1;
}

.swiper-slide .txt_box h3 {
  color: #fff;
  font-size: 71px;
  line-height: 1em;
}

.swiper-slide .txt_box p {
  margin-top: 70px;
  font-size: 31px;
  color: #fff;
  line-height: 1em;
}

.swiper-slide .img_box {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}

.swiper-slide img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>