<script setup>
import { ref, onMounted } from 'vue'
import { CompromisLogo, BCard, BButton, BFooter } from '@compromis/blobby'
import Rellax from 'rellax'
import thumbnail from './assets/images/thumbnail.png'

onMounted(() => {
  const rellax = new Rellax('.rellax')
})

const title = ref("Exigim igualtat, exigim respecte - Compromís")
const description = ref("Els valencians i valencianes som els únics que paguem a territoris més rics que nosaltres. Diners que haurien d’anar a sanitat, educació, serveis socials o ocupació. La culpa és d’un sistema de finançament injust caducat des de 2014 i que els diferents governs espanyols no han volgut reformar.")
const image = ref(thumbnail)
</script>

<template>
  <div class="container">
    <Head lang="ca">
      <Title>{{ title }}</Title>
      <Meta name="description" :content="description" />
      <Meta name="keywords" content="compromis, finançament just, exigim respecte, exigim igualtat, rodalies, finanación justa, cercanías, dependencia, valencia" />
      <Meta name="robots" content="index, follow" />

      <Meta name="og:locale" content="ca" />
      <Meta name="og:type" content="website" />
      <Meta name="og:description" :content="description" />
      <Meta name="og:image" :content="image" />
      <Meta name="og:url" content="https://exigimigualtat.compromis.net" />
      <Meta name="twitter:site" content="@compromis" />
      <Meta name="twitter:card" content="summary_large_image" />
      <Meta name="twitter:title" :content="title" />
      <Meta name="twitter:description" :content="description" />
      <Meta name="twitter:image" :content="image" />
      <Meta name="twitter:url" content="https://exigimigualtat.compromis.net" />
    </Head>
    <header class="header">
      <a href="https://compromis.net" target="_blank" class="compromis-logo">
        <compromis-logo />
        <span class="visually-hidden">Compromís</span>
      </a>

      <h1 class="site-title text-6xl">
        Exigim<br class="d-md-none" /> igualtat,<br>
        exigim<br class="d-md-none" /> respecte!
      </h1>

      <b-button href="#sign">
        <img src="~assets/images/pencil.svg" alt="">
        Signa
      </b-button>
    </header>

    <main>
      <section class="card-grid">
        <b-card as="article" padding class="text-xl odd">
          <div class="icon calculator rellax" data-rellax-speed="1.15">
            <img src="~assets/images/calculator.webp" alt="">
          </div>
          <h2 class="text-gradient from-purple to-blue">Exigim finançament just</h2>
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

        <b-card as="article" padding class="text-xl even">
          <div class="icon piggy rellax" data-rellax-speed="1">
            <img src="~assets/images/piggy.webp" alt="">
          </div>
          <h2 class="text-gradient">Exigim inversions suficients</h2>
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

        <b-card as="article" padding class="text-xl odd">
          <div class="icon heart rellax" data-rellax-speed="1.25">
            <img src="~assets/images/heart.webp" alt="">
          </div>
          <h2 class="text-gradient from-magenta to-plum">
            Exigim diners per a la dependència
          </h2>
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

        <b-card as="article" padding class="text-xl even">
          <div class="icon crayons rellax" data-rellax-speed="0.75">
            <img src="~assets/images/crayons.webp" alt="">
          </div>
          <h2 class="text-gradient from-purple to-blue">Exigim que paguen el que ens deuen</h2>
          <p>
            L’Estat deu als valencians i valencianes 26.000 milions d’euros.
            Un deute que ens ofega: el pagament del deute és la conselleria
            amb més pressupost de la Generalitat, diners que no podem posar en centres de salut,
            escoles o residències. Per això exigim el pagament del deute històric
            de l’Estat amb els valencians i valencianes, tal i com s’ha fet amb altres territoris.
          </p>
        </b-card>

        <b-card as="article" padding class="text-xl odd">
          <div class="icon train rellax" data-rellax-speed="0.75">
            <img src="~assets/images/train.webp" alt="">
          </div>
          <h2 class="text-gradient">Exigim rodalies dignes</h2>
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
          <p>Per a més informació, visita <a href="https://trencancelado.com" target="_blank">trencancelado.com</a></p>
        </b-card>
      </section>

      <section aria-labelledby="sign">
        <h2 class="sign" id="sign">
          Signa per a exigir igualtat,<br>
          signa per a exigir respecte
        </h2>
        <iframe class="form rounded overflow-hidden" src="https://docs.google.com/forms/d/e/1FAIpQLSegWMSeVJp6AZ6tVzlTjuDZjFno9aw--KDHfFKn0MUXN-wl3A/viewform?embedded=true" width="100%" height="1592" frameborder="0" marginheight="0" marginwidth="0">Loading…</iframe>
      </section>
    </main>
    <b-footer campaign="Exigim igualtat, exigim respecte!" />
  </div>
</template>

<style lang="scss">
@import '@compromis/blobby/scss/blobby';

body {
  font-weight: 500;
}

.card-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 3.5rem;
  margin-top: 2rem;

  .card {
    position: relative;
    min-height: 21rem;
    display: flex;
    border-radius: 1.5rem !important;

    .card-content {
      display: flex;
      flex-direction: column;
      height: 100%;
      flex-grow: 1;
    }

    &.card-padded {
      padding: 2.25rem;
    }

    h2 {
      font-weight: 700;
      width: fit-content;
      letter-spacing: -.02em;
      padding-bottom: 1rem;
      margin-bottom: auto;
      font-size: 2.25rem;
    }

    p {
      max-width: 50ch;
    }

    &.even {
      text-align: right;
      padding-left: 200px;

      h2,
      p {
        margin-left: auto;
      }
    }

    &.odd {
      padding-right: 200px;
    }
  }

  .card p:last-child {
    margin-bottom: 0;
  }

  .icon {
    position: absolute;
    top: 55%;

    img {
      width: 200px;
      transform: translateY(-50%);
    }

    &.calculator {
      right: -2rem;
    }

    &.piggy {
      left: -4rem;

      img {
        width: 240px;
      }
    }

    &.heart {
      right: -2rem;

      img {
        transform: translateY(-50%) scaleX(-1);
      }
    }

    &.crayons {
      left: -3rem;
      top: 70%;

      img {
        width: 150px;
      }
    }

    &.train {
      top: auto;
      right: -5rem;
      bottom: -6rem;

      img {
        width: 340px;
        transform: none;
      }
    }
  }
}

.container {
  padding: 2rem;
  max-width: 1000px;
}

.header {
  .compromis-logo {
    margin-bottom: 3rem;

    svg {
      width: 200px;
    }
  }

  .site-title {
    font-weight: 500;
    padding-bottom: 1rem;
    line-height: 1;
    margin-bottom: 1.5rem;
  }
}

.sign {
  margin-top: 5rem;
  text-align: center;
}

.button-primary {
  display: inline-flex;
  background: $gradient-primary;
  color: $white;
  margin-bottom: 2rem;
  padding: .75em 2em;
  border-radius: 2rem;
  font-size: $text-xl;
  transition: .2s ease;
  align-items: center;

  img {
    height: 1em;
    margin-right: .5em;
  }

  &:hover {
    color: $white;
    text-decoration: none;
    box-shadow: $shadow-raised;
    transform: translateY(-.2em);
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

@include media-breakpoint-down(md) {
  .container {
    padding: 1rem;
  }

  .header {
    .site-title {
      font-size: 3.75rem !important;
    }
  }

  .card-grid {
    margin-top: 3rem;
    gap: 6rem;

    .card {
      &.card-padded {
        padding: 120px 1.5rem 1.5rem;
      }

      &.odd {
        padding-right: 1.5rem;
      }

      &.even {
        padding-left: 1.5rem;
        text-align: left;

        h2 {
          margin-left: 0;
        }
      }

      .icon {
        top: -2.5rem;
        left: 50%;
        right: auto;
        bottom: auto;
        transform: translate(-50%, 0) !important;

        img {
          transform: none;
          width: auto;
          height: 150px;
        }
      }
    }
  }

  .form {
    height: 2200px;
  }
}
</style>
