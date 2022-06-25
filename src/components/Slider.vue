<template>
  <div class="slider">
    <carousel @next="next" @prev="prev">
      <carousel-slide
        v-for="(slide, index) in slides"
        :key="slide"
        :index="index"
        :visibleSlide="visibleSlide"
      >
        <img :src="slide" />
      </carousel-slide>
    </carousel>
    <!-- <h2 class="card-title">This is Exam Question 7 "Slider"</h2> -->
  </div>
</template>

<script>
import Carousel from "../components/Carousel.vue";
import CarouselSlide from "../components/CarouselSlide.vue";
export default {
  data() {
    return {
      slides: [
        "https://picsum.photos/id/240/1168/500",
        "https://picsum.photos/id/241/1168/500",
        "https://picsum.photos/id/242/1168/500",
      ],
      visibleSlide: 0,
    };
  },
  computed: {
    slidesLen() {
      return this.slides.lenght;
    },
  },
  methods: {
    next() {
      console.log("next");
      if (this.visibleSlide >= this.slidesLen - 1) {
        this.visibleSlide = 0;
      } else {
        this.visibleSlide++;
      }
    },
    prev() {
      console.log("prev");
      if (this.visibleSlide <= 0) {
        this.visibleSlide = this.slidesLen - 1;
      } else {
        this.visibleSlide--;
      }
    },
  },
  components: {
    Carousel,
    CarouselSlide,
  },
};
</script>

<style lang="sass" scoped>
.slider
    display: flex
    justify-content: center
</style>
