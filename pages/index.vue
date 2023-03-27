<template>
    <center>
        <div>
            <carousel />
            <messagebar />
            <div class="recommend-menu">
                <div class="item-recommend-menu">เมนูแนะนำ</div>
                <div class="item-recommend-menu sharebutton">
                    <img class="icon-sharebutton" width="12" height="12" src="~/assets/images/icon/Icon_facebook.png">
                    แชร์ 7.2 พัน
                </div>
            </div>
            <recommendmenu />
            <div class="topup-menu">
                <div class="item-topup-menu">เติมเกมออนไลน์</div>
                <div class="item-topup-menu-sub">
                    <div style="margin-right: 16px;">GAME ONLINE TOP UP</div>
                    <div class="topup-total"><a href="/">ดูทั้งหมด</a></div>
                </div>
            </div>
            <topupmenu />
        </div>
    </center>
</template>

<style>
div.topup-total a {
    font-size: 10px;
    color: white;
    text-decoration: none;

}

div.topup-total {
    width: 50px;
    height: 25px;
    background-color: #343a40;
    border-radius: 16px;
    text-align: center;

}

.item-topup-menu-sub {
    width: 1200px;
    height: 30px;
    font-size: 14px;
    color: #6c757d;
    text-align: start;
    display: flex;
    align-items: center;

}

.item-topup-menu {
    width: 1200px;
    height: 30px;
    font-size: 24px;
    color: #343a40;
    text-align: start;
    margin: 8px 0 0 0;
}

.icon-sharebutton {
    border-radius: 8px;
    filter: invert(100%);

}

.sharebutton {
    font-weight: 200;
    font-size: 12px;
    background-color: #007bff;
    color: white;
    text-align: center;
    border-radius: 4px;
    width: 100px;
    height: 24px;
    margin-left: 24px;
}

.recommend-menu {
    width: 1200px;
    height: 30px;
    font-size: 24px;
    color: #343a40;
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin: 8px 0 16px 0;
}
</style>

<script>
import carousel from '~~/components/carousel.vue';
import messagebar from '~~/components/messagebar.vue';
import recommendmenu from '~~/components/recommend-menu.vue';
import topupmenu from '~~/components/topupmenu.vue'

export default {
    name: 'index',
    components: {
        carousel,
        messagebar,
        recommendmenu,
        topupmenu,
    }
}

</script>



