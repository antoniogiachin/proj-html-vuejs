<template>
<div class="row ro-cols-2 my-5">

    <div class="col my-5 px-3">
        <a class="ms_card-h" href="#" >
            <div class="row">
                <div class="col-md-4 p-2 d-flex align-items-center justify-content-center">
                    <div class="ms_course-img ">
                        <img :src='require("../../assets/img/course-02-480x298.jpg")'  alt="course-1">
                    </div>
                </div>
                <div class="col-md-8 p-2 d-flex align-items-center justify-content-center">
                    <div class="ms_card-body pe-4">
                        <h3 class="card-title"><span class="h2">$40.</span>00</h3>
                        <h4 class="card-title">Learning to write as a Professional Author</h4>
                        <span class="me-5 ms_span-card-left">20 Lessons</span>
                        <span class="ms-5 ms_span-card-right"> 50 Students</span>
                    </div>
                </div>
            </div>
        </a>
    </div>

</div>
</template>

<script>
export default {
    name: 'coursesCard',

    props: {

    }
}
</script>

<style lang="scss" scoped>

</style>