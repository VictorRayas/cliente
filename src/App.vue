<script setup>
</script>

<template>

    <b-container fluid>
      <b-row>
   
          <b-navbar toggleable="lg" type="dark" variant="info">
            <b-navbar-toggle target="navbar-nav"></b-navbar-toggle>
            <b-collapse id="navbar-nav" is-nav>
              <b-navbar-nav class="ml-auto">

                <b-nav-item href="#">
                  <b-link :to="{ name: 'inicio'}">Inicio</b-link>
                </b-nav-item>

                <b-nav-item href="#/main">
                <b-link :to="{ name: 'main'}">Main</b-link>
                </b-nav-item>

                <b-nav-item href="#">
                  <b-link :to="{ name: 'tercero'}">Tercero</b-link>
                </b-nav-item>

              </b-navbar-nav>
            </b-collapse>
          </b-navbar>

      </b-row>

      <b-row>
        <b-col sm="3">

       <b-sidebar id="sidebar"    b-sidebar shadow visible no-close-on-route-change no-header-close>
        <div class="px-3 py-2">
          <b-nav vertical class="pt-5">
           <b-navbar-nav class="ml-auto">

                <b-nav-item >
                  <b-link :to="{ name: 'inicio'}">Inicio</b-link>
                </b-nav-item>

                <b-nav-item href="#/main">
                <b-link :to="{ name: 'main'}">Main</b-link>
                </b-nav-item>

                <b-nav-item href="#">
                  <b-link :to="{ name:'tercero'}">Tercero</b-link>
                </b-nav-item>

              </b-navbar-nav>
          </b-nav>
        </div>
        </b-sidebar>
      </b-col>
      


     
      <b-col>
        <router-view> </router-view>
      </b-col>
      </b-row>
   
    </b-container>

</template>

<style scoped>
.myNav {
  background-color: rgb(158, 192, 233);
  font-family: Arial, Helvetica, sans-serif;
  border-color: rgb(2, 3, 78);
}
</style>
