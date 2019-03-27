<template>
    <div id="app">
        <Profile/>
        <Services/>
        <Comments/>
    </div>
</template>

<script>
    import Comments from './components/Comments'
    import Profile from './components/Profile'
    import Services from './components/Services'

    export default {
        name: 'app',
        components: {
            Comments,
            Profile,
            Services
        }
    }
</script>

<style>
    #app {
        padding-top: 20px;
        display: flex;
        flex-wrap: wrap;
        display: -webkit-flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        margin: auto;
    }

    h2 {
        color: #333333;
        font-family: Arial;
        font-size: 16px;
        font-weight: 700;
        padding-top: 7px;
        padding-right: 7px;
    }

    p {
        color: #333333;
        font-family: "Arial MT";
        font-size: 14px;
        font-weight: 400;
        line-height: 19px;
        margin: 0px;
    }

</style>
