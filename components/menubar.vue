<template>
    <div class="menubar">
        <img src="~/assets/images/logo/logo.png" width="100px" />
        <div class="mainmenu">
            <label class="title">
                <slot></slot>
            </label>
            <div class="navigator">
            </div>
        </div>
    </div>
</template>

<style>
.menubar {
    background-color: white;
    position: fixed;
    font-size: 14px;
    font-family: sans-serif;
    top: 0;
    left: 0;
    right: 0;
    height: 100px;
    display: flex;
    align-items: center;
    justify-content: space-between;
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

a.nuxt-link-exact-active {
    color: #929292;
}

a:hover {
    color: #6f42c1;
    text-decoration: none;
}
</style>