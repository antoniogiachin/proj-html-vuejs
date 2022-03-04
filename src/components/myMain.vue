<template>
    <main>
        <!-- sezione jumbotron -->
        <sectionJumbo/>

        <!-- sezione online courses -->
        <onlineCourses/>

        <!-- sezione smart touring -->
        <smartTouring/>

        <!-- sezione enjoy companiionship -->
        <enjoyComp/>

        <!-- sezione varbatim quotes -->
        <verbatimQuotes/>

        <!-- sezione recap-flex -->
        <recapFlex/>

        <!-- sezione most popular -->
        <mostPopular/>

        <!-- sezione newsletter -->
        <myNewsLetter/>
        
    </main>
</template>

<script>
import sectionJumbo from './partials/sectionJumbo.vue'
import onlineCourses from './partials/onlineCourses.vue'
import smartTouring from './partials/smartTouring.vue'
import enjoyComp from './partials/enjoyComp.vue'
import verbatimQuotes from './partials/verbatimQuotes.vue'
import recapFlex from './partials/recapFlex.vue'
import mostPopular from './partials/mostPopular.vue'
import myNewsLetter from './partials/myNewsLetter.vue'





export default {
    name: 'myMain',

    components : {
        sectionJumbo,

        onlineCourses,

        smartTouring,

        enjoyComp,

        verbatimQuotes,

        recapFlex,

        mostPopular,

        myNewsLetter,
        
    }
}
</script>

<style lang="scss" scoped>

</style>