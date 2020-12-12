<template>
  <div class="profile">
    <img class="user_photo" src="../assets/photo.png" />
    <div class="user_info">
      <h2>Вероника Ростова</h2>
      <span>Менеджер по продажам</span>
    </div>
    <div class="title">
      <p>
        Подберу для вас самые лучшие предложения. Мои услуги абсолютно
        бесплатные
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Profile",
};
</script>

<style scoped>
.profile {
  max-width: 450px;
  justify-content: flex-start;
}

.user_photo {
  width: 124px;
  height: 124px;
  position: absolute;
  top: 19px;
}

.user_info {
  margin-left: 151px;
}

.title {
  max-width: 364px;
  border-radius: 5px;
  box-shadow: 0 0 0 1px rgba(60, 44, 0, 0.25);
  background-color: #fffbc8;
  margin-left: 87px;
  margin-top: 5px;
  padding-left: 41px;
  text-align: left;
}

@media screen and (max-width: 630px) {
  .user_photo {
    position: relative;
    margin-bottom: 19px;
  }

  .user_info {
    margin-left: 0;
  }

  .title {
    width: 90%;
    margin-left: 0;
  }
}
</style>
