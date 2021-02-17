<template>
   <div id="app">
  <b-navbar toggleable type="dark" variant="dark">
    <b-navbar-brand href="#">NavBar</b-navbar-brand>

    <b-navbar-toggle target="navbar-toggle-collapse">
      <template #default="{ expanded }">
        <b-icon v-if="expanded" icon="chevron-bar-up"></b-icon>
        <b-icon v-else icon="chevron-bar-down"></b-icon>
      </template>
    </b-navbar-toggle>

    <b-collapse id="navbar-toggle-collapse" is-nav>
      <b-navbar-nav class="ml-auto">
        <b-nav-item href="#">Link 1</b-nav-item>
        <b-nav-item href="#">Link 2</b-nav-item>
        <b-nav-item href="#" disabled>Disabled</b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>

<div class="container">
      <h1>Bienvenue</h1>

      <div class="row mt-5">
         <div class="col-4">
            <b-card no-body class="overflow-hidden" style="max-width: 540px;">
               <b-row no-gutters>
                  <b-col md="6">
                     <b-card-img src="./assets/image/starwars.jpg" alt="Image" class="rounded-0">
                     </b-card-img>
                  </b-col>
                  <b-col md="6">
                     <b-card-body title="Star Wars">
                        <b-card-text>
                           Star wars
                        </b-card-text>
                     </b-card-body>
                  </b-col>
               </b-row>
            </b-card>
         </div>

         <div class="col-4">
            <b-card no-body class="overflow-hidden" style="max-width: 540px;">
               <b-row no-gutters>
                  <b-col md="6">
                     <b-card-img src="./assets/image/vikings.jpg" alt="Image" class="rounded-0">
                     </b-card-img>
                  </b-col>
                  <b-col md="6">
                     <b-card-body title="Vikings">
                        <b-card-text>
                           This is a wider card with supporting text as a natural lead-in to additional content.
                           This content is a little bit longer.
                        </b-card-text>
                     </b-card-body>
                  </b-col>
               </b-row>
            </b-card>
         </div>

         <div class="col-4">
            <b-card no-body class="overflow-hidden" style="max-width: 540px;">
               <b-row no-gutters>
                  <b-col md="6">
                     <b-card-img src="https://picsum.photos/400/400/?image=20" alt="Image" class="rounded-0">
                     </b-card-img>
                  </b-col>
                  <b-col md="6">
                     <b-card-body title="Espace">
                        <b-card-text>
                           This is a wider card with supporting text as a natural lead-in to additional content.
                           This content is a little bit longer.
                        </b-card-text>
                     </b-card-body>
                  </b-col>
               </b-row>
            </b-card>
         </div>
      </div>
   </div>
   </div>
</template>

<script>
   export default {
      name: 'App',

   }
</script>