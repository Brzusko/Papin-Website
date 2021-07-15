<template>
  <div class="gallery">
    <v-carousel hide-delimiters cycle :interval="4000" progress progress-color="red">
      <v-carousel-item
        v-for="(image, index) in images"
        :key="index"
        :src="`${path}${image}`"
        >
      </v-carousel-item>
    </v-carousel>
    <p class="gallery--button" @click="showOverlay = !showOverlay">
      Kliknij aby zobaczyć całą galerie
    </p>
    <v-dialog v-model="showOverlay" fullscreen>
      <v-btn
        class="mx-2 gallery--exit"
        fab
        dark
        small
        color="#F3EEF0"
      >
        <v-icon color="red">
          mdi-close
        </v-icon>
      </v-btn>
      <div
        v-for="(image, index) in images"
        :key="index"
        class="gallery--image"
        :style="`background: url('${path}${image}') no-repeat;`"
      />
    </v-dialog>
  </div>
</template>

<script>

export default {
  data() {
    return {
      path: 'http://localhost:9000',
      images: [],
      showOverlay: false,
    };
  },
  components: {
  },
  mounted() {
    console.log(this.$route.name);
    this.$fetch();
  },
  async fetch() {
    const res = await this.$axios.get(`${this.path}/gallery`);
    this.images = res.data.length ? res.data : [];
  }
}
</script>
