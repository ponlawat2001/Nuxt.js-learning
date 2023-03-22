<template>
    <div class="menubar">
        <img src="https://www.termtang.com/assets/images/logo.png?v=4" width="150" />
        <div class="mainmenu">
            <label class="title">
                <li v-for="(item, index) in items" :key="index">
                    <NuxtLink class="linkmenu" to="/">
                        {{ item.message }}
                    </NuxtLink>
                </li>
            </label>
            <div class="navigator">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            items: [{ message: 'หน้าหลัก' }, { message: 'เกี่ยวกับเรา' }, { message: 'บัตรเติมเงิน' }, { message: 'เติมเกมออนไลน์' }, { message: 'เติมเงินมือถือ' }, { message: 'สุ่มของรางวัล' }, { message: 'เติมบัตรเครดิต' }, { message: 'คำถามที่พบบ่อย' }]
        };
    }
};

</script>

<style>
.menubar {
    background-color: white;
    /* position: fixed; */
    font-size: 14px;
    font-family: sans-serif;
    top: 0;
    left: 0;
    right: 0;
    height: 100px;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 0 20px;
    box-sizing: border-box;

}

.logo {
    width: 36px;
}

.cart {
    width: 36px;
    height: 36px;
    background-color: #f1f1f1;
    margin-left: 24px;
    padding: 2px;
    border-radius: 30px;
    display: flex;
}

.mainmenu {
    display: flex;
    margin-left: 150px;
}

.navigator {
    display: flex;
    margin-left: auto;
    padding-left: 8px;
}

.title {
    list-style: none;
    margin: 0;
    padding: 0;
    align-content: flex-end;
    display: flex;
}

.menubar li {
    padding: 0 20px;
}

a.router-link-exact-active.linkmenu {
    color: #929292;
    text-decoration: none;
}

a:hover.linkmenu {
    color: #6f42c1;
    text-decoration: none;
}
</style>