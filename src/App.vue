<template>
    <div id="app" v-bind:style="{ backgroundColor: '#42b983'}">
        <router-view/>
    </div>
</template>

<script>
    import NavBar from '@/components/NavBar'
    import {Datetime} from 'vue-datetime';
    import {VueTuicalendar} from '@lkmadushan/vue-tuicalendar'
    import moment from 'moment'


    export default {
        components: {
            NavBar,
            moment,
            Datetime,
            VueTuicalendar,
        },
        name: 'App'

    }
</script>

<style>
    html, body {
        width: 100%;
        height: 100%;
        margin: 0;
        padding: 0;
    }

    #app {
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
        height: auto;
        min-height: 100%;

    }

    .row {
        /* display: -webkit-box; */
        /* display: -ms-flexbox; */
        display: flex;
        -ms-flex-wrap: wrap;
        flex-wrap: wrap;
        margin-right: -15px;
        margin-left: -15px;
    }

    .tile {
        position: relative;
        background: #ffffff;
        border-radius: 10px 10px 30px 10px;
        padding: 20px;
        -webkit-box-shadow: 0 2px 2px 0 rgba(0, 0, 0, 0.14), 0 1px 5px 0 rgba(0, 0, 0, 0.12), 0 3px 1px -2px rgba(0, 0, 0, 0.2);
        box-shadow: 0 2px 2px 0 rgba(0, 0, 0, 0.14), 0 1px 5px 0 rgba(0, 0, 0, 0.12), 0 3px 1px -2px rgba(0, 0, 0, 0.2);
        margin-bottom: 30px;
        -webkit-transition: all 0.3s ease-in-out;
        -o-transition: all 0.3s ease-in-out;
        transition: all 0.3s ease-in-out;
    }

    .col-1, .col-2, .col-3, .col-4, .col-5, .col-6, .col-7, .col-8, .col-9, .col-10, .col-11, .col-12, .col, .col-auto, .col-sm-1, .col-sm-2, .col-sm-3, .col-sm-4, .col-sm-5, .col-sm-6, .col-sm-7, .col-sm-8, .col-sm-9, .col-sm-10, .col-sm-11, .col-sm-12, .col-sm, .col-sm-auto, .col-md-1, .col-md-2, .col-md-3, .col-md-4, .col-md-5, .col-md-6, .col-md-7, .col-md-8, .col-md-9, .col-md-10, .col-md-11, .col-md-12, .col-md, .col-md-auto, .col-lg-1, .col-lg-2, .col-lg-3, .col-lg-4, .col-lg-5, .col-lg-6, .col-lg-7, .col-lg-8, .col-lg-9, .col-lg-10, .col-lg-11, .col-lg-12, .col-lg, .col-lg-auto, .col-xl-1, .col-xl-2, .col-xl-3, .col-xl-4, .col-xl-5, .col-xl-6, .col-xl-7, .col-xl-8, .col-xl-9, .col-xl-10, .col-xl-11, .col-xl-12, .col-xl, .col-xl-auto {
        position: relative;
        width: 100%;
        min-height: 1px;
        padding-right: 15px;
        padding-left: 15px;
    }

    .app-content {
        min-height: calc(100vh - 50px);
        margin-top: 10px;
        padding: 30px;
        -webkit-transition: margin-left 0.3s ease;
        -o-transition: margin-left 0.3s ease;
        transition: margin-left 0.3s ease;
    }

    .line-head {
        padding-bottom: 10px;
        border-bottom: 1px solid #ddd;
    }


</style>
