<template>
    <div class="login">
        <NuxtLink class="logintext" to="/">เข้าสู่ระบบ</NuxtLink>
    </div>
</template>

<style>
.login {
    background-color: #343a40;
    text-align: right;
    height: 50px;
    width: 100%;
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