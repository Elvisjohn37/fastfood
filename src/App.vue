<template>
  <div>
      <MainNavigation />
  <div :class="styles.app">
    <RouterView />
  </div>
  </div>
</template>

<script setup>
import { RouterView } from 'vue-router'
import MainNavigation from './components/MainNavigation.vue'
import styles from './App.module.scss'
</script>
