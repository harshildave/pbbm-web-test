<template>
  <v-app>
    <v-main>
      <v-container>
        <nav-bar />
        <nuxt />
      </v-container>
    </v-main>
    <v-footer :absolute="!fixed" app>
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>

<script>
import NavBar from '~/components/NavBar'
export default {
  components: {
    NavBar,
  },
  data() {
    return {
      fixed: false,
    }
  },
}
</script>
