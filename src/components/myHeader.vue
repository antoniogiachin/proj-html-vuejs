<template>

    <header class="ms_header">

        <div class="container">

            <!-- navbar bootstrap -->
            <nav class="navbar navbar-expand-lg ">
                <div class="container-fluid">

                    <!-- logo dimensioni width 50% -->
                    <a class="navbar-brand" href="#">
                        <img src="../assets/img/dark-logo.png" class="w-50" alt="navbar-logo">
                    </a>
                    
                    <!-- lista link dinamica, ad ogni link in after fontawasome freccia giu' -->
                    <ul class="navbar-nav ms-auto me-3">
                        
                        <li class="nav-item " v-for="(link, index) in navLinks" :key="index">
                            <a class="nav-link ms_nav-link" :href="link.url">{{link.name}}</a>
                        </li>

                        

                        <li class="nav-item">
                            <a class="nav-link text-dark" href="#">
                                <i class="fa-regular fa-circle-user"></i>
                            </a>
                        </li>
                                                                
                    </ul>

                    <!-- form stilizzato da me  -->
                    <form class="d-flex align-items-center px-2 rounded-2 ms_form">
                        <input class="form-control me-2 bg-transparent border-0 ms_input" type="search" placeholder="Search..." aria-label="Search">
                        <a href="#"><i class="fa-solid fa-magnifying-glass ms_search-icon"></i></a>        
                    </form>
                    
                </div>
            </nav>
        </div>

    </header>

</template>

<script>
export default {
    name: 'myHeader',

    //ricevo oggetto props da app'
    props: {
        "navLinks" : Array,
    }
}
</script>

<style lang="scss" scoped>
// richiamo varibili create da me
@import "../assets/style/variables.scss";

.ms_header{
    box-shadow: 0px 3px 10px $colorGrey;
    font-size: $fontLittle;

    .ms_nav-link{

        color: $colorDarkFirst;

        &:hover{
            color: $colorGreen;
        }


        &::after{
            display: inline-block;
            text-rendering: auto;
            -webkit-font-smoothing: antialiased;
            font: var(--fa-font-solid);
            content: "\f078";
            margin: 0px 5px;
        }
    }

    .fa-circle-user:hover{
        transform: scale(1.2);
        color: $colorGreen;
    }


    .ms_form {
        background-color: $colorLightGrey;
        
        .ms_input{
            outline: none !important;

        }

        .ms_search-icon{
            color: $colorGreen;
        }
    }


}


</style>