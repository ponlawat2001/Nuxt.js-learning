<template>
    <div class="login">
        <img class="icon-login" width="14" height="14" src="~/assets/images/icon/Icon_facebook.png" />
        <NuxtLink class="logintext-left" to="/">เวลาทำการ 10:00-22:00</NuxtLink>

        <img class="icon-login" width="14" height="14" src="~/assets/images/icon/Icon_lock.png" />
        <NuxtLink class="logintext" to="/">เข้าสู่ระบบ</NuxtLink>
        <label class="loginslash">|</label>
        <img class="icon-login" width="14" height="14" src="~/assets/images/icon/Icon_add-user.png" />
        <NuxtLink class="logintext" to="/">สมัครสมาชิก</NuxtLink>

    </div>
</template>

<style>
.icon-login {
    filter: invert(100%);
    margin-right: 8px;
    justify-self: end;
    align-self: center;
}

.loginslash {
    color: white;
    margin-left: 16px;
    margin-right: 16px;
}

.login {
    background-color: #636363;
    text-align: center;
    font-size: 14px;
    height: 40px;
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
}

.router-link-exact-active.logintext-left {
    color: white;
    text-decoration: none;
    margin-right: 840px;
}


.router-link-exact-active.logintext {
    color: white;
    text-decoration: none;

}

.logintext:hover {
    color: #929292;
    text-decoration: none;
}
</style>