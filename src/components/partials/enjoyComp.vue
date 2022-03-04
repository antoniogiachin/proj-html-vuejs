<template>
    <section id="enjoy-comp" class="py-5 position-relative">

        <div class="container">
            
            <!-- riga testo e img -->
            <div class="row">

                <!-- img -->
                <div class="col-6 d-flex justify-content-center position-relative">
                    <img src="../../assets/img/maxcoach-shape-05.png" class="position-absolute ms_shape-01" alt="shape-01">
                    <img src="../../assets/img/maxcoach-shape-07.png" class="position-absolute ms_shape-02" alt="shape-02">
                    <img src="../../assets/img/icon-youtube-play.png"  class="ms_yt-icon position-absolute top-50 start-50 translate-middle" alt="yt-logo-img">
                    <img src="../../assets/img/home-2-popup-video-poster.jpg" class="w-75 rounded-1" alt="enjoy-img">
                </div>

                <!-- testo -->
                <div class="col-4 pe-5 position-relative ms_text-col">
                    <p class="text-uppercase fw-bold">get started <span class="fw-bold">efforlessly</span> </p>
                    <h1 class="pe-2">Enjoy Our <span>Companionship</span> </h1>
                    <p class="pe-5 mt-3">Sneak peak intowhat has in store for you on our online teaching and mentoring portal. Seek for some hidden hints of early-bird reward as well.</p>
                    <a href="#" class="position-absolute top-100 ms_link fw-bold">Download free guidebook</a>
                </div>
            </div>
        </div>
        
                

    </section>
</template>

<script>
export default {
    name: 'enjoyComp'
}
</script>

<style lang="scss" scoped>
// richiamo varibili create da me
@import "../../assets/style/variables.scss";

.ms_yt-icon{
    width: 70px;
    height: 50px;
    cursor: pointer;
}

.ms_shape-01{
    left: 0;
    top: 50px;
    z-index: -1;
}

.ms_shape-02{
    bottom: -30px;
    right: 60px;
    z-index: -1;
}

.ms_text-col{
    
    font-size:  $fontLittle;


    p{
        color:$colorFadeBlue;

        span {
            color:$colorDarkBlue;
        }
    }

    h1{
        color: $colorDarkBlue;

        span {
            color : $colorGreen
        }
    }

    .ms_link{
        color: $colorGreen;

        &::after{
            @include awasomeAppend;
            content: "\f178";
            margin-left: 5px;
        }
    }

}

</style>