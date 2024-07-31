<script>
export default {
    data () {
        return {
            links: [
                {
                    label: 'characters',
                    url: '#',
                    current: false
                },
                {
                    label: 'comics',
                    url: '#',
                    current: true
                },
                {
                    label: 'movies',
                    url: '#',
                    current: false
                },
                {
                    label: 'tv',
                    url: '#',
                    current: false
                },
                {
                    label: 'games',
                    url: '#',
                    current: false
                },
                {
                    label: 'collectibles',
                    url: '#',
                    current: false
                },
                {
                    label: 'videos',
                    url: '#',
                    current: false
                },
                {
                    label: 'fans',
                    url: '#',
                    current: false
                },
                {
                    label: 'news',
                    url: '#',
                    current: false
                },
                {
                    label: 'shop',
                    url: '#',
                    current: false
                },
            ]
        }
    }
}
</script>
<template>
    <div>
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <div class="content d-flex justify-content-between">
                        <div class="logo d-flex py-2">
                            <img src="../assets/img/dc-logo.png" alt="dc-logo">
                        </div>
                        <div class="nav-menu">
                            <ul class="list-unstyled d-flex">
                                <li v-for="link, index in links" :key="index" :class="link.current ? 'active' : ''">
                                    <a :href="link.url">{{ link.label }}</a>
                                </li>
                                <!-- <li class="active"><a href="#">comics</a></li>
                                <li><a href="#">movies</a></li>
                                <li><a href="#">tv</a></li>
                                <li><a href="#">games</a></li>
                                <li><a href="#">collectibles</a></li>
                                <li><a href="#">videos</a></li>
                                <li><a href="#">fans</a></li>
                                <li><a href="#">news</a></li>
                                <li><a href="#">shop</a></li> -->
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../styles/partials/variables';
    ul {
        li {
            padding: 20px;
            a {
                text-decoration: none;
                text-transform: uppercase;
                color: black;
                font-size: 10px;
                transition: font-weight 0.3s;
                &:hover {
                    font-weight: 800;
                }
            }
        }
    }
    .active {
        border-bottom: 5px solid variables.$primary_color;
    }
    .logo, .nav-menu {
        height: 70px;
    }
    img {
        height: 50px;
    }
</style>