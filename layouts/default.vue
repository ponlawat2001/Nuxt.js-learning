<template>
    <div>
        <login />
        <menubar />
        <NuxtPage />
        <!-- <footer /> -->
    </div>
</template>

<script>
import menubar from '~/components/menubar.vue';
import login from '~/components/headerlogin.vue';
// import footer from '~/components/footer.vue'

export default {
    name: 'default',
    components: {
        menubar,
        login,
    }
}

</script>

<style>
body {
    margin: 0%;
    background-color: #f8f9fa;
    line-height: 23px;
    font-style: normal;
    font-family: TrueMedium, sans-serif;
    color: #929292;
    font-weight: 400;
}
</style>