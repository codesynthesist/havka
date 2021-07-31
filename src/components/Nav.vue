<template>
  <nav class="nav">
    <ul>
      <li>
        <router-link to="/pizza">Пицца</router-link>
      </li>
      <li>
        <router-link to="/sushi">Суши</router-link>
      </li>
      <li>
        <router-link to="/wok">Вок</router-link>
      </li>
      <li>
        <router-link to="/grill">Гриль</router-link>
      </li>
    </ul>
  </nav>
</template>

<script lang="js">
import Vue from 'vue';

export default class Nav extends Vue {

}

</script>

<style lang="sass">
.nav
  display: flex
  justify-content: flex-end

  ul
    display: flex
    list-style: none

    li
      margin: 10px 10px

      a
        text-decoration: none
</style>
