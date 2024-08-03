<script>
export default {
    data () {
        return {
            dcComics: [
                {
                    label: 'characters',
                    url: '#',
                },
                {
                    label: 'comics',
                    url: '#',
                },
                {
                    label: 'movies',
                    url: '#',
                },
                {
                    label: 'tv',
                    url: '#',
                },
                {
                    label: 'games',
                    url: '#',
                },
                {
                    label: 'videos',
                    url: '#',
                },
                {
                    label: 'news',
                    url: '#',
                }
            ],
            shops: [
                {
                    label: 'Shop DC',
                    url: '#'
                },
                {
                    label: 'Shop DC Collectibles',
                    url: '#'
                }
            ],
            dCs: [
                {
                    label: 'Terms of Use',
                    url: '#'
                },
                {
                    label: 'Privacy Policy (New)',
                    url: '#'
                },
                {
                    label: 'Ad Chioces',
                    url: '#'
                },
                {
                    label: 'Advertising',
                    url: '#'
                },
                {
                    label: 'Jobs',
                    url: '#'
                },
                {
                    label: 'Subscriptions',
                    url: '#'
                },
                {
                    label: 'Talent Workshops',
                    url: '#'
                },
                {
                    label: 'CPSC Certificates',
                    url: '#'
                },
                {
                    label: 'Ratings',
                    url: '#'
                },
                {
                    label: 'Shop Help',
                    url: '#'
                },
                {
                    label: 'Contact Us',
                    url: '#'
                }
            ],
            sites: [
                {
                    label: 'DC',
                    url: '#'
                },
                {
                    label: 'MAD Magazine',
                    url: '#'
                },
                {
                    label: 'DC Kids',
                    url: '#'
                },
                {
                    label: 'DC Universe',
                    url: '#'
                },
                {
                    label: 'DC Power Visa',
                    url: '#'
                }
            ]
        }
    }
}
</script>
<template>
    <footer>
        <div class="bg-top">
            <div class="container">
                <div class="row">
                    <div class="col-12 col-md-2">
                        <div class="content my-4">
                            <h6 class="text-white">DC COMICS</h6>
                            <ul class="list-unstyled">
                                <li v-for="(dcComic, index) in dcComics" :key="index">
                                    <a :href="dcComic.url">{{dcComic.label}}</a>
                                </li>
                            </ul>
                            <h6 class="text-white">SHOP</h6>
                            <ul class="list-unstyled">
                                <li v-for="(shop, index) in shops" :key="index">
                                    <a :href="shop.url">{{shop.label}}</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                    <div class="col-12 col-md-2">
                        <div class="content my-4">
                            <h6 class="text-white">DC</h6>
                            <ul class="list-unstyled">
                                <li v-for="(dC, index) in dCs" :key="index">
                                    <a :href="dC.url">{{dC.label}}</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                    <div class="col-12 col-md-2">
                        <div class="content my-4">
                            <h6 class="text-white">SITES</h6>
                            <ul class="list-unstyled">
                                <li v-for="(site, index) in sites" :key="index">
                                    <a :href="site.url">{{site.label}}</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                    <div class="col-md-6">
                    </div>
                </div>
            </div>
        </div>
        <div class="bg-bottom">
            <div class="container">
                <div class="row"> 
                    <div class="col-12">
                        <div class="content d-flex justify-content-between align-items-center">
                            <button class="btn btn-sm btn-tertiary text-white">SIGN-UP NOW!</button>
                            <div class="icons d-flex">
                                <div class="text-primary">
                                    FOLLOW US
                                </div>
                                <img class="ms-3" src="../assets/img/footer-facebook.png" alt="">
                                <img class="ms-3" src="../assets/img/footer-twitter.png" alt="">
                                <img class="ms-3" src="../assets/img/footer-youtube.png" alt="">
                                <img class="ms-3" src="../assets/img/footer-pinterest.png" alt="">
                                <img class="ms-3" src="../assets/img/footer-periscope.png" alt="">
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>
<style lang="scss" scoped>
    footer { 
        color: rgb(139, 135, 135);
        height: 600px;
        .bg-top {
            background-image: url(../assets/img/footer-bg.jpg);
            
            li {
                font-size: 10px;
                a {
                    text-decoration: none;
                    color: #999898;
                }
            }
            .col-md-6 {
                background-image: url('../assets/img/dc-logo-bg.png');
                background-size: 400px;
                background-position: center;
                background-repeat: no-repeat;
            }
        }
        .bg-bottom {
            background-color: #303030;
            .content {
                height: 70px;
            }
            .btn {
                border: 1px solid #0d6efd;
            }
            img {
                height: 20px;
            }
        }
    }
</style>