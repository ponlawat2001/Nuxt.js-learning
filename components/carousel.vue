<template>
    <vueper-slides :dragging-distance="100" :autoplay="true" :fixed-height="true" :arrows="false">
        <vueper-slide v-for="(slide, i) in slides" :key="i" :image="slide.image" :title="slide.title"
            :content="slide.content">
        </vueper-slide>
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
                title: 'บัตรเติมเกมออนไลน์',
                content: 'ด้วยระบบอัตโนมัติตลอด 24 ชม. ถูกกว่าเติมเอง 100%',
                image: 'https://www.termtang.com/assets/images/slide/1.jpg'

            },
            {
                title: 'เติมเงินรวดเร็วทันใจ',
                content: 'ด้วยระบบอัตโนมัติ 5 ช่องทาง สะดวก รวดเร็ว ปลอดภัย',
                image: 'https://www.termtang.com/assets/images/slide/2.jpg'

            },
            {
                title: 'ระบบสุ่มรางวัลใหม่',
                content: 'สุ่มรางวัลเริ่มต้นเพียง 10 เครดิตเท่านั้น',
                image: 'https://www.termtang.com/assets/images/slide/3.jpg'

            }
        ]
    })
}
</script>

<style>
.vueperslide__title {
    font-size: 36px;
    font-weight: 600;
    color: white;
    position: absolute;
    top: 40%;
    left: 10%;
    z-index: 10;
}

.vueperslide__content {
    font-size: 16px;
    color: white;
    position: absolute;
    top: 47%;
    left: 10%;
    z-index: 10;
}

.vueperslides--fixed-height {
    height: 500px;
}

.slidetext {
    text-align: center;
    color: black;
}

.vueperslides__bullet .default {
    background-color: rgba(0, 0, 0, 0.3);
    border: none;
    box-shadow: none;
    transition: 0.3s;
    width: 10px;
    height: 10px;
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