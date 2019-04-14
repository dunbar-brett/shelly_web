<template>
    <!-- <header class="main-header">
        <nav>
            <nuxt-link to='/'
                       tag='img'
                       :src='logo'
                       class="logo">
            </nuxt-link>
            <ul class="nav pull-right">
                <li>
                    Portfolio
                    <ul>
                        <nuxt-link tag="li" to="/">Paintings</nuxt-link>
                        <nuxt-link tag="li" to="/">Illustrations</nuxt-link>
                    </ul>
                </li>
                <nuxt-link to='/about' tag="li"><a>About</a></nuxt-link>
                <li><a href="https://society6.com/shellyweasel">Store</a></li>
                <nuxt-link to='/about' tag="li"><a>Contact</a></nuxt-link>
            </ul>
        </nav>
    </header> -->

    <header class="main-header">
        <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
            <div class="d-flex flex-grow-1">
                <span class="w-100 d-lg-none d-block"><!-- hidden spacer to center brand on mobile --></span>
                <a class="navbar-brand" href="#">
                    Navbar 7
                </a>
                <div class="w-100 text-right">
                    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#myNavbar7">
                        <span class="navbar-toggler-icon"></span>
                    </button>
                </div>
            </div>
            <div class="collapse navbar-collapse flex-grow-1 text-right" id="myNavbar7">
                <ul class="navbar-nav ml-auto flex-nowrap">
                    <li class="nav-item">
                        <a href="#" class="nav-link">Link</a>
                    </li>
                    <li class="nav-item">
                        <a href="#" class="nav-link">Link</a>
                    </li>
                    <li class="nav-item">
                        <a href="#" class="nav-link">Link</a>
                    </li>
                    <li class="nav-item">
                        <a href="#" class="nav-link">Link</a>
                    </li>
                </ul>
            </div>
        </nav>
    </header>
</template>
<style lang="scss">
    .main-header {
        background-color: green;

        .logo{
            width: 25%;
        }
    }
</style>


<script>
import logo from '~/assets/images/logos/shelly-weasel-logo.png';

export default {
    data() {
        return {
            logo: logo,
        };
    },
};
</script>