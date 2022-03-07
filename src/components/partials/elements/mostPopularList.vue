<template>
    <ul class="fa-ul">
        <li v-for="(popular, index) in popularList" :key="index"> <a :href="popular.url"><span class="fa-li"><i class="fas fa-long-arrow-alt-right me-1"></i></span>{{popular.title}}</a> </li>
    </ul>
</template>

<script>
export default {
    name: 'mostPopularList',

    props : {
        "popularList" : Array,
    }
}
</script>

<style lang="scss" scoped>
// richiamo varibili create da me
@import "../../../assets/style/variables.scss";

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
</style>