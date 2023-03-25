<template>
    <div class="messagebar">
        <div class="messagebox">
            <img class="icon-message" width="12" height="12" src="~/assets/images/icon/Icon_bell.png">
            Messages
        </div>
        <div class="arrow"></div>
        <Vue3Marquee class="marquee" :gradient="true" :gradientColor="[103, 103, 103]" :gradientWidth="`10%`">
            ระบบเติมเงินเกมส์ออนไลน์สามารถใช้งานได้ปกติแล้วนะคะ
            ลูกค้าสามารถทำการสั่งซื้อได้ด้วยตนเองผ่านระบบอัตโนมัติได้ตลอด 24 ช.ม ขอบคุณที่ใช้บริการค่ะ. &
        </Vue3Marquee>
    </div>
</template>

<script>
import { Vue3Marquee } from 'vue3-marquee'
import 'vue3-marquee/dist/style.css'

export default {
    components: {
        Vue3Marquee,
    },
}
</script>

<style>
.marquee {
    color: white;
    width: 1050px;
    height: 24px;
}

.icon-message {
    filter: invert(100%);
    justify-self: end;
    align-self: center;

}

.messagebar {
    background-color: #676767;
    height: 40px;
    justify-content: center;
    align-items: center;
    display: flex;
}

.messagebox {
    font-weight: 700;
    background-color: #8766c4;
    color: white;
    text-align: center;
    border-radius: 4px;
    width: 200px;
    height: 24px;
    margin-left: 24px;


}

.arrow {
    width: 0;
    height: 0;
    border-top: 5px solid transparent;
    border-bottom: 5px solid transparent;
    border-left: 5px solid #8766c4;
}
</style>