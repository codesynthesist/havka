<template>
  <div class="container">
    <header class="header">
      <router-link to="/" class="header-logo">
        <img src="../assets/img/logo.png">
        <h1 class="header-logo__text">Чисто<span>пожрать</span></h1>
      </router-link>

      <Nav/>

      <div class="cart">Корзина</div>
    </header>
  </div>
</template>

<script>
import { Vue, Component } from 'vue-property-decorator';
import Nav from '@/components/Nav.vue';

@Component({
  components: {
    Nav,
  },
})

export default class Header extends Vue {

}
</script>

<style lang="sass">
.header
  display: flex
  justify-content: space-between
  align-items: center
  padding: 10px

.header-logo
  display: flex
  align-items: flex-end
  line-height: 1

  &__text
    display: block
    margin-left: 10px
    font-size: 16px

    span
      display: block
      font-size: 14px
  img
    width: 40px
</style>
