<template>
    <section id="courses" class="py-5">

        <div class="container">

            <!-- titolo sezione -->
            <div class="row section-title">
                <div class="col text-center">
                    <p class="text-uppercase">stimulated to learn?</p>
                    <h2>Featured Online Courses</h2>
                </div>
            </div>

            <!-- corsi -->
            <div class="row row-cols-2 my-5">
                <coursesCard v-for="(course, index) in courses" :key="index" :course="course"/>
            </div>
            
            <!-- button corsi -->
            <div class="row">
                <div class="col d-flex justify-content-center">
                    <button class="ms_button d-inline-block border-0 rounded-2 d-block">View all courses</button>
                </div>
            </div>


        </div>

    </section>

</template>

<script>
import coursesCard from './elements/coursesCard.vue';

export default {
    name: 'onlineCourses',

    components: {
        coursesCard,
    },

    data(){
        return{

            //array oggetti corsi
            courses: [

                {
                    price: '$40.',

                    priceDex : '00',

                    name: 'Learning to write as a Professional Author',

                    lessons: '20',

                    students: '50',

                    img: 'course-02-480x298.jpg',

                    url: '#'
                },

                {
                    price: 'Free',

                    priceDex : '',

                    name: 'Customer-centric Info-tech Strategies',

                    lessons: '24',

                    students: '769',

                    img: 'stock-full-hd-03-480x298.jpg',

                    url: '#'
                },

                {
                    price: '$19.',

                    priceDex : '00',

                    name: 'Opening Programming Courses for Everyone: Python',

                    lessons: '17',

                    students: '62',

                    img: 'stock-full-hd-04-480x298.jpg',

                    url: '#'
                },

                {
                    price: '$26.',

                    priceDex : '00',

                    name: 'Accademic Listening and Note-taking',

                    lessons: '14',

                    students: '67',

                    img: 'stock-full-hd-06-480x298.jpg',

                    url: '#'
                },

                {
                    price: '$39.',

                    priceDex : '00',

                    name: 'Master jQuery in a Short Period of Time',

                    lessons: '6',

                    students: '51',

                    img: 'course-featured-image-01-480x298.jpg',

                    url: '#'
                },

                {
                    price: '$59.',

                    priceDex : '00',

                    name: 'Introduction to Javascript for Beginners',

                    lessons: '14',

                    students: '76',

                    img: 'stock-full-hd-05-480x298.jpg',

                    url: '#'
                },

            ],

        }
    }
}
</script>

<style lang="scss" scoped>
// richiamo varibili create da me
@import "../../assets/style/variables.scss";

#courses{
    background-color: $colorLightGrey;

    .section-title{
        @include sectionTitle
    }

    .ms_card-h{
        text-decoration: none;

        .ms_course-img{
            width: 150px;
            height: 150px;
            display: flex;
            align-items: center;
            border-radius: 50%;

            img{
                width: 100%;
                height: 100%;
                object-fit: cover;
                border-radius: 50%;
            }
        }

        .ms_card-body{
            
            h3{
                color:$colorGreen;
            }

            h4{
                color: $colorDarkBlue;
            }

            color: $colorFadeBlue;

            .ms_span-card-right{
                
                font-size: $fontLittle;

                &::before{
                    @include awasomeAppend;
                    content: "\f007";
                }
            }
        
            .ms_span-card-left{
                
                font-size: $fontLittle;

                &::before{
                    @include awasomeAppend;
                    content: "\f15c";
                }
            }

        }

        &:hover{

            h4{
                color: $colorGreen;
            }

        }

    }

    .ms_button{
        @include button;

        &::after{
            @include awasomeAppend;
            content: "\f178";
            margin-left: 20px;
        }
    }
}
</style>