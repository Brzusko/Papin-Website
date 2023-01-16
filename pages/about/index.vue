<template>
  <div class="about">
    <div class="about--container">
      <div class="about--mobile__header">
        O Nas
      </div>
      <div class="about--image">
        <div class="about--image__pin">
          Aleksandra Papin
        </div>
        <img :src="APapin"/>
        <div class="about--mobile__info about-visible-mobile">
          Aleksandra Papin
        </div>
      </div>
      <div class="about--text">
        <p><b>Aleksandra Papin i Marek Papin</b> – absolwenci Uniwersytetu Śląskiego, na
          <b class="bold-color">Wydziale Biologii i Ochrony Środowiska</b>, oboje z kilkunastoletnim
          doświadczeniem w branży ochrony środowiska.</p>
        <img :src="PPapin" class="about-visible-mobile img-mobile-height" style="margin-bottom: 29px; margin-top: 29px;">
        <p>Z zamiłowania przyrodnicy a zawodowo związani jesteśmy z branżą
          ochrony środowiska.</p>

        <p>Sporządzamy zarówno <b class="bold-color">inwentaryzacje przyrodnicze</b>, w tym specjalistyczne
        inwentaryzacje herpetologiczne, ornitologiczne i chiropterologiczne.
        Z racji wieloletniego doświadczenia w branży środowiskowej, zakres
        naszej pracy obejmuje również sporządzanie kart informacyjnych oraz
        raportów oddziaływania na środowisko.</p>
      </div>
    </div>
    <div class="about--container">
      <div class="about--text force-position-start">
        <div class="about--marek visible-mobile">
          <img :src="MPapin"/>
          <div class="about--mobile__info about-visible-mobile">
            Marek Papin
          </div>
        </div>
        <p class="about-visible-desktop">Do każdego tematu podchodzimy indywidualnie, działamy elastycznie i
          terminowo, dostosowując się do ustalonego harmonogramu Inwestora.</p>

        <p>Dysponujemy sprzętem umożliwiającym dokonywanie i dokumentowanie
        obserwacji – <b class="bold-color">sprzęt GPS, lornetka, aparaty fotograficzne, rejestratory
        dźwięku, detektor ultradźwiękowy, posiadamy specjalistyczne
            oprogramowanie do analizy dźwięku (np. głosów nietoperzy)</b>.</p>

        <p>Wystawiam faktury w ramach prowadzonej działalności gospodarczej.</p>
        <img :src="PPapin" class="about--inner-imager about-visible-desktop"/>
      </div>
      <div class="about--image force-padding-top about-visible-desktop">
        <div class="about--image__wrapper">
          <div class="about--image__pin-2">
            Marek Papin
          </div>
          <img :src="MPapin"/>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import APapin from '@/static/2ziomek.png';
import PPapin from '@/static/panstwoPapin.png';
import MPapin from '@/static/1ziomek.png';
import ALeafes from '@/static/ap_leafes.png';
import MLeafes from '@/static/mp_leafes.png';

export default {
  data() {
    return {
      APapin,
      PPapin,
      MPapin,
      ALeafes,
      MLeafes,
    }
  },
  components: {
  },
}
</script>
