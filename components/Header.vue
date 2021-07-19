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
      <nuxt-link :to="routes[3].path" class="it-header--link">
          {{ routes[3].name }}
      </nuxt-link>
      <nuxt-link :to="routes[4].path" class="it-header--link">
          {{ routes[4].name }}
      </nuxt-link>
      <img :src="Logo"/>
      <v-icon x-large color="black" @click="showMobileMenu = true" class="visible-mobile">mdi-menu</v-icon>
      <v-dialog v-model="showMobileMenu" fullscreen transition="dialog-top-transition" hide-overlay>
        <div class="it-header--mobile">
          <v-icon class="absolute-icon" x-large color="black" @click="showMobileMenu = false">mdi-alpha-x</v-icon>
          <img :src="Logo"/>
          <nuxt-link exact :to="routes[0].path" class="it-header--link-mobile" @click="showMobileMenu = false">
            {{ routes[0].name }}
          </nuxt-link>
          <nuxt-link :to="routes[1].path" class="it-header--link-mobile" @click="showMobileMenu = false">
            {{ routes[1].name }}
          </nuxt-link>
          <nuxt-link :to="routes[2].path" class="it-header--link-mobile" @click="showMobileMenu = false">
            {{ routes[2].name }}
          </nuxt-link>
          <nuxt-link :to="routes[3].path" class="it-header--link-mobile" @click="showMobileMenu = false">
            {{ routes[3].name }}
          </nuxt-link>
          <nuxt-link :to="routes[4].path" class="it-header--link-mobile" @click="showMobileMenu = false">
            {{ routes[4].name }}
          </nuxt-link>
        </div>
      </v-dialog>
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
            showMobileMenu: false,
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
