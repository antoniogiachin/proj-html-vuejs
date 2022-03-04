<template>
    <section id="smart-touring" class="py-5">
        <div class="container">
            
            <!-- titolo sezione -->
            <div class="row section-title">
                <div class="col text-center">
                    <p class="text-uppercase">max coach available courses</p>
                    <h2>Access <span>Smart Tutoring</span>  Program For Benefits</h2>
                </div>
            </div>

            <!-- row con cards -->
            <div class="row my-5">
                <div class="col-4 ms_card">
                    <img src="../../assets/img/home-2-image-box-01.png" class="img-fluid" alt="sm-t-img1">
                    <h3 class="mt-3">Customize Preferences</h3>
                    <p>Learners are given the right to arrange and customize their study schedule and timetable based on preferences</p>
                    <a href="#" class="ms_smart-link"> Start here</a>
                </div>

                <div class="col-4 ms_card">
                    <img src="../../assets/img/about-us-02-image-box-02.png" class="img-fluid" alt="sm-t-img1">
                    <h3 class="mt-3">Cloud Storage</h3>
                    <p>You can store online lessons via online cloud or download to your device and revise lessons on the way.</p>
                    <a href="#" class="ms_smart-link"> Get Free Quote</a>
                </div>

                <div class="col-4 ms_card">
                    <img src="../../assets/img/home-2-image-box-03.png" class="img-fluid" alt="sm-t-img1">
                    <h3 class="mt-3">Multimedia Channels</h3>
                    <p>We provide study materials with various formats: video, audio, slides, doc, prints, book and applications</p>
                    <a href="#" class="ms_smart-link"> Start Now</a>
                </div>
            </div>

            

        </div>
    </section>
</template>

<script>
export default {
    name: 'smartTouring',
}
</script>

<style lang="scss" scoped>
// richiamo varibili create da me
@import "../../assets/style/variables.scss";
.section-title{
    
    @include sectionTitle;

    span {
        color: $colorGreen
    }

}

.ms_card{

    font-size: $fontLittle;

    line-height: 30px;

    h3{
        color: $colorDarkBlue;
    }

    p{
        color: $colorFadeBlue;
    }
    .ms_smart-link{

        color: $colorDarkBlue;
        text-decoration: none;

        &:hover{
            text-decoration: underline;
        }

        &::after{    
            @include awasomeAppend;
            content: "\f178";
            margin-left: 5px;
        }
    }
}

</style>