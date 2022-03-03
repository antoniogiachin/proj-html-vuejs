<template>
    <section id="jumbotron" class="py-5">

            <div class="ms_actions d-flex flex-column align-items-center position-absolute rounded-start">
                <a href="#" class="text-dark"><i class="fas fa-ruler-combined"></i></a>
                <a href="#" class="text-dark"><i class="fa-regular fa-life-ring"></i></a>
                <a href="#" class="text-dark"><i class="fas fa-book"></i></a>
                <a href="#" class="text-dark"><i class="fas fa-shopping-cart"></i></a>
            </div>

            <div class="container">

                <!-- riga download e img -->
                <div class="row">
                    <div class="col-5 d-flex align-items-center ">
                        <div class="ms_card">
                            <h1 class="mb-1">Distant learning for further expansion</h1>
                            <p>Learning is a lofe-long jurney that in fact we never find the terminate stop. Stop searching, enjoy the process.</p>
                            <button class="border-0 ms_button rounded-2 d-block my-2"> <span>Download free guide</span> </button>
                            <span class="ms_sample">Have questions?</span> <span ><a class="ms_sample-link" href="#">Get Free Sample</a></span>
                        </div>
                    </div>
                    <div class="col-6 offset-1 d-flex justify-content-center position-relative">
                        <div class="shape-container position-absolute d-flex flex-column">
                            <img src="../../assets/img/maxcoach-shape-07.png" class="shape" alt="shape-jumbo">
                            <img src="../../assets/img/maxcoach-shape-07.png" class="shape" alt="shape-jumbo">
                        </div>
                        <img src="../../assets/img/maxcoach-shape-07.png" class="shape shape-03 position-absolute" alt="shape-jumbo">
                        <img src="../../assets/img/about-me-profile.jpg"  class="rounded-circle w-75 " alt="first-section-img">
                        <img src="../../assets/img/maxcoach-shape-02.png" class="shape shape-02 my-5" alt="shape-jumbo">
                    </div>
                </div>

                <!-- row clients -->
                <div class="row my-4">
                    <div class="col d-flex align-items-center justify-content-center">
                        <img src="../../assets/img/client-logo-01.png" class="ms_client-img" alt="client-1">
                    </div>
                    <div class="col d-flex align-items-center justify-content-center">
                        <img src="../../assets/img/client-logo-02.png" class="ms_client-img" alt="client-2">
                    </div>
                    <div class="col d-flex align-items-center justify-content-centerr">
                        <img src="../../assets/img/client-logo-03.png" class="ms_client-img" alt="client-3">
                    </div>
                    <div class="col d-flex align-items-center justify-content-center">
                        <img src="../../assets/img/client-logo-04.png" class="ms_client-img" alt="client-4">
                    </div>
                    <div class="col d-flex align-items-center justify-content-center">
                        <img src="../../assets/img/client-logo-05.png" class="ms_client-img" alt="client-5">
                    </div>
                    <div class="col d-flex align-items-center justify-content-center">
                        <img src="../../assets/img/client-logo-06.png" class="ms_client-img" alt="client-6">
                    </div>
                </div>
            </div>
        </section>
</template>

<script>
export default {
    name: 'sectionJumbo'
}
</script>

<style lang="scss" scoped>
// richiamo varibili create da me
@import "../../assets/style/variables.scss";

#jumbotron{
    position: relative;

    .ms_actions{
        gap: 10px;
        right: 0;
        box-shadow: 0px 3px 10px $colorGrey;
        padding: 5px;
        font-size: $fontLittle;
    }
    .ms_card{

        color: $colorDarkBlue;
        padding-right: 120px;

        p{
            color:$colorFadeBlue;
        }

        .ms_sample{
            font-size:$fontLittle;
            color:$colorFadeBlue;
        }

        .ms_sample-link{
            font-size: $fontLittle;
            color: $colorGreen;

            &::after{
                @include awasomeAppend;
                content: "\f178";
                margin-left: 5px;
            }
        }

        .ms_button{
            
            @include button;
    
            &::before{
                @include awasomeAppend;
                content: "\f019";
            }
    
        }
    }
    

    .shape{
        width: 100px;
        height: 100px;
    }

    .shape-02 {
        margin-left: -20px;
    }

    .shape-container{
        top: 20%;
        left: 0;
        gap: 10px;
        z-index: -1;
    }

    .shape-03{
        bottom: 0;
        left: 50%;
        z-index: -1;
    }

    .ms_client-img{
        filter: opacity(0.5);
    }
    

}
</style>