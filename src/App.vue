<template>
  <div id="app">
    <Profile />
    <Services />
    <Comments />
  </div>
</template>

<script>
import Comments from "./components/Comments";
import Profile from "./components/Profile";
import Services from "./components/Services";

export default {
  name: "app",
  components: {
    Comments,
    Profile,
    Services,
  },
};
</script>

<style>
#app {
  max-width: 487px;
  min-width: 360px;
  display: flex;
  flex-wrap: wrap;
  box-sizing: border-box;
  display: -webkit-flex;
  align-items: flex-start;
  padding: 19px;
  margin: auto;
}

.row {
  display: flex;
  flex-direction: row;
  align-items: center;
}

h2 {
  height: 20px;
  font-family: Arial;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 20px;
  margin-top: 7px;
  margin-bottom: 2px;
  color: #333333;
}

h3 {
  width: 450px;
  height: 21px;
  font-family: Arial;
  font-style: normal;
  font-weight: bold;
  font-size: 14px;
  line-height: 19px;
  color: #333333;
}

span {
  width: auto;
  height: 20px;
  font-family: Arial;
  font-style: normal;
  font-weight: normal;
  font-size: 12px;
  line-height: 20px;
  margin-bottom: 9px;
  color: #808080;
}

p {
  color: #333333;
  font-family: "Arial";
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 19px;
  padding-top: 10px;
  padding-bottom: 11px;
  margin-bottom: 0;
}
</style>
