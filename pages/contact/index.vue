<template>
  <div class="contact">
    <div class="contact--card visible-desktop">
      <img :src="Plant" class="contact--card__plant"/>
    </div>
    <div class="contact--content">
      <div class="contact--content__up">
        <div class="contact--content__container">
          <p class="contact--content__header">Kontakt</p>
          <div class="contact--content__text">
            Zapraszamy do kontaktu – oferujemy rzetelną dokumentację, w konkurencyjnych cenach.<br>
            Obszar naszych działań to zasadniczo rejen Śląska i Polski południowej, ale po uzgodnieniu warunków możemy również dalej
          </div>
        </div>
      </div>
      <div class="contact--content__down">
        <div class="contact--content__info">
          <p>Aleksandra Papin</p>
          <div class="contact--content__field">
            <div class="contact--content__data">
              <div class="contact--content__data--header">
                <v-icon class="icon" color="black">mdi-email</v-icon>
                <span>Email</span>
              </div>
              <p class="contact--content__data--info">aksandra79@gmail.com</p>
            </div>
            <div class="contact--content__data">
              <div class="contact--content__data--header">
                <v-icon class="icon" color="black">mdi-phone</v-icon>
                <span>Numer Kontaktowy</span>
              </div>
              <p class="contact--content__data--info">795 127 970</p>
            </div>
          </div>
        </div>
        <div class="contact--content__info">
          <p>Marek Papin</p>
          <div class="contact--content__field">
            <div class="contact--content__data">
              <div class="contact--content__data--header">
                <v-icon class="icon" color="black">mdi-email</v-icon>
                <span>Email</span>
              </div>
              <p class="contact--content__data--info">markus-km@wp.pl</p>
            </div>
            <div class="contact--content__data">
              <div class="contact--content__data--header">
                <v-icon class="icon" color="black">mdi-phone</v-icon>
                <span>Numer Kontaktowy</span>
              </div>
              <p class="contact--content__data--info">604 697 148</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Plant from 'static/plant.png';

export default {
  data() {
    return {
      Plant,
    }
  },
  components: {
  },
}
</script>
