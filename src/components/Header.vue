<template lang="html">
  <nav class="header">
    <img class="header__logo" src="../assets/logo.png" alt="Logo">
    <ul class="header__list">
      <li class="header__list__item" v-for="item in links">
          {{ item }}
      </li>
    </ul>
  </nav>

</template>

<script>
export default {
  name: 'Header',
  data: () => {
    return {
      links: ["Special Price", "About Us", "Contacts"]
    }
  }
}
</script>

<style lang="scss" scoped>
.header {
    width: 80vw;
    height: 64px;
    margin-top: 10px;
    display: flex;
    justify-content: flex-end;

    &__logo {
        align-self: center;
        margin-right: auto;
        height: inherit;
    }
    &__list {
        list-style-type: none;
        align-items: center;
        display: flex;
        width: 30vw;
        justify-content: space-between;
        padding: 0;
        color: #ff757c;
        font-size: 22px;
    }
}
</style>
