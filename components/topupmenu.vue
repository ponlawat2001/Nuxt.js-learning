<template>
    <span class="button-left">
        <img :width="12" src="~/assets/images/icon/Icon_right-arrow.png" class="fa fa-angle-left" />
    </span>
    <div class="topup-box">
        <Splide :options="settings">
            <SplideSlide v-for="(item, i) in items" :key="i">
                <img :src="item.image" :alt="item.title">
                <div class="topuptext">{{ item.title }}</div>
            </SplideSlide>
        </Splide>
    </div>
</template>

<script>
import { Splide, SplideSlide } from '@splidejs/vue-splide';
import '@splidejs/vue-splide/css';

export default {
    components: {
        Splide,
        SplideSlide,
    },
    data: () => ({
        settings: {
            start: 0,
            arrows: true,
            type: 'loop',
            perPage: 6,
            rewind: true,
            autoplay: true,
            speed: '1000',
            Width: '200px',
            gap: '24px',
            focus: 'left',
            pagination: false,

        },

        items: [
            {
                title: 'IQIYI',
                content: 'sdfdsf',
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
            {
                title: 'RoV Mobile MOBA',
                image: 'https://www.termtang.com/assets/images/termgame/aov-2.png?v=3'
            },

        ]
    }),
}
</script>

<style>
div.topup-box img {
    width: 170px;
}

div.topup-box .topuptext {
    color: #343a40;
    font-size: 12px;
    margin-top: 8px;
}

div.topup-box {
    margin: 8px 0 8px 0;
    width: 1200px;
}
</style>