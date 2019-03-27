<template>
    <div class="services">
        <span>Услуг</span>
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

    .services_1 {
        width: 219px;
        height: 24px;
        background-color: #b1e19b;
        border-radius: 0px 2px 2px 0px;
        display: block;
        justify-content: start;
        float: left;
    }

    .services_2 {
        width: 54px;
        height: 24px;
        background-color: #ace2f8;
        border-radius: 0px 2px 2px 0px;
        display: block;
        justify-content: start;
        float: left;
    }

    .services_3 {
        width: 36px;
        height: 24px;
        margin-bottom: 8px;
        background-color: #ace2f8;
        border-radius: 0px 2px 2px 0px;
        display: block;
        justify-content: start;
        float: left;
    }

    hr {
        margin-top: 7px;
        margin-bottom: 15px;
        height: 1px;
        color: #808080;
        opacity: 0.4;
    }

    p {
        text-align: left;
        margin-bottom: 2px;
        padding-left: 7px;
    }

    b {
        padding-right: 41px;
    }

    span {
        color: #333333;
        font-family: "Arial MT";
        font-size: 14px;
        font-weight: 400;
        line-height: 19px;
        margin: 0px;
        padding-right: 34px;
    }

    .services {
        width: 319px;
        margin-top: 15px;
        margin-bottom: 28px;
        margin-left: 120px;
        text-align: right;
        display: flex;
        flex-direction: column;
    }
</style>