import { default } from '../layouts/default.vue';
<template>
  <section class="section">
    <h2 class="title is-3 has-text-grey">Titulo 2</h2>
    <h3 class="subtitle is-6 has-text-grey">Hola Como estas</h3>
  </section>
</template>

<script>
export default {
  name: 'About',

  components: {},

  head() {
    return {
      title: 'Hols soy un titulo',
      meta: [
        {
          description: 'hola soy una descripcion',
        },
      ],
    }
  },
}
</script>
