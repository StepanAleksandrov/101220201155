<template>
    <div>
        <div><h3>{{comment.user_name}} <span>{{comment.data}}</span></h3></div>

        <div class="comment"><p>{{comment.text}}</p></div>
    </div>
</template>

<script>
    export default {
        name: "comment",
        props: ['comment'],
    }
</script>

<style scoped>

    h3 {
        color: #333333;
        font-family: "Arial - Bold MT";
        font-size: 14px;
        font-weight: 700;
        line-height: 20px;
    }

    span{
        color: #808080;
        font-family: "Arial - Bold MT";
        font-size: 11px;
        font-weight: 400;
        line-height: 20px;
        margin-left: 7px;
    }

    .comment {
        width: 449px;
        border: 18px solid #808080;
        border-image: url("../assets/com.png") 25 round stretch;
        margin-bottom: 20px;
    }
</style>