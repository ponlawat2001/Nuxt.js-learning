<template>
    <div>
        <menubar />
        <Nuxt />
        <footer />
    </div>
</template>

<script>
import menubar from '~/components/menubar.vue';
// import footer from '~/components/footer.vue'

export default {
    name: 'default',
    components: {
        menubar,
    }
}

</script>