<script setup>
import { ref, onMounted } from 'vue'
import { CompromisLogo, BCard, BButton, BFooter } from '@compromis/blobby'
import Rellax from 'rellax'
import thumbnail from '../assets/images/thumbnail.png'

onMounted(() => {
  const rellax = new Rellax('.rellax')
})

const title = ref("Exigimos igualdad, exigimos respeto - Compromís")
const description = ref("Los valencianos y valencianas somos los únicos que pagamos a territorios más ricos que nosotros. Dinero que debería ir a sanidad, educación, servicios sociales o empleo...")
const image = ref('https://exigimigualtat.compromis.net' + thumbnail)
</script>

<template>
  <div>
    <Head lang="es">
      <Title>{{ title }}</Title>
      <Meta name="description" :content="description" />
      <Meta name="keywords" content="compromis, financiación justa, altet, cercanías, dependencia, valencia, alicante, aeropuerto" />
      <Meta name="robots" content="index, follow" />

      <Meta name="og:locale" content="ca" />
      <Meta name="og:type" content="website" />
      <Meta name="og:description" :content="description" />
      <Meta name="og:image" :content="image" />
      <Meta name="og:url" content="https://exigimigualtat.compromis.net/cas" />
      <Meta name="twitter:site" content="@compromis" />
      <Meta name="twitter:card" content="summary_large_image" />
      <Meta name="twitter:title" :content="title" />
      <Meta name="twitter:description" :content="description" />
      <Meta name="twitter:image" :content="image" />
      <Meta name="twitter:url" content="https://exigimigualtat.compromis.net/cas" />
    </Head>
    <header class="header">
      <div class="d-flex">
        <a href="https://compromis.net" target="_blank" class="compromis-logo">
          <compromis-logo />
          <span class="visually-hidden">Compromís</span>
        </a>
        <nuxt-link to="/" class="link-muted-to-black language-link">Valencià</nuxt-link>
      </div>

      <h1 class="site-title text-6xl">
        Exigimos<br class="d-md-none" /> <span class="text-gradient from-purple to-blue">igualdad</span>,<br>
        exigimos<br class="d-md-none" /> <span class="text-gradient">respeto</span>
      </h1>

      <b-button href="#sign">
        <img src="~assets/images/pencil.svg" alt="">
        Firmar
      </b-button>
    </header>

    <main>
      <section class="card-grid">
        <b-card as="article" padding class="text-xl odd">
          <div class="icon calculator rellax" data-rellax-speed="1.15">
            <img src="~assets/images/calculator.webp" alt="">
          </div>
          <h2 class="text-gradient from-purple to-blue">Exigimos una financiación justa</h2>
          <p>
            Los valencianos y valencianas somos los únicos que pagamos a territorios más ricos que nosotros. Dinero que debería ir a sanidad, educación, servicios sociales o empleo. La culpa es de un sistema de financiación injusto caducado desde 2014 y que los distintos gobiernos españoles no han querido reformar.
          </p>
          <p>
            Por eso exigimos la reforma inmediata del sistema de financiación y un mecanismo que nos compense y garantice que tenemos la misma capacidad de financiar los servicios públicos que otros territorios.
          </p>
        </b-card>

        <b-card as="article" padding class="text-xl even">
          <div class="icon piggy rellax" data-rellax-speed="1">
            <img src="~assets/images/piggy.webp" alt="">
          </div>
          <h2 class="text-gradient">Exigim inversions suficients</h2>
          <p>
            Los valencianos y valencianas hemos recibido menos
             inversiones del Estado de las que nos tocan según
             nuestra población. Además, de las inversiones
             presupuestadas sólo se acaba ejecutando una
             pequeña parte.
          </p>
          <p>
            Por eso exigimos inversiones suficientes y que
            se ejecuten las inversiones previstas. Inversiones como
            la conexión en cercanías del aeropuerto del Altet, el
            túnel pasante ferroviario de València, el coste de las
            desaladoras de las comarcas de Castellón o la
            conexión Valencia-Alicante por el tren de la costa.
          </p>
        </b-card>

        <b-card as="article" padding class="text-xl odd">
          <div class="icon heart rellax" data-rellax-speed="1.25">
            <img src="~assets/images/heart.webp" alt="">
          </div>
          <h2 class="text-gradient from-magenta to-plum">
            Exigimos cumplir la ley de dependencia
          </h2>
          <p>
            La Ley marca que el Estado debe pagar la mitad del coste de las políticas de dependencia, pero actualmente sólo llega al 16%. El resto debemos ponerlo la Generalitat.
          </p>
          <p>
            Por eso, exigimos que el Estado deje de incumplir la ley y aporte los 700 millones de euros que nos debe, para seguir mejorando la atención a las personas en situación de dependencia.
          </p>
        </b-card>

        <b-card as="article" padding class="text-xl even">
          <div class="icon crayons rellax" data-rellax-speed="0.75">
            <img src="~assets/images/crayons.webp" alt="">
          </div>
          <h2 class="text-gradient from-purple to-blue">Exigimos que paguen lo que nos deben</h2>
          <p>
            El Estado debe a los valencianos y valencianas 26.000 millones de euros. Una deuda que nos ahoga: el pago de la deuda es la conselleria con mayor presupuesto de la Generalitat, dinero que no podemos poner en centros de salud, escuelas o residencias. Por eso, exigimos el pago de la deuda histórica del Estado con los valencianos y valencianas, tal y como se ha hecho con otros territorios.
          </p>
        </b-card>

        <b-card as="article" padding class="text-xl odd">
          <div class="icon train rellax" data-rellax-speed="0.75">
            <img src="~assets/images/train.webp" alt="">
          </div>
          <h2 class="text-gradient">Exigimos cercanías dignos y sostenibles</h2>
          <p>
            La falta de inversión y la nefasta gestión en el servicio ha provocado que las cercanías valencianas sean líderes en retrasos y cancelaciones. No se puede luchar contra la emergencia climática boicoteando el transporte público más sostenible y vertebrador que tenemos.</p>
          <p>
            Por eso, exigimos un plan de choque con inversiones para mejorar el servicio, crear nuevas líneas, abaratar precios y transferir la gestión a la Generalitat.
          </p>
          <p>Para más información, visita <a href="https://trencancelado.com" target="_blank">trencancelado.com</a></p>
        </b-card>
      </section>

      <section aria-labelledby="sign">
        <h2 class="sign" id="sign">
          Firma para exigir igualdad,<br>
          firma para exigir respeto
        </h2>
        <iframe class="form rounded overflow-hidden" src="https://docs.google.com/forms/d/e/1FAIpQLSegWMSeVJp6AZ6tVzlTjuDZjFno9aw--KDHfFKn0MUXN-wl3A/viewform?embedded=true" width="100%" height="2300" frameborder="0" marginheight="0" marginwidth="0">Loading…</iframe>
      </section>
    </main>
    <b-footer campaign="Exigim igualtat, exigim respecte!" />
  </div>
</template>
