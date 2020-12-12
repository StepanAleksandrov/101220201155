<template>
  <div>
    <div class="comments_info">
      <div class="row">
        <h2>Последние отзывы</h2>
        <p><a href="#">Все отзывы</a></p>
      </div>

      <div class="row">
        <div><img src="../assets/like.png" alt="" /> 131</div>
        <div><img src="../assets/comments.png" alt="" />14</div>
      </div>
    </div>
    <div class="comments">
      <commentViews
        v-for="comment in comments"
        :key="comment.id"
        :comment="comment"
      />
      <textarea
        type="text"
        class="send_comment"
        v-model="text_"
        value="text_"
        v-on:keyup.ctrl.enter="sendComment"
      ></textarea>
    </div>

    <button class="submite" v-on:click="sendComment">
      <p>Написать консультанту</p>
    </button>
  </div>
</template>

<script>
import commentViews from "../views/commentViews";
import data from "../data";

export default {
  name: "Comments",
  data() {
    return data;
  },
  components: {
    commentViews,
  },
  methods: {
    sendComment: function() {
      var today = new Date();
      var dd = today.getDate();
      var mm = this.months[today.getMonth()];
      var yyyy = today.getFullYear();

      today = dd + " " + mm + " " + yyyy;
      this.text_
        ? this.comments.push({
            id: Math.random(10),
            user_name: "User_1",
            data: today,
            text: this.text_,
          })
        : (this.text_ = "");
      this.text_ = "";
    },
  },
};
</script>

<style scoped>
img {
  width: auto;
  height: 14px;
  padding-right: 4px;
}

img:last-child {
  padding-left: 16px;
}

h2 {
  margin-top: 0px;
  margin-bottom: 0px;
}

p {
  padding-top: 0px;
  padding-bottom: 0px;
}

.comments {
  margin-top: 10px;
}

.comments_info {
  display: flex;
  flex-direction: row;
  align-items: center;
}

a {
  margin-right: 97px;
  margin-left: 9px;
}

.send_comment {
  width: 100%;
  height: 65px;
  resize: none;
  margin-top: 10px;
  padding: 15px;
  border: 1px solid #000000;
  background-color: #ffffff;
}

.submite {
  width: 282px;
  height: 43px;
  margin-top: 34px;
  border: none;
  border-radius: 20px;
  background-color: #fdd639;
  margin-left: 87px;
}

@media screen and (max-width: 630px) {
  .comments {
    width: 100%;
  }
  .send_comment {
    width: 80%;
  }

  .comments_info {
    flex-direction: column;
    align-items: flex-start;
  }

  .submite {
    margin-left: 40px;
  }
}
</style>
