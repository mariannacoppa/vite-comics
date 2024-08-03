<script>
import dcComics from '../../vue-dc-comics-2/dc-comics.json';
import CardItem from './CardItem.vue';

export default {
    components: {
        CardItem
    },
    props: {
        mainTitle: String
    },
    data() {
        return {
            menues: [
                {
                    img: '../src/assets/img/buy-comics-digital-comics.png',
                    url: '#',
                    label: 'digital comics'
                },
                {
                    img: '../src/assets/img/buy-comics-merchandise.png',
                    url: '#',
                    label: 'dc merchandise'
                },
                {
                    img: '../src/assets/img/buy-comics-subscriptions.png',
                    url: '#',
                    label: 'subscriptions'
                },
                {
                    img: '../src/assets/img/buy-comics-shop-locator.png',
                    url: '#',
                    label: 'comic shop locator'
                },
                {
                    img: '../src/assets/img/buy-dc-power-visa.svg',
                    url: '#',
                    label: 'dc power visa'
                }
            ],
            cards: dcComics
        }
    }
}
</script>
<template>
    <main>
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <div class="badge p-3 bg-primary">
                        {{ mainTitle }}
                    </div>
                </div>
            </div>
        </div>
    </main>
    <div class="bg-dark">
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <div class="content d-flex justify-content-center flex-wrap mt-5">
                        <CardItem class="card col-3" v-for="(card, index) in cards" :thumb="card.thumb" :series="card.series" />
                    </div>
                </div>
                <div class="col-12">
                    <div class="content d-flex justify-content-center">
                        <div class="btn btn-primary my-3">load more</div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div class="bg-primary">
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <div class="content align-content-center">
                        <ul class="list-unstyled d-flex justify-content-between">
                            <li class="px-2 mt-2 align-content-center" v-for="(menu, index) in menues" :key="index">
                                <img :src="menu.img" :alt="menu.label">
                                <a :href="menu.url">{{menu.label}}</a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
    main {
        background-image: url('../assets/img/jumbotron.jpg');
        background-size: cover;
        height: 250px;
        .badge {
            margin-top: 230px;
        }
        .card {
            img {
                height: 200px;
                object-fit: contain;
            }
            background-color: black;
        }
    }
    .bg-dark {
        .btn {
            text-transform: uppercase;
        }
    }
    .bg-primary {
        a {
            text-transform: uppercase;
            font-size: 8px;
            color: white;
            text-decoration: none;
        }
        img {
            width: 20px;
            padding-right: 5px;
        }
    }
</style>