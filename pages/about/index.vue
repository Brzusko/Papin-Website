<template>
  <div class="about">
    <div class="about--container">
      <div class="about--image">
        <div class="about--image__pin">
          Aleksandra Papin
        </div>
        <img :src="APapin"/>
      </div>
      <div class="about--text">
        <p><b>Aleksandra Papin i Marek Papin</b> – absolwenci Uniwersytetu Śląskiego, na
          <b class="bold-color">Wydziale Biologii i Ochrony Środowiska</b>, oboje z kilkunastoletnim
          doświadczeniem w branży ochrony środowiska.</p>

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
        <p>Do każdego tematu podchodzimy indywidualnie, działamy elastycznie i
          terminowo, dostosowując się do ustalonego harmonogramu Inwestora.</p>

        <p>Dysponujemy sprzętem umożliwiającym dokonywanie i dokumentowanie
        obserwacji – <b class="bold-color">sprzęt GPS, lornetka, aparaty fotograficzne, rejestratory
        dźwięku, detektor ultradźwiękowy, posiadamy specjalistyczne
            oprogramowanie do analizy dźwięku (np. głosów nietoperzy)</b>.</p>

        <p>Pracujemy na umowę zlecenie lub umowę o dzieło, co czyni nas bardziej
          konkurencyjnymi na rynku.</p>
        <img :src="PPapin" class="about--inner-imager"/>
      </div>
      <div class="about--image force-padding-top">
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
