<template>
  <div>
    <b-carousel>
      <b-carousel-item v-for="(carousel, i) in carousels" :key="i">
        <section :class="`hero is-medium is-${carousel.color}`">
          <img src="@/assets/bienvenida.jpg" alt="" />
        </section>
      </b-carousel-item>
    </b-carousel>

    <section class="section container">
      <h3 class="title">Quienes somos?</h3>
      <p class="">
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nostrum ad
        molestias eos voluptates placeat nesciunt ipsa doloribus consequatur
        possimus? Repudiandae quaerat aspernatur eius magni officiis deleniti
        dicta quasi qui facere!
      </p>

      <p>
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Aliquid soluta
        officia beatae facere consequatur perspiciatis eius quod, ea, aut ipsam
        cupiditate vel error quis nulla sed quibusdam. Nulla, quasi quaerat.
      </p>

      <b-button size="is-medium" type="is-info">Hacer Cita</b-button>
    </section>

    <section class="section container">
      <h3 class="title is-3">Nuestros Servicios</h3>
      <div class="columns is-mobile">
        <card title="Free" icon="github">
          Open source on <a href="https://github.com/buefy/buefy"> GitHub </a>
        </card>

        <card title="Responsive" icon="cellphone-link">
          <b class="has-text-grey"> Every </b> component is responsive
        </card>

        <card title="Modern" icon="alert-decagram">
          Built with <a href="https://vuejs.org/"> Vue.js </a> and
          <a href="http://bulma.io/"> Bulma </a>
        </card>

        <!-- <card title="Lightweight" icon="arrange-bring-to-front">
          No other internal dependency
        </card> -->
      </div>
    </section>

    <section class="section container">
      <h3 class="title is-3 has-text-centered">Testimonios</h3>

      <div class="columns">
        <div class="column">
          <h5>Test 1</h5>
          <p>
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quisquam,
            nihil voluptatibus? Ipsam illum accusamus quam non perspiciatis?
            Fugiat inventore vitae neque. Excepturi cumque molestias cum itaque,
            iusto nihil? Illum, totam!
          </p>
          <span>Nombre del cliente</span>
        </div>

        <div class="column">
          <h5>Test 2</h5>
          <p>
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quisquam,
            nihil voluptatibus? Ipsam illum accusamus quam non perspiciatis?
            Fugiat inventore vitae neque. Excepturi cumque molestias cum itaque,
            iusto nihil? Illum, totam!
          </p>
          <span>Nombre del cliente</span>
        </div>

        <div class="column">
          <h5>Test 3</h5>
          <p>
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quisquam,
            nihil voluptatibus? Ipsam illum accusamus quam non perspiciatis?
            Fugiat inventore vitae neque. Excepturi cumque molestias cum itaque,
            iusto nihil? Illum, totam!
          </p>
          <span>Nombre del cliente</span>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import Card from '~/components/Card'

export default {
  name: 'HomePage',

  components: {
    Card,
  },

  head: {
    title: 'Inicio - Fisioterapia Vallarta',
    meta: [
      {
        hid: 'description',
        name: 'description',
        content: 'Descripción de página web',
      },
    ],
  },

  data() {
    return {
      carousels: [
        { text: 'Slide 1', color: 'primary' },
        { text: 'Slide 2', color: 'info' },
        { text: 'Slide 3', color: 'success' },
        { text: 'Slide 4', color: 'warning' },
        { text: 'Slide 5', color: 'danger' },
      ],
    }
  },
}
</script>
