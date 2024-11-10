<template>
  <q-page class="flex flex-center">
    <!-- <img
      alt="Quasar logo"
      src="~assets/quasar-logo-vertical.svg"
      style="width: 200px; height: 200px"
    > -->
    <CardsActions/>
  </q-page>
</template>

<script setup>
import CardsActions from 'components/CardsActions.vue'

defineOptions({
  name: 'IndexPage'
});
</script>
