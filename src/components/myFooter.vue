<template>
    <footer class="py-5">

        <div class="container">

            <div class="row">
                <div class="col-6">
                    <span class="d-inline-block mb-2">Explore</span>
                    <ul>
                        <li><a href="#">382 NE 191st St # 87394 Miami, FL 33179-3899</a> </li>
                        <li><a href="#">+1(305)547-9909(9am - 5pm EST, Monday - Friday)</a> </li>
                        <li><a href="#">support@MaxCoach.com</a> </li>
                        <li><a href="#"><i class="fab fa-twitter"></i></a> </li>
                        
                    </ul>
                </div>
                <div class="col-6">
                    <div class="row">
                        <div class="col-6">
                            <span class="d-inline-block mb-2">Explore</span>
                            <ul class="list-right d-flex flex-column">

                                <li><a href="#">Start Here</a> </li>
                                <li><a href="#">Blog</a> </li>
                                <li><a href="#">About us</a> </li>
                                <li><a href="#">About us</a> </li>
                                <li><a href="#">About us</a> </li>
                                <li><a href="#">About us</a> </li>
                        
                            </ul>   
                        </div>

                        <div class="col-4">
                            <span class="d-inline-block mb-2">Information</span>

                            <ul>

                                <li><a href="#">Membership</a> </li>
                                <li><a href="#">Purchase Guide</a> </li>
                                <li><a href="#">Privacy Policy</a> </li>
                                <li><a href="#">Privacy Policy</a> </li>
                        
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
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';

footer{
    background-color: $mostPopular;
    padding: 0px 80px;

    ul {
        list-style-type: none;
        line-height: 35px;
        padding: 0;

        li a{
            text-decoration: none;
            color: $colorFadeBlue
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