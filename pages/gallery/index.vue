<template>
  <div class="gallery" id="anchor">
    <v-carousel hide-delimiters cycle :interval="4000" progress progress-color="red" class="visible-desktop">
      <v-carousel-item
        v-for="(image, index) in images"
        :key="index"
        :src="`${path}${image}`"
        >
      </v-carousel-item>
    </v-carousel>
    <p class="gallery--button visible-desktop" @click="showOverlay = !showOverlay">
      Kliknij aby zobaczyć całą galerie
    </p>
    <v-dialog v-model="showOverlay" max-width="85vw">
      <v-toolbar color="white" light>
        <v-toolbar-title>Galeria Zdjęć</v-toolbar-title>
        <v-spacer/>
        <v-btn
          class="mx-2 gallery--exit"
          fab
          light
          x-small
          color="#F3EEF0"
          @click="showOverlay = !showOverlay"
        >
          <v-icon color="black">
            mdi-close
          </v-icon>
        </v-btn>
      </v-toolbar>
      <div
        v-for="(image, index) in images"
        :key="index"
        class="gallery--image"
        :style="`background: url('${path}${image}') no-repeat;`"
      />
    </v-dialog>
    <div class="gallery--mobile visible-mobile">
      <div class="gallery--mobile__header" id="header">
        <p>Galeria Zdjęć</p>
      </div>
      <v-img
        v-for="(image, index) in images"
        :key="index"
        :src="`${path}${image}`"
        max-width="95vw"
      />
      <v-btn
        class="mx-2 gallery--scroll"
        fab
        light
        large
        color="#F3EEF0"
        link
      >
        <a href="#anchor" v-smooth-scroll style="border: none; color: transparent;">
          <v-icon color="black" x-large>
            mdi-chevron-up
          </v-icon>
        </a>
      </v-btn>
    </div>
  </div>
</template>

<script>

export default {
  data() {
    return {
      path: 'https://api.inwentaryzacje-papin.pl',
      images: [],
      showOverlay: false,
      showImage: false,
      selectedImage: '',
    };
  },
  components: {
  },
  mounted() {
    this.$fetch();
  },
  async fetch() {
    const res = await this.$axios.get(`${this.path}/gallery`);
    this.images = res.data.length ? res.data : [];
  }
}
</script>
