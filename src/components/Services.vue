<template>
        <div class="services">
            Услуг
            <hr>
            <div><p class="services_1">Ручное бронирование</p><b class="right">11</b></div>
            <div><p class="services_2">Пакетные туры</p><b class="right">3</b></div>
            <div><p class="services_3">Отели</p><b class="right">1</b></div>
            <hr>
            <div><p class="font-weight-bold">Всего<b class="right">15</b></p></div>
        </div>

</template>

<script>
    export default {
        name: "Services"
    }
</script>

<style scoped>

    .services_1{
        width: 219px;
        height: 24px;
        background-color: #b1e19b;
        border-radius: 0px 2px 2px 0px;
        display: block;
        justify-content: start;
        float: left;
    }

    .services_2{
        width: 54px;
        height: 24px;
        background-color: #ace2f8;
        border-radius: 0px 2px 2px 0px;
        display: block;
        justify-content: start;
        float: left;
    }

    .services_3{
        width: 36px;
        height: 24px;
        background-color: #ace2f8;
        border-radius: 0px 2px 2px 0px;
        display: block;
        justify-content: start;
        float: left;
    }

    hr{
        margin-top: 7px;
        margin-bottom: 15px;
        height: 1px;
        color: #808080;
    }

    p{
        text-align: left;
        margin-bottom: 2px;
        padding-left: 7px;
    }

    .services {
        width: 319px;
        margin-top: 20px;
        margin-bottom: 28px;
        margin-left: 120px;
        text-align: right;
        display: flex;
        flex-direction: column;
    }
</style>