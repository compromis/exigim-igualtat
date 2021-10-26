<script setup>
import { CompromisLogo, BCard } from '@compromis/blobby'
</script>

<template>
  <div class="container">
    <a href="https://compromis.net" target="_blank" class="compromis-logo">
      <compromis-logo />
    </a>

    <h1 class="site-title text-6xl">
      Exigim igualtat,<br>
      exigim respecte!
    </h1>

    <div class="card-grid">
      <b-card padding class="text-lg">
        <h2 class="text-gradient from-purple to-blue">Exigim inversions suficients</h2>
        <p>
          Els valencians i valencianes hem rebut menys
          inversions de l’Estat de les que ens toquen segons la
          nostra població. A més, de les inversions
          pressupostades només s’acaben executant una
          xicoteta part.
        </p>
        <p>
          Per això exigim inversions suficients i que
          s’executen les inversions previstes. Inversions com
          la connexió en rodalies de l’aeroport de l’Altet, el
          túnel passant ferroviari de València, el cost de les
          dessaladores de les comarques de Castelló o la
          connexió València-Alacant pel tren de la costa.
        </p>
      </b-card>

      <b-card padding class="text-lg">
        <h2 class="text-gradient">Exigim Finançament Just</h2>
        <p>
          Els valencians i valencianes som els únics que
          paguem a territoris més rics que nosaltres. Diners
          que haurien d’anar a sanitat, educació, serveis
          socials o ocupació. La culpa és d’un sistema de
          finançament injust caducat des de 2014 i que els
          diferents governs espanyols no han volgut
          reformar.
        </p>
        <p>
          Per això exigim la reforma immediata del sistema
          de finançament i la posada en marxa d’un
          mecanisme que ens compense i garantisca que
          tenim la mateixa capacitat de finançar els serveis
          públics que altres territoris
        </p>
      </b-card>

      <b-card padding class="text-lg">
        <h2 class="text-gradient from-magenta to-plum">Exigim Rodalies Dignes</h2>
        <p>
          La falta d’inversió i la nefasta gestió en el servei ha
          provocat que les rodalies valencianes siguen líders
          en retards i cancel·lacions. Si vas en tren mai saps
          quan arribaràs.
        </p>
        <p>
          Per això exigim un pla de xoc amb inversions per a
          millorar el servei i que transferisquen la seua gestió
          als valencians i valencianes.
        </p>
      </b-card>

      <b-card padding class="text-lg">
        <div class="icon">👵</div>
        <h2>Exigim diners per a la dependència</h2>
        <p>
          La Llei marca que l’Estat ha de pagar la meitat del
          cost de les polítiques de dependència, però
          actualment només arriba al 16%. La resta l’ha de
          posar la Generalitat.
        </p>
        <p>
          Per això exigim que l’Estat complisca la llei i aporte
          els 700 milions d’euros que falten per a continuar
          millorant l’atenció a les persones en situació de
          dependència.
        </p>
      </b-card>
    </div>

    <h2>Signa per a exigir igualtat, signa per a exigir respecte</h2>
    <iframe></iframe>
  </div>
</template>

<style lang="scss">
@import './node_modules/@compromis/blobby/scss/blobby';

.card-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 2rem;

  .card {
    position: relative;

    h2 {
      font-weight: 500;
      width: fit-content;
    }
  }

  .card p:last-child {
    margin-bottom: 0;
  }

  .icon {
    position: absolute;
    top: -2rem;
    right: -2rem;
    font-size: 8rem;
  }
}

.container {
  padding: 2rem;
}

.site-title {
  font-weight: 500;
  padding-bottom: 1rem;
  line-height: 1.1;
}

.compromis-logo {
  svg {
    width: 200px;
  }
}

.from-purple {
  --gradient-start: #5c439a;
}

.to-blue {
  --gradient-end: #50b2e4;
}

.from-magenta {
  --gradient-start: #db2b60;
}

.to-plum {
  --gradient-end: #90298b;
}
</style>
