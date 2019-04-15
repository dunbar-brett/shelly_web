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
            <div class="collapse navbar-collapse flex-grow-1 text-center" id="myNavbar7">
                <ul class="navbar-nav ml-auto flex-nowrap">
                    <li class="nav-item sjw-nav-item sjw-dropdown">
                        <a class="nav-link sjw-dropbtn">
                            Portfolio
                        </a>
                        <div class="sjw-dropdown-content">
                            <a class="sjw-dropdown-content-item text-center" href="#">Paintings</a>
                            <a class="sjw-dropdown-content-item text-center" href="#">Illustrations</a>
                        </div>
                    </li>
                    <li class="nav-item sjw-nav-item">
                        <a href="#" class="nav-link">About</a>
                    </li>
                    <li class="nav-item sjw-nav-item">
                        <a href="https://society6.com/shellyweasel" 
                           target="_blank"
                           class="nav-link">
                           Store
                        </a>
                    </li>
                    <li class="nav-item sjw-nav-item">
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

        .sjw-nav-item {
            width: 8rem;
        }

        .sjw-dropdown {
            &:hover {
                background: rgba(145, 216, 221, .8);
            }
        }

        .sjw-dropdown-content {
            display: none;
            position: absolute;
            background-color: rgba(145, 216, 221, .8);
            min-width: 8rem;
            //box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
            z-index: 1;

            .sjw-dropdown-content-item {
                float: none;
                color: black;
                padding: 12px 16px;
                text-decoration: none;
                display: block;
                text-align: left;

                &:hover {
                    //background-color: rgba(145, 216, 221, .8);
                    color: white;
                }
            }
        }

        .sjw-dropdown:hover .sjw-dropdown-content {
            display: block;
        }

        .social-media-icons {
            background-color: lightgrey;
            min-width: 12rem;

            .social-media-icon {
                display: inline-block;
                min-width: 4rem;
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