<template>
    <vueper-slides :dragging-distance="100" :autoplay="true" :arrows="false">
        <vueper-slide v-for="(slide, i) in slides" :key="i" :image="slide.image" :title="slide.title"
            :content="slide.content" />
    </vueper-slides>
</template>

<script>
import { VueperSlides, VueperSlide } from 'vueperslides'
import 'vueperslides/dist/vueperslides.css'


export default {
    components: { VueperSlides, VueperSlide },
    data: () => ({
        slides: [
            {
                title: 'Slide #1',
                content: 'Slide 1 content.',
                image: 'https://www.termtang.com/assets/images/promotion/1.jpg'

            },
            {
                title: 'Slide #2',
                content: 'Slide 2 content.',
                image: 'https://www.termtang.com/assets/images/promotion/2.jpg'

            },
            {
                title: 'Slide #3',
                content: '<h1>Slide 3 content.</h1>',
                image: 'https://www.termtang.com/assets/images/promotion/3.jpg'

            }
        ]
    })
}
</script>

<style>
.slidetext {
    text-align: center;
    color: black;
}

.vueperslides__bullet .default {
    background-color: rgba(0, 0, 0, 0.3);
    border: none;
    box-shadow: none;
    transition: 0.3s;
    width: 16px;
    height: 16px;
}

.vueperslides__bullet--active .default {
    background-color: orange;
}

.vueperslides__bullet span {
    display: block;
    color: #fff;
    font-size: 10px;
    opacity: 0.8;
}
</style>