<template>
  <div class="it-header" :class="{ dark }">
      <nuxt-link exact :to="routes[0].path" class="it-header--link">
          {{ routes[0].name }}
      </nuxt-link>
      <nuxt-link :to="routes[1].path" class="it-header--link">
          {{ routes[1].name }}
      </nuxt-link>
      <nuxt-link :to="routes[2].path" class="it-header--link">
          {{ routes[2].name }}
      </nuxt-link>
<!--      <div class="it-header&#45;&#45;logo">-->
<!--          <img :src="Logo"/>-->
<!--      </div>-->
      <nuxt-link :to="routes[3].path" class="it-header--link">
          {{ routes[3].name }}
      </nuxt-link>
      <nuxt-link :to="routes[4].path" class="it-header--link">
          {{ routes[4].name }}
      </nuxt-link>
      <img :src="Logo"/>
  </div>
</template>

<script>
import Logo from '@/static/LOGO.png';

export default {
    components: {
    },
    props: {
      dark: {
        type: Boolean,
        default: false
      }
    },
    data () {
        return {
            Logo,
            routes: [
                {
                    path: '/',
                    name: 'Strona Główna',
                    isActive: false,
                },
                {
                    path: '/about',
                    name: 'O nas',
                    isActive: false,
                },
                {
                    path: '/offer',
                    name: 'Oferta',
                    isActive: false,
                },
                {
                    path: '/gallery',
                    name: 'Galeria zdjęć',
                    isActive: false,
                },
                {
                    path: '/contact',
                    name: 'Kontakt',
                    isActive: false,
                },
            ]
        }
    }
}
</script>
