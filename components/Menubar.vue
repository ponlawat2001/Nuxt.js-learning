<template>
    <div class="menubar">
        <img class="logo" src="~/assets/images/logo/logo.png" alt="Logo" />

        <div class="mainmenu">
            <label class="title">
                <slot></slot>
            </label>
        </div>
        <div class="navigator">
            <img class="navigatorlogo" src="~/assets/images/logo/facebook.svg" alt="Facebook" />
            <img class="navigatorlogo" src="~/assets/images/logo/google.svg" alt="Google" />
            <img class="navigatorlogo" src="~/assets/images/logo/twitter.svg" alt="twitter" />
            <img class="navigatorlogo" src="~/assets/images/logo/apple.svg" alt="Apple" />
        </div>
        <div class="cart">
            <img class="navigatorlogo" src="~/assets/images/logo/paperbag.svg" alt="Paperbag" />
        </div>
        <img class="navigatorlogo" style="margin-left: 24px;" src="~/assets/images/logo/magnifier.svg" alt="Apple" />
    </div>
</template>

<style>
.menubar {
    background-color: white;
    position: fixed;
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

.navigatorlogo {
    width: 16px;
    margin-left: 8px;
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
    margin-right: auto;
}

.navigator {
    display: flex;
    margin-left: auto;
}

.title {
    list-style: none;
    margin: 0;
    padding: 0;
    display: flex;
}

.menubar li {
    padding: 0 20px;
}
</style>