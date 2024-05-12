<template>
  <div class="card_list">
    <div class="img">
      <img :src="card.imgSrc" :alt="card.alt" />
    </div>
    <div class="txt_box">
      <div class="tit">
        <h4>{{ card.title }}</h4>
        <p>{{ card.content }}</p>
      </div>
      <div class="btm_box">
        <p class="sub_text">{{ card.subText }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    card: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style scoped>
/* 필요한 스타일을 추가하세요 */
</style>