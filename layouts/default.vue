<template>
  <v-app dark>
    <Header :dark="lightTheme"/>
    <v-main>
      <nuxt />
    </v-main>
  </v-app>
</template>

<script>
import Header from '~/components/Header';

export default {
  components: {
    Header,
  },
  computed: {
    lightTheme() {
      return !(this.$route.name === 'offer');
    }
  },
  data () {
    return {
    }
  }
}
</script>
