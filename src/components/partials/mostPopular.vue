<template>
    <section id="most-popular" class="py-5">

        <div class="container">
            <div class="row">
                <div class="col-4">
                    <!-- titolo sezione -->
                    <div class="row section-title">
                        <div class="col">
                            <p class="text-uppercase">max coach available courses</p>
                            <h3>Most Viewed <span>Best Blogs</span> </h3>
                        </div>
                    </div>

                    <!-- lista sezione -->
                    <mostPopularList :popularList="popularList"/>
                </div>
                
                <div class="col-4">

                    <div class="card border-0 ms_card">
                        <img src="../../assets/img/artist-blog-03-480x352.jpeg" class="card-img-top" alt="blog-card-img">
                        <div class="card-body lh-lg">
                            <a href="#">
                                <span class="text-uppercase">Artist</span>
                                <h5>Brush Strokes Energize Trees <br> in Paintings</h5>
                                <span class="ms_span-left me-5">May 15, 2020</span> <span class="ms_span-right">688 views</span>
                            </a>
                        </div>
                    </div>

                </div>

                <div class="col-4"> 
                        

                    <div class="card border-0 ms_card">
                        <img src="../../assets/img/artist-blog-01-480x352.jpg" class="card-img-top" alt="blog-card-img">
                        <div class="card-body lh-lg">
                            <a href="#">
                                <span class="text-uppercase">Artist</span>
                                <h5>Pocket Sized Notebooks Hold Miniature Paintings</h5>
                                <span class="ms_span-left me-5">May 15, 2020</span> <span class="ms_span-right">608 views</span>
                            </a>
                        </div>
                    </div>
                        
                    
                </div>
                
            </div>
        </div>
    </section>
</template>

<script>
import mostPopularList from './elements/mostPopularList.vue';

export default {
    name: 'mostPopular',

    components: {
        mostPopularList,
    },

    data(){
        return {

            // array oggetti lista popular
            popularList: [

                {
                    url: '#',

                    title: 'Become a Better Blogger: Content Planning'
                
                },

                {
                    url: '#',

                    title: 'Promoting Your Online Buiness on Pinterest'
                
                },

                {
                    url: '#',

                    title: 'Designing on Online Course from Expert\'s Prospective'
                
                },

                {
                    url: '#',

                    title: 'Why Online Courses are The Future of Education'
                
                },

            ],
        }
    }
}
</script>

<style lang="scss" scoped>
// richiamo varibili create da me
@import "../../assets/style/variables.scss";

#most-popular{
    background-color: $mostPopular;

    font-size: $fontLittle;

    .section-title{
        @include sectionTitle;

        span{
            color: $colorGreen;
        }
        
    }

    .fa-ul{
        margin: 0px 25px;
        line-height: 40px;

        a{
            color: $colorDarkBlue;
            text-decoration: none;

            &:hover{
                color: $colorGreen;
                text-decoration: underline;
            }
        }
    }
    
    .card-body{

        font-size: $fontLittle;

        a{
            text-decoration: none;
        }

        h5{
            color: $colorDarkBlue;
        }

        span{
            color: $colorFadeBlue;
        }

        .ms_span-left{
            &::before{
                @include awasomeAppend;
                content:'\f133'
            }
        }

        .ms_span-right{
            &::before{
                @include awasomeAppend;
                content:'\f06e'
            }
        }

        &:hover{
            h5{
                color: $colorGreen;
                text-decoration: underline;
            }
        }
    }
}
</style>