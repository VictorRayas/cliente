<template>
  <div>
    <b-breadcrumb :items="items"></b-breadcrumb>
    <p>Inicio</p>
    <b-button :to="{ name: 'reservaVuelos'}" variant="info">Reservas de Vuelos</b-button>
    <b-button :to="{ name: 'vuelosDisponibles'}" variant="success" >Vuelos Disponibles</b-button>
    <b-button :to="{ name: 'vuelosCancelados'}" variant="danger" >Vuelos Cancelados</b-button>

    <!-- <b-link :to="{name:'inicio'}">Siguiente</b-link> -->
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [   ],
    };
  },
};
</script>

<style>
</style>