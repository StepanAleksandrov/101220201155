<template>
    <div class="column">
        <div class="row">
            <div class="row">
                <h2>Последние отзывы</h2>
                <p><a href="#">Все отзывы</a></p>
            </div>

            <div class="row">
                <div class=""><p><img src="../assets/like.png" alt="">131</p></div>
                <div><img src="../assets/comments.png" alt="">14</div>
            </div>
        </div>
        <div class="comments">
            <commentViews v-for="comment in comments" :comment="comment"/>
            <textarea type="text" class="send_comment" v-model="text_" value="text_"
                      v-on:keyup.ctrl.enter="sendComment"></textarea>
        </div>
        <button class="submite" v-on:click="click">
            <p>Написать консультанту</p>
        </button>
    </div>
</template>

<script>
    import commentViews from '../views/commentViews'

    export default {
        name: "Comments",
        data() {
            return {
                text_: '',
                months: ["январь", "февраль", "март", "апрель", "май", "июнь",
                    "июль", "август", "сентябрь", "октябрь", "ноябрь", "декабрь"],
                comments: [
                    {
                        id: 1,
                        user_name: 'Самуил',
                        data: '13 октября 2011',
                        text: 'Привет, Верунь! ниче себе ты крутая. фотка ' +
                        '' +
                        'класс!!!!'
                    },
                    {
                        id: 2,
                        user_name: 'Лилия Семёновна',
                        data: '14 октября 2011',
                        text: 'Вероника, здравствуйте! Есть такой ' +
                        'вопрос: Особый вид куниц жизненно стабилизирует кинетический момент, это и есть всемирно ' +
                        'известный центр огранки алмазов и торговли бриллиантами?'
                    },
                    {
                        id: 3,
                        user_name: 'Лилия Семёновна',
                        data: '14 октября 2011',
                        text: 'Вероника, здравствуйте! Есть такой ' +
                        'вопрос: Особый вид куниц жизненно стабилизирует кинетический момент?'
                    }
                ]
            }
        },
        components: {
            commentViews
        },
        methods: {

            click: function () {

                var today = new Date();
                var dd = today.getDate();
                var mm = this.months[today.getMonth()];
                var yyyy = today.getFullYear();

                today = dd + ' ' + mm + ' ' + yyyy;
                this.comments.push({id: Math.random(10), user_name: 'User_1', data: today, text: this.text_});
                this.text_ = '';
            },

            sendComment: function () {

                var today = new Date();
                var dd = today.getDate();
                var mm = this.months[today.getMonth()];
                var yyyy = today.getFullYear();

                today = dd + ' ' + mm + ' ' + yyyy;
                this.comments.push({id: Math.random(10), user_name: 'User_1', data: today, text: this.text_});
                this.text_ = '';
            }
        }
    }
</script>

<style scoped>

    img {
        padding-right: 5px;
    }

    img:last-child {
        padding-left: 21px;
        padding-top: -10px;
    }

    h2 {
        padding-top: 0px;
    }

    .row {
        display: flex;
        margin-bottom: 10px;
    }

    a {
        margin-right: 105px;
    }

    .send_comment {
        width: 449px;
        height: 65px;
        margin-top: 30px;
        padding: 15px;
        border: 1px solid rgba(0, 0, 0, 0.19);
        background-color: #ffffff;
        display: flex;
    }

    .submite {
        width: 282px;
        height: 43px;
        margin-top: 34px;
        border: none;
        border-radius: 20px;
        background-color: #fdd639;
        margin-left: 84px;

    }
</style>