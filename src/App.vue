<template>
  <div id="app">
    <transition name="fade-transform" mode="out-in">
      <router-view />
    </transition>
  </div>
</template>

<style lang="scss">
[v-cloak] {
  display: none !important;
}
</style>
