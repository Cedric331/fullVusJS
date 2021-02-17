<template>
   <div>
         <h1>Bienvenue</h1>
         <div class="row mt-5">
            <Card title="Star Wars" content="Test" image="starwars.jpg"/>
            <Card title="Vikings" content="Test" image="vikings.jpg"/>
            <Card title="Espace" content="Test" image="espace.jpg"/>
         </div>
   </div>
</template>


<script>
import Card from "@/components/Card"

export default {
   components: {
      Card,
   },
}
</script>
