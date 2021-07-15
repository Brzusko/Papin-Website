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
       <div class="home--bottom_content-wrapper">
         <div class="home--bottom_content">
           <div class="home--bottom_content__text">
             <p>
               Zajmujemy się sporządzaniem różnorodnych dokumentacji środowiskowych - prowadzimy
               inwentaryzacje przyrodnicze w zakresie siedlisk przyrodniczych oraz gatunków roślin, grzybów i zwierząt, sporządzamy dokumentacje niezbędne do uzyskania decyzji środowiskowej:
             </p>
             <p>
               <b class="bold-color">-karty informacyjne przedsięwzięcia (KIP)</b>
               <br/>
               <br/>
               <b class="bold-color">-raporty o oddziaływaniu na środowisko (ROŚ)</b>
             </p>
             <p>
               Sporządzamy również prognozy oddziaływania na środowisko dla projektów miejscowych planów zagospodarowania przestrzennego (MPZP) i studium uwarunkowań i kierunków zagospodarowania przestrzennego.
             </p>
           </div>
           <div class="home--bottom_content__img">
              <img :src="plant"/>
           </div>
         </div>
       </div>
     </div>
   </div>
 </div>
</template>

<script>
import BG from '@/static/BG_Home_2.png';
import plant from '@/static/plant.png';

export default {
  components: {
  },
  data() {
    return {
      BG,
      plant
    }
  },
  mounted() {
    console.log(this.$route.name)
  }
}
</script>
