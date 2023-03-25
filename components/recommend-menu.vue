<template>
    <div class="recommend-box">
        <a href="/" class="recommend-card" v-for="item in items">
            <img src="~/assets/images/icon/Icon_creditcard.png" width="70" height="70">
            {{ item.title }}
        </a>

    </div>
    <div class="recommend-box">
        <a href="/" class="recommend-card" v-for="item2 in items2">
            {{ item2 }}
        </a>
    </div>
</template>

<script>
export default {

    data: () => ({
        items: [
            {
                title: 'บัตรเติมเงิน',
                icon: '~/assets/images/icon/Icon_creditcard.png',
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