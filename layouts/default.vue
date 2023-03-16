<template>
    <div>
        <login />
        <menubar />
        <Nuxt />
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