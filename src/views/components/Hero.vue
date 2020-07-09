<template>
    <section class="section-hero section-shaped my-0">
        <div class="shape shape-style-1 shape-primary">
            <span class="span-150"></span>
            <span class="span-50"></span>
            <span class="span-50"></span>
            <span class="span-75"></span>
            <span class="span-100"></span>
            <span class="span-75"></span>
            <span class="span-50"></span>
            <span class="span-100"></span>
            <span class="span-50"></span>
            <span class="span-100"></span>
        </div>
        <div class="container shape-container d-flex align-items-center">
            <div class="col px-0">
                <div class="row justify-content-center align-items-center">
                    <div class="col-lg-7 text-center pt-lg">
                        <p class="lead text-white mt-4 mb-5">Hello !</p>
                        
                        <p class="h1  text-white mt-4 mb-5">I'm <span class="text-info font-weight-light">Chanisara Uttamawetin</span></p>
                        <p class="h1  text-white mt-4 mb-5">Web Programmer </p>
                        <div class="btn-wrapper ">
                            <base-button tag="a"
                                         href="#/profile"
                                         class="mb-3 mb-sm-0 "
                                         type="info"
                                         >
                                Click ME
                            </base-button>
                        </div>
                    </div>
                </div>
                <div class="row align-items-center justify-content-around stars-and-coded">
                </div>
                
            </div>
        </div>
        <div class="col-lg-6 mb-lg-auto">
                    <div class="rounded shadow-lg overflow-hidden transform-perspective-right">
                        <b-carousel id="carousel1"
                                    controls
                                    indicators>
                            <!-- Text slides with image -->
                            <b-carousel-slide img-src="img/theme/img-1-1200x1000.jpg"></b-carousel-slide>
                            <b-carousel-slide img-src="img/theme/img-2-1200x1000.jpg"></b-carousel-slide>
                        </b-carousel>
                    </div>
                </div>
    </section>
    
</template>
<script>
export default {};
</script>
<style>
</style>
