<template>
    <div>
        <TheHeader/>
        <main class="main-content">
            <nuxt/>
        </main>
        <TheFooter/>
    </div>
</template>

<script>
import TheHeader from "~/components/TheHeader.vue";
import TheFooter from "~/components/TheFooter.vue";

export default {
    components: {
        TheHeader,
        TheFooter
    }
};
</script>


<style>
html {
    font-family: "Lato", sans-serif;
    font-size: 16px;
    word-spacing: 1px;
    -ms-text-size-adjust: 100%;
    -webkit-text-size-adjust: 100%;
    -moz-osx-font-smoothing: grayscale;
    -webkit-font-smoothing: antialiased;
    box-sizing: border-box;
}

*,
*:before,
*:after {
    box-sizing: border-box;
    margin: 0;
}

.main-content {
    background-color: white;
}
</style>
