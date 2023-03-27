<template>
    <div class="topup-box">
        <vueper-slides class="topup-card" :dragging-distance="100" :autoplay="true" :fixed-height="true" :arrows="false">
            <vueper-slide v-for="item in items" :key="i" :image="item.image" :title="item.title" :content="item.content">
            </vueper-slide>
        </vueper-slides>
    </div>
</template>

<script>
export default {
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
    overflow: auto;
    width: 1200px;
    white-space: nowrap;
    margin: 8px 0 24px 0;
}

div.topup-box a {
    display: inline-block;
    color: #6c757d;
    text-align: center;
    text-decoration: none;
}

div.topup-box a:hover {
    color: #6f42c1;
}

.topup-card {
    border: 1px #6c757d;
    border-radius: 8px;
    margin: 0 6px 0 6px;

}
</style>