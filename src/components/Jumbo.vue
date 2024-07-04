<script>
   export default {
      data() {
         return {
            imageName: "jumbo.jpg"
         };
      },
      methods: {
         getImgPath: function(path) {
            return new URL(path, import.meta.url).href;
         }
      }
   };
</script>

<template>
   <img :src="getImgPath(`../assets/${imageName}`)">
</template>

<style scoped>

</style>