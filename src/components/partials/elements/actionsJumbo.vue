<template>
    <div class="ms_actions d-flex flex-column align-items-center position-absolute rounded-start">
        <a :href="action.url" v-for="(action, index) in actionLinks" :key="index" class="text-dark"><i class="fas" :class="action.icon"></i></a>
    </div>
</template>

<script>
export default {
    name: 'actionsJumbo',

    props : {
        "actionLinks" : Array
    }
}
</script>

<style lang="scss" scoped>
// richiamo varibili create da me
@import "../../../assets/style/variables.scss";

.ms_actions{
    gap: 10px;
    right: 0;
    box-shadow: 0px 3px 10px $colorGrey;
    padding: 5px;
    font-size: $fontLittle;
}
</style>