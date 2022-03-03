<template>
    <main>
        <!-- sezione jumbotron -->
        <sectionJumbo/>

        <!-- sezione online courses -->
        <onlineCourses/>
        
    </main>
</template>

<script>
import sectionJumbo from './partials/sectionJumbo.vue'
import onlineCourses from './partials/onlineCourses.vue'


export default {
    name: 'myMain',

    components : {
        sectionJumbo,

        onlineCourses,
    }
}
</script>

<style lang="scss" scoped>
// richiamo varibili create da me
@import "../assets/style/variables.scss";

#jumbotron{
    position: relative;

    .ms_actions{
        gap: 10px;
        right: 0;
        box-shadow: 0px 3px 10px $colorGrey;
        padding: 5px;
        font-size: 0.8em;
    }
    .ms_card{

        color: $colorDarkBlue;
        padding-right: 120px;

        p{
            color:$colorFadeBlue;
        }

        .ms_sample{
            font-size:0.8em;
            color:$colorFadeBlue;
        }

        .ms_sample-link{
            font-size: 0.8em;
            color: $colorGreen;

            &::after{
                display: inline-block;
                text-rendering: auto;
                -webkit-font-smoothing: antialiased;
                font: var(--fa-font-solid);
                content: "\f178";
                margin: 0px 10px;
            }
        }

        .ms_button{
            background-color: $colorGreen;
            color: #fff;
            padding: 15px 20px;
            font-weight: bold;
            font-size: 0.8em;
    
            &::before{
                display: inline-block;
                text-rendering: auto;
                -webkit-font-smoothing: antialiased;
                font: var(--fa-font-solid);
                content: "\f019";
                margin: 0px 10px;
            }
    
            &:hover{
                background-color: $colorDarkBlue;
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