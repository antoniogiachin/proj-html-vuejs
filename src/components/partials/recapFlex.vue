<template>
    <section id="recap-flex">
        <div class="container">
            <div class="row">

                <div class="col-3 d-flex flex-column justify-content-center align-items-center border-start border-end ms_col">
                    <h6>Successfully trained</h6>
                    <h2>1790</h2>
                    <p>Enrolled Learners</p>
                </div>

                <div class="col-3 d-flex flex-column justify-content-center align-items-center border-end ms_col">
                    <h6>Successfully trained</h6>
                    <h2>1790</h2>
                    <p>Enrolled Learners</p>
                </div>

                <div class="col-3 d-flex flex-column justify-content-center align-items-center border-end ms_col">
                    <h6>Successfully trained</h6>
                    <h2>1790</h2>
                    <p>Enrolled Learners</p>
                </div>

                <div class="col-3 d-flex flex-column justify-content-center align-items-center border-end ms_col">
                    <h6>Successfully trained</h6>
                    <h2>1790</h2>
                    <p>Enrolled Learners</p>
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

h6{
    color: $colorDarkBlue;
}

h2{
    color: $colorGreen;
}

p{
    color: $colorFadeBlue
}

</style>