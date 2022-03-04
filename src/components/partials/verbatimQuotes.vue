<template>
    <section id="verbatim-quotes" class="position-relative">
        
        <!-- shape divider -->
        <img src="../../assets/img/wave.png" class="ms_wave" alt="wave-divider">

        <div class="container">

            <!-- titolo sezione -->
            <div class="row section-title">
                <div class="col text-center">
                    <p class="text-uppercase fw-bold">great words about maxcoach</p>
                    <h2> Our <span>top learners' </span> verbatim</h2>
                </div>
            </div>

            <div class="row">

            </div>
        </div>
    </section>
</template>

<script>
export default {
    name:'verbatimQuotes'
}
</script>

<style lang="scss" scoped>
// richiamo varibili create da me
@import "../../assets/style/variables.scss";



#verbatim-quotes{
    background-color: $colorLightGrey;

    
    .ms_wave{
        position: absolute;
        top: -275px;
        transform: rotatey(180deg);
        width: 1000px;
        height: 500px;
        right: 0;
        z-index: -1;

    }

    .section-title{

        padding: 100px 0px;
        p{
            color: $colorFadeBlue;
        }

        h2{
            color: $colorDarkBlue;

            span{
                color: $colorGreen;
            }
        }
    }
}
</style>