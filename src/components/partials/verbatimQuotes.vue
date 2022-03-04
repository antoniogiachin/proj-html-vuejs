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

        </div>

        <div class="container-fluid">

            <!-- row quotes -->
            <div class="row">

                <div class="col-4 p-4 ms_faded">
                    <div class="ms_card rounded-1">
                        <h5 class="pb-3">It's a chioce of quality for peaople with special needs</h5>
                        <p>I am a very strict person so I require everything to be organized and neat. Then, i'll be able to make things right and shine. MaxCoach guys got me.</p>
                        <div class="ms_people-quote d-flex pt-3">
                            <img src="../../assets/img/testimonial-avata-03.jpg" class="img-fluid rounded-circle" alt="testimonial-img">
                            <div class="ms_people-info d-flex flex-column justify-content-center ms-5">
                                <span class="fw-bold text-uppercase mb-1">florence themes</span>
                                <span>/ Multimedia Admin</span>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="col-4 p-4">
                    <div class="ms_card rounded-1">
                        <h5 class="pb-3">High level efficiency and scientific teaching methods</h5>
                        <p>I am free  to elarn at my own peace, follow my own schedule and choose the subject I wanto to learn from  the syllabus. Great study portal for people like me.</p>
                        <div class="ms_people-quote d-flex pt-3">
                            <img src="../../assets/img/testimonial-avata-02.jpg" class="img-fluid rounded-circle" alt="testimonial-img">
                            <div class="ms_people-info d-flex flex-column justify-content-center ms-5">
                                <span class="fw-bold text-uppercase mb-1">mina hollace</span>
                                <span>/ Freelancer</span>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="col-4 p-4 ms_faded">
                    <div class="ms_card rounded-1">
                        <h5 class="pb-3">Professional team of specialist and passionate mentors at reach</h5>
                        <p>i need to get a certification for English profiency and MaxCoach is my best choice. Their tutors are smart and professional when dealing with students.</p>
                        <div class="ms_people-quote d-flex pt-3">
                            <img src="../../assets/img/testimonial-avata-04.jpg" class="img-fluid rounded-circle" alt="testimonial-img">
                            <div class="ms_people-info d-flex flex-column justify-content-center ms-5">
                                <span class="fw-bold text-uppercase mb-1">Medley Pondor</span>
                                <span>/ IT Specialist</span>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- separatore -->
                <div class="ms_divide d-flex justify-content-center mt-2">
                    <i class="fas fa-circle ms_current-dot"></i>
                    <i class="fas fa-circle"></i>
                    <i class="fas fa-circle"></i>
                    <i class="fas fa-circle"></i>
                </div>

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

    .ms_faded{
        filter: opacity(0.5);
    }

    .ms_card{
        font-size: $fontLittle;

        padding: 30px 60px;

        background-color: #fff;

        h5{
            color: $colorDarkBlue
        }

        p{
            color: $colorFadeBlue;
        }
        
        span{
            color: $colorDarkBlue;

        }

        img{
            width: 100px;
            height: 100px;
        }
    }
    
    .ms_divide{

        font-size:  0.5em;
        color: $colorGrey;
        gap: 20px;

        .ms_current-dot{
            color: $colorDarkBlue;
            transform: scale(1.5);
            
        }

    }
}
</style>