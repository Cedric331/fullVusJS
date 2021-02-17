<template>
   <div id="app">
      <b-navbar toggleable type="dark" variant="dark">
         <b-navbar-brand href="/">Accueil</b-navbar-brand>

         <b-navbar-toggle target="navbar-toggle-collapse">
            <template #default="{ expanded }">
               <b-icon v-if="expanded" icon="chevron-bar-up"></b-icon>
               <b-icon v-else icon="chevron-bar-down"></b-icon>
            </template>
         </b-navbar-toggle>

         <b-collapse id="navbar-toggle-collapse" is-nav>
            <b-navbar-nav class="ml-auto">
               <b-nav-item href="/about">A propos</b-nav-item>
               <b-nav-item href="#">Link 2</b-nav-item>
               <b-nav-item href="#" disabled>Disabled</b-nav-item>
            </b-navbar-nav>
         </b-collapse>
      </b-navbar>
   <div class="container">
      <router-view></router-view>
   </div>
      
   </div>
</template>

<script>
   export default {
      name: 'App',
   }
</script>