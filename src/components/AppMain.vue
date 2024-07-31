<script>
export default {
    
}
</script>
<template>
    <main>
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <div class="badge p-3 bg-primary">
                        current series
                    </div>
                </div>
            </div>
        </div>
    </main>
    <div class="bg-dark">
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <div class="content d-flex justify-content-center">
                        <div class="cards text-white">cards</div>
                    </div>
                </div>
                <div class="col-12">
                    <div class="content d-flex justify-content-center">
                        <div class="btn btn-primary mt-3">load more</div>
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
    }
    .bg-dark {
        height: 250px;
        .btn {
            text-transform: uppercase;
        }
    }
</style>