<template>
    <header class="main-header">
        <nav>
            <nuxt-link to='/'
                       tag='img'
                       :src='logo'
                       class="logo">
            </nuxt-link>
            <ul>
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
    </header>
</template>
<style>
    .main-header {
        background-color: green;

        .logo{

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