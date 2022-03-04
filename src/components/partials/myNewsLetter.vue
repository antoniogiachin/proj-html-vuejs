<template>
    <section id="newsletter" class="py-5">
        
        <div class="container text-center">
            <div class="row my-5 ms_newsletter">
                <div class="col-2 position-relative">
                        <img src="../../assets/img/maxcoach-shape-05.png" class="img-fluid shape-01 position-absolute" alt="shape-img">
                </div>
                <div class="col-6 offset-1 d-flex flex-column align-items-center">
                    <h3>Subscribe <span>Newsletter</span></h3>
                    <p>Enter your email address to register to our newsletter subscription delivered on a regular basis!</p>
                    <div class="input-group mb-3">
                        <input type="email" class="form-control ms_input border-0" placeholder="Enter your email" aria-label="Recipient's username" aria-describedby="basic-addon2">
                        <button class="border-0 ms_button rounded-2  ">Subscribe</button>
                    </div>      
                </div>
                <div class="col-2 offset-1 position-relative">
                    <img src="../../assets/img/maxcoach-shape-02.png" class="img-fluid shape-02 position-absolute" alt="shape-img">
                </div>
            </div>
        </div>

    </section>
</template>

<script>
export default {
    name: 'myNewsLetter'
}
</script>

<style lang="scss" scoped>
/* // richiamo varibili create da me */
@import "../../assets/style/variables.scss";

.ms_newsletter{
    p{
            color:$colorDarkBlue;

    }

    h3{
        color:$colorDarkBlue;

        span{
            color: $colorGreen;
        }
    }

    .ms_input{
        background-color: $colorLightGrey
    }

    .ms_button{
        @include button;
    }

    .shape-01{
        right: 5px;
        top: 20px;
        width: 80px;
        height: 80px;
    }

    .shape-02{
        left: 80px;
    }
}
</style>