<template>
 <div class="home">
   <div class="home--first_section">
     <div class="home--left_header">
       <p>Inwentaryzacje</p>
     </div>
     <div class="home--right_header">
       <p>PAPIN</p>
     </div>
     <v-icon x-large class="home--bottom_navigator">mdi-chevron-down</v-icon>
   </div>
   <div class="home--second_section">
     <div class="home--bottom_layout">
       <div class="home--bottom_header">
         <p>Witamy na naszej stronie</p>
       </div>
       <div class="home--bottom_content">
         content
       </div>
       <div class="home--bottom_image">
         <img :src="BG"/>
         <div class="home--upper-color"/>
         <div class="home--bottom-color"/>
       </div>
     </div>
   </div>
 </div>
</template>

<script>
import BG from '@/static/BG_Home_2.png'

export default {
  components: {
  },
  data() {
    return {
      BG,
    }
  },
  mounted() {
    console.log(this.$route.name)
  }
}
</script>
