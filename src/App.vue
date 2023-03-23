<template>
  <div>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css"
      integrity="sha512-SzlrxWUlpfuzQ+pcUCosxcglQRNAq/DZjVsC0lE40xsADsfeQoEypE+enwcOiGjk/bSuGGKHEyjSoQ1zVisanQ=="
      crossorigin="anonymous" referrerpolicy="no-referrer" />

    <Menu :logo="true">
      <template v-slot:primary>
        <ul class="menu__list d-flex">
          <li class="menu__list-item">
            <router-link to="/" class="menu__list-link standard"> More Apps </router-link>
          </li>
          <li class="menu__list-item">
            <router-link to="/" class="menu__list-link standard"> Games </router-link>
          </li>
        </ul>
      </template>

      <template v-slot:secondary>
        <ul class="menu__list d-flex">
          <li class="menu__list-item standard__icon">
            <router-link to=""> <i class="fa-sharp fa-solid fa-chart-simple"></i> </router-link>
          </li>
          <li class="menu__list-item standard__icon">
            <router-link to=""> <i class="fa-solid fa-user"></i> </router-link>
          </li>
          <li class="menu__list-item standard__icon danger">
            <i class="fa-solid fa-right-from-bracket"></i>
          </li>
        </ul>
      </template>
    </Menu>
  </div>
</template>

<script>
import Menu from './components/Menu.vue';

export default {
  name: 'App',
  components: {
    Menu
  }
}
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  list-style: none;
  text-decoration: none;
  box-sizing: border-box;

  font-family: sans-serif;
}
</style>