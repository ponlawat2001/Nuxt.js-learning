<template>
    <div>
        <carousel />
        <messagebar />
    </div>
</template>

<script>
import carousel from '~~/components/carousel.vue';
import messagebar from '~~/components/messagebar.vue'

export default {
    name: 'index',
    components: {
        carousel,
        messagebar
    }
}

</script>



