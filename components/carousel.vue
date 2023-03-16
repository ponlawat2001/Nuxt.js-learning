<template>
    <div id="carouselExampleIndicators" class="carousel slide" data-bs-ride="carousel" data-bs-pause="false">
        <div class="carousel-indicators">
            <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active"
                aria-current="true" aria-label="Slide 1">
                <span></span>
            </button>
            <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1" aria-label="Slide 2">
                <span></span>
            </button>
            <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2" aria-label="Slide 3">
                <span></span>
            </button>
        </div>
        <div class="carousel-inner">
            <div class="carousel-item active">
                <img src="~/assets/images/slider/slider_1.jpeg" class="d-block w-100" alt="...">
            </div>
            <div class="carousel-item">
                <img src="~/assets/images/slider/slider_2.jpeg" class="d-block w-100" alt="...">
            </div>
            <div class="carousel-item">
                <img src="~/assets/images/slider/slider_3.jpeg" class="d-block w-100" alt="...">
            </div>
        </div>

    </div>
</template>
<style>
.carousel-indicators [data-bs-target] {
    position: relative;
    width: 16px;
    height: 16px;
    border: none;
    margin-right: 8px;
    margin-left: 8px;
    border-radius: 24px;
    background-color: black;

}

.carousel-indicators .active {
    background-color: orange;
}
</style>



