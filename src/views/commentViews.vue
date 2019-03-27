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
        margin-bottom: 9px;
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
        border: 1px solid rgba(0, 0, 0, 0.19);
        margin-bottom: 23px;
        padding: 15px 18px 15px 18px;
    }
</style>