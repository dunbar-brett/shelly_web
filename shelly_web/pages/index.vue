<template>
    <section class="container-fluid sjw-banner-wrapper">
        <banner/>
    </section>
</template>

<script>
import banner from "~/components/Banner.vue";

export default {
    components: {
        banner
    }
};
</script>

<style lang="scss">
.sjw-banner-wrapper {
    padding-left: 0;
    padding-right: 0;
}
</style>
