<template lang="html">
<div class="tour-box">
  <img class="tour-box__img" :src=imgUrl alt="">
  <p class="tour-box__dest">{{ destination }}</p>
  <p class="tour-box__date">{{ date }}</p>
  <p class="tour-box__descr">{{ description }}</p>
</div>
</template>

<script>
export default {
  name: 'Tour',
  props: {
    destination: String,
    date: String,
    description: String,
    imgUrl: String
  }
}
</script>

<style lang="scss" scoped>
.tour-box {
    width: 300px;
    height: fit-content;
    display: flex;
    flex-direction: column;
    align-items: center;

    &__img {
        width: 100%;
        height: 200px;
    }

    &__date {
        font-size: 18px;
    }
    &__dest {
        margin: 10px 0 0;
        font-size: 20px;
        color: #ff757c;
        font-weight: 500;
    }

}
.tour-box p {
    margin: 10px 0 0;
}
</style>
