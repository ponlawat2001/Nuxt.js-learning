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
        </div>
    </center>
</template>

<style>
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

export default {
    name: 'index',
    components: {
        carousel,
        messagebar,
        recommendmenu,
    }
}

</script>



