<template>
    <main>
        <!-- sezione jumbotron -->
        <sectionJumbo/>

        <!-- sezione online courses -->
        <onlineCourses/>

        <!-- sezione smart touring -->
        <smartTouring/>
        
    </main>
</template>

<script>
import sectionJumbo from './partials/sectionJumbo.vue'
import onlineCourses from './partials/onlineCourses.vue'
import smartTouring from './partials/smartTouring.vue'


export default {
    name: 'myMain',

    components : {
        sectionJumbo,

        onlineCourses,

        smartTouring,
    }
}
</script>

<style lang="scss" scoped>

</style>