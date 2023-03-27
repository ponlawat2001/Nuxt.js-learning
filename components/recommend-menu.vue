<template>
    <div class="recommend-box">
        <a href="/" class="recommend-card" v-for="item in items">
            <img :src="`~/assets/images/icon/${item.icon}`" width="70" height="70">
            {{ item.title }}
        </a>

    </div>
    <div class="recommend-box">
        <img src="https://www.termtang.com/assets/images/507044632017_s13881.png?v=2">
        <img src="https://www.termtang.com/assets/images/1385772071434_s12100.png?v=1">

    </div>
</template>

<script>
export default {
    name: 'recommendmenu',
    data: () => ({
        items: [
            {
                title: 'บัตรเติมเงิน',
                icon: 'Icon_card.png',
            },
            {
                title: 'เติมเกมออนไลน์',
                icon: 'ssdfs',
            },
            {
                title: 'เติมเงินมือถือ',
                icon: 'ssdfs',
            },
            {
                title: 'สุ่มของรางวัล',
                icon: 'ssdfs',
            },
            {
                title: 'เกมเสี่ยงโชค',
                icon: 'ssdfs',
            },
            {
                title: 'วิธีเติมเกมคุ้มๆ',
                icon: 'ssdfs',
            },
        ],
        items2: ['dsfs', 'sdfds'],
    }),

}

</script>

<style>
div.recommend-box {
    overflow: auto;
    white-space: nowrap;
    margin: 0 0 24px 0;
}

div.recommend-box a {
    display: inline-block;
    color: #6c757d;
    text-align: center;
    padding: 14px;
    text-decoration: none;
}

div.recommend-box a:hover {
    color: #6f42c1;
}

.recommend-card {
    border: 1px #6c757d;
    width: 165px;
    height: 140px;
    background-color: white;
    border-radius: 8px;
    margin: 0 6px 0 6px;

}
</style>