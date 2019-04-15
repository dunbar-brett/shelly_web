<template>
    <section id="main-slideshow" class="carousel slide"
             data-ride="carousel">
        <ol class="carousel-indicators">
            <!-- repeat this -->
            <li data-target="#main-slideshow"
                data-slide-to="0"
                class="active"></li>
            <li data-target="#main-slideshow"
                data-slide-to="1"></li>
        </ol>
        <div class="carousel-inner sjw-carousel-inner" role="listbox">
            <!-- repeat this -->
            <div class="carousel-item active">
                <img src="~/assets/images/banner/squished-face.png"
                     class="d-block w-100" alt="First Slide">
            </div>

            <div class="carousel-item">
                <img src="~/assets/images/banner/mountain.png"
                     class="d-block w-100" alt="Second Slide">
            </div>
            <!-- controls -->
            <a href="#main-slideshow" 
               class="carousel-control-prev"
               role="button"
               data-slide="prev">
                <span class="carousel-control-prev-icon"></span>
                <span class="sr-only">Previous</span>
            </a>
            <a href="#main-slideshow" 
               class="carousel-control-next"
               role="button"
               data-slide="next">
                <span class="carousel-control-next-icon"></span>
                <span class="sr-only">NExt</span>
            </a>
        </div>
    </section>
</template>

<script>

export default {
    data() {
        return {
            images: [
                '~/assets/images/banner/squished-face.png',
                '~/assets/images/banner/mountain.png'
            ]
        };
    }
};
</script>
<style lang="scss">
#main-slideshow {
    min-width: 100%;
    margin: 0 -10.3rem;

    .sjw-carousel-inner {
        min-height: 65rem;  
        max-height: 65rem;
    }
}
</style>

