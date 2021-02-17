<template>

   <div class="col-md-6 mb-4">
      <div class="card">
         <div class="view overlay">
            <img :src="'./image/'+image" style="min-height:350px;max-height:350px;" class="card-img-top" alt="">
            <a>
               <div class="mask rgba-white-slight waves-effect waves-light"></div>
            </a>
         </div>

         <div class="card-body">

            <h4 class="card-title"><strong>{{title}}</strong></h4>
            <hr>

            <p class="card-text mb-3">{{content}}
            </p>
            <p class="font-small font-weight-bold dark-grey-text mb-1"><i class="far fa-clock-o"></i>
               27/08/2019</p>
            <p class="font-small grey-text mb-0">Anna Smith</p>
            <p class="text-right mb-0 font-small font-weight-bold"><a>read more <i class="fas fa-angle-right"></i></a>
            </p>
         </div>

      </div>
   </div>

</template>



<script>
   export default {
      props: {
         title: { type: String, default: ''},
         content: { type: String, default: ''},
         image: { type: String, default: ''},
      },
      mounted() {
         console.log(this.image)
      },
   }
</script>