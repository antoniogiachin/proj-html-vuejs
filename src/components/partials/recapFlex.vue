<template>
    <section id="recap-flex">
        <div class="container">
            <div class="row text-center">

                <div class="col-3 lh-lg d-flex flex-column justify-content-center align-items-center border-start border-end ms_col">
                    <h5>Successfully <br> Trained</h5>
                    <h2>1790</h2>
                    <p class="text-uppercase">Enrolled Learners</p>
                </div>

                <div class="col-3 d-flex flex-column justify-content-center align-items-center border-end ms_col">
                    <h5>Proudly <br> Received</h5>
                    <h2>19</h2>
                    <p class="text-uppercase">countrywide awards</p>
                </div>

                <div class="col-3 d-flex flex-column justify-content-center align-items-center border-end ms_col">
                    <h5>Family <br> Established</h5>
                    <h2>24</h2>
                    <p class="text-uppercase">local branches</p>
                </div>

                <div class="col-3 d-flex flex-column justify-content-center align-items-center border-end ms_col">
                    <h5>Getting <br> Featured on</h5>
                    <h2>1090</h2>
                    <p class="text-uppercase">Blog Posts</p>
                </div>

            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'recapFlex'
}
</script>

<style lang="scss" scoped>
// richiamo varibili create da me
@import "../../assets/style/variables.scss";

.ms_col{
    padding: 80px 30px;
}

h5{
    color: $colorDarkBlue;
}

h2{
    color: $colorGreen;
    font-size: $fontBig;
}

p{
    color: $colorFadeBlue;
    font-size: $fontLittle;
}

</style>