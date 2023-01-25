<template>
    <div class="menubar">
        <img class="logo" src="assets/images/logo/logo.png" alt="Logo" />
        <label class="title">
            Menu
            <slot></slot>
        </label>
    </div>
</template>

<style>
.menubar {
    background-color: #f1f1f1;
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    height: 100px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 20px;
    box-sizing: border-box;
}

.logo {
    height: 24;
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