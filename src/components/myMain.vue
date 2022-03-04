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
        
    </main>
</template>

<script>
import sectionJumbo from './partials/sectionJumbo.vue'
import onlineCourses from './partials/onlineCourses.vue'
import smartTouring from './partials/smartTouring.vue'
import enjoyComp from './partials/enjoyComp.vue'


export default {
    name: 'myMain',

    components : {
        sectionJumbo,

        onlineCourses,

        smartTouring,

        enjoyComp,
    }
}
</script>

<style lang="scss" scoped>

</style>