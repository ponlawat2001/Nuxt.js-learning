<template>
    <div class="login">
        <nuxt-link class="logintext" to="/">เข้าสู่ระบบ</nuxt-link>
    </div>
</template>

<style>
.login {
    background-color: #343a40;
    text-align: right;
    height: 50px;
}

.nuxt-link-exact-active.logintext {
    color: white;
    text-decoration: none;
}

.logintext:hover {
    color: #929292;
    text-decoration: none;
}
</style>