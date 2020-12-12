<template>
  <div class="services">
    <span>Услуг</span>
    <hr />
    <div class="row">
      <div class="container">
        <div class="services_booking">
          <span class="absolute">Ручное бронирование</span>
        </div>
      </div>
      <b class="right">11</b>
    </div>
    <div class="row">
      <div class="container">
        <div class="services_tours">
          <span class="absolute">Пакетные туры</span>
        </div>
      </div>

      <b class="right">3</b>
    </div>
    <div class="row">
      <div class="container">
        <div class="services_hotels"><span class="absolute">Отели</span></div>
      </div>
      <b class="right">1</b>
    </div>
    <hr />
    <div class="row">
      <p class="font-weight-bold">
        Всего
      </p>
      <b class="font-weight-bold right">15</b>
    </div>
    <div class="vl"></div>
  </div>
</template>

<script>
export default {
  name: "Services",
};
</script>

<style scoped>
.container {
  max-height: 26px;
  position: relative;
  display: contents;
}

.row {
  justify-content: space-between;
  flex-wrap: nowrap;
}

.absolute {
  position: absolute;
}

.services {
  width: 319px;
  margin-top: 13px;
  margin-bottom: 20px;
  margin-left: 130px;
  text-align: right;
  display: flex;
  flex-direction: column;
  position: relative;
}

.services_booking {
  width: 219px;
  height: 24px;
  background-color: #b1e19b;
  border-radius: 0px 3px 3px 0px;
  display: block;
  text-align: left;
  padding-left: 6px;
  margin-bottom: 2px;
  float: left;
  color: #333333;
}

.services_tours {
  width: 54px;
  height: 24px;
  border-radius: 0px 3px 3px 0px;
  text-align: left;
  padding-left: 6px;
  display: flex;
  margin-bottom: 2px;
  float: left;
  background-color: #ace2f8;
}

.services_hotels {
  width: 36px;
  height: 24px;
  margin-bottom: 8px;
  border-radius: 0px 3px 3px 0px;
  text-align: left;
  padding-left: 6px;
  margin-bottom: 2px;
  display: block;
  float: left;
  background-color: #ace2f8;
}

hr {
  margin-top: 7px;
  margin-bottom: 15px;
  height: 1px;
  color: #808080;
  opacity: 0.4;
}

.font-weight-bold {
  text-align: left;
  margin-bottom: 2px;
  padding-left: 7px;
  padding-bottom: 0;
  padding-top: 0;
}

b {
  padding-right: 41px;
  padding-left: 15px;
  line-height: 20px;
}

span {
  color: #333333;
  font-size: 13px;
  line-height: 26px;
  margin: 0px;
  padding-right: 34px;
}

.vl {
  border-left: 1px solid rgba(51, 51, 51, 0.2);
  height: 76px;
  position: absolute;
  left: 0;
  top: 44px;
}

@media screen and (max-width: 850px) {
  .services {
    margin-top: 25px;
    margin-left: 0;
  }
}
</style>
