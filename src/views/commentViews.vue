<template>
  <div>
    <div>
      <h3>
        {{ comment.user_name }} <span>{{ comment.data }}</span>
      </h3>
    </div>

    <div class="comment">
      <p>{{ comment.text }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "comment",
  props: ["comment"],
};
</script>

<style scoped>
.comment {
  max-width: 450px;
  border: 11px solid;
  box-shadow: 0px 4px 10px rgba(128, 128, 128, 0.1);
  border-image: url("../assets/com.svg") 11 stretch;
  margin-bottom: 20px;
}

@media screen and (max-width: 630px) {
  .comment {
    width: 70%;
  }
}
</style>
