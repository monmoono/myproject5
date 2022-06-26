<template>
  <div v-show="visibleSlide === index" class="carousel-slide">
    <slot></slot>
  </div>
</template>

<script>
export default {
  props: ["visibleSlide", "index"],
  data() {
 
  },

};
</script>

<style lang="sass" scoped>
.carousel-slide
    position: absolute
    top: 18px
    left: 0
    bottom: 0
    right: 0

.carousel-slide img
    width: 100%
    height: 100%

.carousel-img
    border: 2px solid #817f7fee
    padding: 5px
    margin: 0px
    box-shadow: 2px 3px 9px 3px #0000001f
</style>
