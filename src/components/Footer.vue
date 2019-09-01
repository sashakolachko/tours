<template lang="html">
  <div class="footer">
    <p class="footer__text">Designed in {{ year }}</p>
  </div>
</template>

<script>
export default {
  name: "Footer",
  props: {
    year: String
  }
}
</script>

<style lang="scss" scoped>
.footer {
    width: 100vw;
    height: 35px;
    background-color: #0e7886;
    display: flex;
    align-items: center;
    justify-content: center;
    &__text {
        color: #fff;
        font-size: 14px;
    }
}
</style>
