<template>
    <header class="main-header">
        <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
            <div class="d-flex flex-grow-1">
                <span class="w-100 d-lg-none d-block"><!-- hidden spacer to center brand on mobile --></span>
                <nuxt-link to='/'
                       tag='img'
                       :src='logo'
                       class="navbar-brand logo">
                </nuxt-link>

                <div class="w-100 text-right">
                    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#myNavbar7">
                        <span class="navbar-toggler-icon"></span>
                    </button>
                </div>
            </div>
            <div class="collapse navbar-collapse flex-grow-1 text-right" id="myNavbar7">
                <ul class="navbar-nav ml-auto flex-nowrap">
                    <li class="nav-item dropdown">
                        <a data-toggle="dropdown" class="nav-link dropdown-toggle"
                           href="#" role="button" aria-haspopup="true" aria-expanded="false">
                            Portfolio
                        </a>
                        <div class="dropdown-menu">
                            <a class="dropdown-item" href="#">Paintings</a>
                            <a class="dropdown-item" href="#">Illustrations</a>
                        </div>
                    </li>
                    <li class="nav-item">
                        <a href="#" class="nav-link">About</a>
                    </li>
                    <li class="nav-item">
                        <a href="https://society6.com/shellyweasel" 
                           target="_blank"
                           class="nav-link">
                           Store
                        </a>
                    </li>
                    <li class="nav-item">
                        <a href="#" class="nav-link">Contact</a>
                    </li>
                </ul>
                <div class="social-media-icons">
                    <div class="facebook-icon social-media-icon">Facebook</div>
                    <div class="instagram-icon social-media-icon">Instagram</div>
                    <div class="youtube-icon social-media-icon">YouTube</div>
                </div>
            </div>
        </nav>
    </header>
</template>
<style lang="scss">
    .main-header {
        .logo{
            width: 25%;
            height: 25%
        }

        .social-media-icons {
            background-color: lightgrey;

            .social-media-icon {
                display: inline-block;
            }
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