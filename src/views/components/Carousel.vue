<template>
    <section class="section section-lg section-shaped overflow-hidden my-0">
        <div class="shape shape-style-1 shape-default shape-skew">
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
        </div>
        <div class="container py-0 pb-lg">
            <div class="row justify-content-between align-items-center">
                <div class="col-lg-5 mb-5 mb-lg-0">
                    <h1 class="text-white font-weight-light">Activities and Volunteer camp</h1>
                    <p class="lead text-white mt-4">Photos of some of the activities that I attended during my bachelor's degree.</p>
                    <a href="#/profile"
                       class="btn btn-white mt-4">View Proflie</a>
                </div>
                <div class="col-lg-6 mb-lg-auto">
                    <div class="rounded shadow-lg overflow-hidden transform-perspective-right">
                        <b-carousel id="carousel1"
                                    controls
                                    indicators>
                            <!-- Text slides with image -->
                            <b-carousel-slide img-src="img/theme/1.jpg"></b-carousel-slide>
                            <b-carousel-slide img-src="img/theme/2.jpg"></b-carousel-slide>
                            <b-carousel-slide img-src="img/theme/3.jpg"></b-carousel-slide>
                            <b-carousel-slide img-src="img/theme/4.jpg"></b-carousel-slide>
                            <b-carousel-slide img-src="img/theme/5.jpg"></b-carousel-slide>
                            <b-carousel-slide img-src="img/theme/6.jpg"></b-carousel-slide>
                            <b-carousel-slide img-src="img/theme/7.jpg"></b-carousel-slide>
                            <b-carousel-slide img-src="img/theme/9.jpg"></b-carousel-slide>
                            <b-carousel-slide img-src="img/theme/10.jpg"></b-carousel-slide>
                        </b-carousel>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
import { BCarousel } from "bootstrap-vue/esm/components/carousel/carousel";
import { BCarouselSlide } from "bootstrap-vue/esm/components/carousel/carousel-slide";

export default {
  components: {
    BCarousel,
    BCarouselSlide
  }
};
</script>
<style>
</style>
