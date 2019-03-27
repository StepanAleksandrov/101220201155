<template>
    <div class="profile">
        <img class="user_photo" src="../assets/photo.png">
        <div class="user_info">
            <h2>Вероника Ростова</h2>
            <h4>Менеджер по продажам</h4>
        </div>
        <div class="title">
            <p>Подберу для вас самые лучшие предложения.
                Мои услуги абсолютно бесплатные</p>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Profile"
    }
</script>

<style scoped>

    .profile {
        min-width: 440px;
        max-width: 449px;
    }

    h4 {
        color: #808080;
        font-family: "Arial - Bold MT";
        font-size: 12px;
        font-weight: 400;
        line-height: 20px;
        margin-bottom: 9px;
    }

    .user_photo {
        position: absolute;
    }

    .user_info {
        margin-left: 134px;
    }

    .title {
        max-width: 449px;
        border-radius: 1px;
        box-shadow: 0 0 0 1px rgba(60, 44, 0, 0.25);
        background-color: #fffbc8;
        margin-left: 87px;
        padding: 12px 15px 9px 47px;
    }
</style>