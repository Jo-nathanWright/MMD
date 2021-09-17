<template>
  <header>
    <Navbar />
  </header>
  <main id="grad">
    <router-view />
  </main>
</template>

<script>
import { computed } from 'vue'
import { AppState } from './AppState'
export default {
  name: 'App',
  setup() {
    return {
      appState: computed(() => AppState)
    }
  }
}
</script>
<style lang="scss">
@import "./assets/scss/main.scss";

#grad {
  background-image: linear-gradient(#118593, #a712dd);
}
</style>
