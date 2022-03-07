<template>


    <div class="col my-5 px-3">
        <a class="ms_card-h" :href="course.url" >
            <div class="row">
                <div class="col-md-4 p-2 d-flex align-items-center justify-content-center">
                    <div class="ms_course-img ">
                        <img :src='require("../../../assets/img/" + course.img)'  alt="course-1">
                    </div>
                </div>
                <div class="col-md-8 p-2 d-flex align-items-center justify-content-center">
                    <div class="ms_card-body pe-4">
                        <h3 class="card-title"><span class="h2">{{course.price}}</span>{{course.priceDex}}</h3>
                        <h4 class="card-title">{{course.name}}</h4>
                        <span class="me-5 ms_span-card-left">{{course.lessons}} Lessons</span>
                        <span class="ms-5 ms_span-card-right"> {{course.students}} Students</span>
                    </div>
                </div>
            </div>
        </a>
    </div>


</template>

<script>
export default {
    name: 'coursesCard',

    props: {
        "course" : Object
    }
}
</script>

<style lang="scss" scoped>
// richiamo varibili create da me
@import "../../../assets/style/variables.scss";

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
</style>