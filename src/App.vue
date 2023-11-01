<template>
  <body class="bg-background">
    <header>
      <Navbar />
    </header>
    <main>
      <router-view />
    </main>
    <footer class="text-light">
      Made with 💖 by CodeWorks
    </footer>
  </body>
</template>

<script>
import { computed } from 'vue'
import { AppState } from './AppState'
import Navbar from './components/Navbar.vue'

export default {
  setup() {
    return {
      appState: computed(() => AppState)
    }
  },
  components: { Navbar }
}
</script>
<style lang="scss">
.bg-img {
  // Sky - purple
  // background-image: url(https://images.unsplash.com/photo-1602498456745-e9503b30470b?auto=format&fit=crop&q=80&w=1974&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D);
  // winding forest road
  // background-image: url(https://images.unsplash.com/photo-1606830079880-e90bd08e9a98?auto=format&fit=crop&q=80&w=1974&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D);
  // beach - aerial
  // background-image: url(https://images.unsplash.com/photo-1524946274118-e7680e33ccc5?auto=format&fit=crop&q=80&w=2070&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D);
  // Shanghai
  background-image: url(https://images.unsplash.com/photo-1614221330834-9399e5631af3?auto=format&fit=crop&q=80&w=2067&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D);
  object-fit: cover;
  object-position: center;
}


@import "./assets/scss/main.scss";

:root {
  --main-height: calc(100vh - 32px - 64px);
}


footer {
  display: grid;
  place-content: center;
  height: 32px;
}
</style>
