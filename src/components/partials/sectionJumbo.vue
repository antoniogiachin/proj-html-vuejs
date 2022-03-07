<template>
    <section id="jumbotron" class="py-5">

        <!-- componente menu azioni -->
        <actionsJumbo :actionLinks="actionLinks"/>

        <div class="container">

            <!-- riga download e img -->
            <div class="row">
                <div class="col-5 d-flex align-items-center">
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

            <!-- row clientsJumbo -->
            <clientsJumbo :clients="clients" />
        </div>
        
        </section>
</template>

<script>
import clientsJumbo from './elements/clientsJumbo.vue';
import actionsJumbo from './elements/actionsJumbo.vue';


export default {
    name: 'sectionJumbo',

    components: {
        clientsJumbo,

        actionsJumbo,
    },

    data(){

        return {

            // Array oggetti clients
            clients: [

                {
                    brand: 'stylus',

                    appendUrl: require('../../assets/img/client-logo-01.png'),
                },

                {
                    brand: 'tree',

                    appendUrl: require('../../assets/img/client-logo-02.png'),
                },

                {
                    brand: 'brook',

                    appendUrl: require('../../assets/img/client-logo-03.png'),
                },

                {
                    brand: 'pencil',

                    appendUrl: require('../../assets/img/client-logo-04.png'),
                },

                {
                    brand: 'alive',

                    appendUrl: require('../../assets/img/client-logo-05.png'),
                },

                {
                    brand: 'sixbase',

                    appendUrl:require('../../assets/img/client-logo-06.png'),
                },

            ],

            //array Actions Links
            actionLinks : [

                {
                    url: '#',

                    icon: 'fa-ruler-combined'
                },

                {
                    url: '#',

                    icon: 'fa-life-ring'
                },

                {
                    url: '#',

                    icon: 'fa-book'
                },

                {
                    url: '#',

                    icon: 'fa-shopping-cart'
                },
            ],

        }

    }
}
</script>

<style lang="scss" scoped>
// richiamo varibili create da me
@import "../../assets/style/variables.scss";

#jumbotron{
    position: relative;

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
            text-decoration: none;

            &::after{
                @include awasomeAppend;
                content: "\f178";
                margin-left: 5px;
            }

            &:hover{
                text-decoration: underline;
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