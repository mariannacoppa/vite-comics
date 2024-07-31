<script>
export default {
    
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
                                <li>Characters</li>
                                <li>Comics</li>
                                <li>Movies</li>
                                <li>TV</li>
                                <li>Games</li>
                                <li>Videos</li>
                                <li>News</li>
                            </ul>
                            <h6 class="text-white">SHOP</h6>
                            <ul class="list-unstyled">
                                <li>Shop DC</li>
                                <li>Shop DC Collections</li>
                            </ul>
                        </div>
                    </div>
                    <div class="col-12 col-md-2">
                        <div class="content my-4">
                            <h6 class="text-white">DC</h6>
                            <ul class="list-unstyled">
                                <li>Terms Of Use</li>
                                <li>Privacy Policy (New)</li>
                                <li>Ad Choices</li>
                                <li>Advertising</li>
                                <li>Jobs</li>
                                <li>Subscriptions</li>
                                <li>Talent Workshops</li>
                                <li>CPSC Certificates</li>
                                <li>Ratings</li>
                                <li>Shop Help</li>
                                <li>Contact Us</li>
                            </ul>
                        </div>
                    </div>
                    <div class="col-12 col-md-2">
                        <div class="content my-4">
                            <h6 class="text-white">SITES</h6>
                            <ul class="list-unstyled">
                                <li>DC</li>
                                <li>MAD Magazine</li>
                                <li>DC Kids</li>
                                <li>DC Universe</li>
                                <li>DC Power Visa</li>
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