<template>
<div class="row mt-4">
    <div class="col d-flex align-items-center justify-content-center" v-for="(client, index) in clients" :key="index">
        <img :src='require("../../../assets/img/" + client.url)' class="ms_client-img" alt="client">
    </div>  
</div>
</template>

<script>
export default {
    name: 'clientsJumbo',

    props : {

        "clients" : Array,

    },

}
</script>

<style lang="scss" scoped>
.ms_client-img{
    filter: opacity(0.5);
}
</style>