<template>
  <main class="main-container">
    <div class="top">
      <Header />
    </div>

    <div class="bottom">
      <div class="left">
        <Nav />
      </div>

      <div class="right">
        <div class="content">
          <router-view />
        </div>
      </div>
    </div>
  </main>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import Header from '@/components/Header.vue'
import Nav from '@/components/Nav.vue'

export default defineComponent({
  name: 'Main',
  components: {
    Header,
    Nav
  }
})
</script>

<style scoped lang="stylus">
</style>
