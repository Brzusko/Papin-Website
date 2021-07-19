<template>
  <div class="offer">
    <div class="offer--header">
      <v-parallax :src="bg">
        <div class="offer--header__text">
          <span>CO</span>
          <span>OFERUJEMY</span>
        </div>
      </v-parallax>
    </div>
    <div class="offer--body">
      <div class="offer--body__title">
        Oferujemy następujące dokumentacje z zakresu ochrony środowiska:
      </div>
      <v-container>
        <v-row>
          <v-col cols="12" sm="4">
            <div class="offer--card">
              <div class="offer--card__header">
                <v-icon x-large>mdi-chart-bar</v-icon>
              </div>
              <div class="offer--card__body">
                <ul>
                  <li>Waloryzacje przyrodnicze i opisy uwarunkowań środowiskowych</li>
                  <li>Szczegółowe inwentaryzacje przyrodnicze</li>
                </ul>
              </div>
            </div>
          </v-col>
          <v-col cols="12" sm="4">
            <div class="offer--card">
              <div class="offer--card__header">
                <v-icon x-large>mdi-clipboard-multiple-outline</v-icon>
              </div>
              <div class="offer--card__body">
                <ul>
                  <li>
                    Opinie w zakresie ptaków i nietoperzy dotyczące termomodernizacji
                    budynków
                  </li>
                  <li>Badania ukierunkowane na szczególnie wrażliwe grupy gatunków
                    (np. płazy lub nietoperze) – z wykorzystaniem metod akustycznych
                    w tym detektora ultradźwiękowego i specjalistycznego
                    oprogramowania
                  </li>
                </ul>
              </div>
            </div>
          </v-col>
          <v-col cols="12" sm="4">
            <div class="offer--card">
              <div class="offer--card__header">
                <v-icon x-large>mdi-magnify</v-icon>
              </div>
              <div class="offer--card__body">
                <ul>
                  <li>Inwentaryzacje dendrologiczne</li>
                  <li>Karty informacyjne przedsięwzięcia</li>
                  <li>Raporty o oddziaływaniu przedsięwzięcia na środowisko</li>
                  <li>Prognozy oddziaływania na środowisko    dla miejscowych planów
                    zagospodarowania przestrzennego.</li>
                </ul>
              </div>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </div>
  </div>
</template>

<script>
import bg from '@/static/offer-bg.png';

export default {
  data() {
    return {
      bg,
    }
  },
  components: {
  },
  mounted() {
  }
}
</script>
