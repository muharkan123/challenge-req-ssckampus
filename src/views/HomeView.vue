<template>
  <div class="home">
    <div class="container ">
      <navbarView />
      <heroView />
    </div>
    <footerView />
  </div>
</template>

<script>
// @ is an alias to /src

import navbarView from '@/components/navbarView.vue'
import heroView from '@/components/heroView.vue'
import footerView from '@/components/footerView.vue'
export default {
  name: 'HomeView',
  components: {
    navbarView,
    heroView,
    footerView
  }
}
</script>
