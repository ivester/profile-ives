<script setup>
import { ref } from 'vue'

const navLinks = ref([
  {
    label: 'Home',
    url: '/'
  },
  {
    label: 'Todo',
    url: '/todo'
  }
])

const useColor = ref('')
</script>

<template>
  <nav class="main-nav">
    <ul>
      <li v-for="item in navLinks">
        <nuxt-link :to="item.url">{{item.label}}</nuxt-link>
      </li>
      <li><input type="color" v-model="useColor"></li>
    </ul>
  </nav>
</template>

<style>
.main-nav ul {
  display: flex;
}
.main-nav li {
  list-style: none;
  padding: 0 12px;
}

.main-nav .router-link-active {
  background-color: v-bind(useColor);
}
</style>