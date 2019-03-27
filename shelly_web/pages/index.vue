<template>
    <section class="container">
        <div>
            <navbar/>
            <gallery/>
        </div>
    </section>
</template>

<script>
import navbar from "~/components/NavBar.vue";
import gallery from "~/components/Gallery.vue";

export default {
    components: {
        navbar,
        gallery
    }
};
</script>

<style>
.container {
    margin: 0 auto;
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
}
</style>
