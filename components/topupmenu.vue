<template>
    <div class="topup-box">
        <vueper-slides class="no-shadow" :slide-ratio="1 / 4" :visible-slides="6" slide-multiple :gap="5"
            :dragging-distance="100" :autoplay="true" :fixed-height="true" :arrows="false"
            :breakpoints="{ 800: { visibleSlides: 2, slideMultiple: 2 } }">
            <vueper-slide class="topup-card" v-for="item in items" :key="i" :image="item.image" :title="item.title"
                :content="item.content">
            </vueper-slide>
        </vueper-slides>
    </div>
</template>

<script>
import { VueperSlides, VueperSlide } from 'vueperslides'
import 'vueperslides/dist/vueperslides.css'
export default {

    components: { VueperSlides, VueperSlide },

    data: () => ({
        items: [
            {
                title: 'IQIYI',
                image: 'https://www.termtang.com/assets/images/termgame/IQIYI.png'
            },
            {
                title: 'RoV Mobile MOBA',
                image: 'https://www.termtang.com/assets/images/termgame/aov-2.png?v=3'
            },
            {
                title: 'RoV Mobile MOBA',
                image: 'https://www.termtang.com/assets/images/termgame/aov-2.png?v=3'
            },
            {
                title: 'RoV Mobile MOBA',
                image: 'https://www.termtang.com/assets/images/termgame/aov-2.png?v=3'
            },
            {
                title: 'RoV Mobile MOBA',
                image: 'https://www.termtang.com/assets/images/termgame/aov-2.png?v=3'
            },
            {
                title: 'RoV Mobile MOBA',
                image: 'https://www.termtang.com/assets/images/termgame/aov-2.png?v=3'
            },

        ]
    }),
}
</script>

<style>
div.topup-box {
    margin: 8px 0 8px 0;
    width: 1200px;
}

div.topup-box .vueperslide__title {
    font-size: 12px;
    font-weight: 600;
    color: gray;
    position: absolute;
    top: 0%;
}

div.topup-box .vueperslide__content {
    font-size: 16px;
    color: white;
    position: absolute;
}

div.topup-box .vueperslides--fixed-height {
    height: 190px;
}

div.topup-box .slidetext {
    text-align: center;
    color: black;
}
</style>