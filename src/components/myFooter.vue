<template>
    <footer class="py-5">

        <div class="container">

            <div class="row">
                <div class="col-6">
                    <span class="d-inline-block mb-2">Explore</span>
                    <ul>

                        <li v-for="(adLink, index) in addressList" :key="index"><a :href="adLink.url">{{adLink.name}}</a> </li>
                        
                        <li><a href="#" v-for="(social, index) in footerSocial" :key="index"><i class="fab me-4" :class="social.class"></i></a> </li>
                        
                    </ul>
                </div>
                <div class="col-6">
                    <div class="row">
                        <div class="col-6">
                            <span class="d-inline-block mb-2">Explore</span>
                            <ul class="list-right d-flex flex-column">

                                <li v-for="(exLink, index) in exploreList" :key="index"><a :href="exLink.url">{{exLink.name}}</a> </li>
                        
                            </ul>   
                        </div>

                        <div class="col-4">
                            <span class="d-inline-block mb-2">Information</span>

                            <ul>

                                <li v-for="(infoLink, index) in informationList" :key="index"><a :href="infoLink.url">{{infoLink.name}}</a> </li>
                        
                            </ul> 
                        </div>
                    </div>
                </div>
            </div>

            <div class="text-center ms_copy mt-5">&copy; 2020 MaxCoach. All Rights Reserved</div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'myFooter',

    props: {
        
        "footerSocial" : Array,

        "footerLinks" : Array

    },

    computed:{

        // lista filtrata per address
        addressList: function (){
            return this.footerLinks.filter(value => {
                return value.address == true;
            })
        },

        // lista filtrata  per explore
        exploreList: function (){
            return this.footerLinks.filter(value => {
                return value.explore == true;
            })
        },

        // lista filtrata  per information
        informationList: function (){
            return this.footerLinks.filter(value => {
                return value.information == true;
            })
        },


    }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';

footer{
    background-color: $mostPopular;
    font-size: $fontLittle;
    font-weight: bolder;
    padding: 0px 80px;

    ul {
        list-style-type: none;
        line-height: 35px;
        padding: 0;

        li a{
            text-decoration: none;
            color: $colorFadeBlue;

            &:hover{
                color: $colorGreen;
            }
        }
    }

    .list-right{
        max-height: 120px;
        flex-wrap: wrap;
        
    }

    .ms_copy{
        color: $colorFadeBlue;
        font-size:  $fontLittle;;
    }
}
</style>