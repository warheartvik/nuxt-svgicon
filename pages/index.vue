<template>
  <div>
    <section class="container">
              Icon with svg sprite v-binding to static folder
              <com-icono-static 
              style="width: 15px; height: 15px"
              :iconName="'lupa'"
              ></com-icono-static>
    </section>    
    <!-- v-binding (to assets folder) - Doesn't work --> 
    <section class="container">
              Icon with svg sprite v-binding to assets folder
              <com-icono-assets
              style="width: 15px; height: 15px"
              :iconName="'lupa'"
              ></com-icono-assets>
    </section>  

    <section class="container">
              Icon with svg sprite in assets folder using string url
              <com-icono-string
              style="width: 15px; height: 15px"
              ></com-icono-string>
    </section>       
  </div>

</template>

<script>
import comIconoStatic from '~/components/comIconoStatic.vue'
import comIconoAssets from '~/components/comIconoAssets.vue'
import comIconoString from '~/components/comIconoString.vue'
export default {
  components: {
    'com-icono-static':comIconoStatic,
    'com-icono-assets': comIconoAssets,
    'com-icono-string': comIconoString

  }
}
</script>

<style>
.container {
  margin: 0 auto;
  display: block;
}
</style>
