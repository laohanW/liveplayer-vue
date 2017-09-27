<template>
    <div>
        <list>
            <cell v-for="l in lists">
                <div class="panel">
                    <text>{{l}}</text>
                </div>
            </cell>
        </list>
    </div>
</template>

<script>
    export default {
        data: function () {
            return {
                name: ''
            }
        }
    }
</script>

<style>
    .topheader {
        background-color: red;
        padding: 10px;
    }

    .panel {
        width: 600px;
        height: 25px;
        margin-left: 75px;
        margin-right: 75px;
        margin-top: 3px;
        margin-bottom: 3px;
        flex-direction: column;
        justify-content: center;
        border-width: 2px;
        border-style: solid;
    }

    .textImage {
        width: 700px;
        height: 250px;
    }

    .textInput {
        height: 80px;
        padding: 10px;
        font-size: 32px;
        width: 750px;
        /*border-top-width:1px;*/
        border-bottom-width: 1px;
    }

    .top-text {
        color: #00BDFF;
        font-size: 46px;
        text-align: center;
        lines: 1;
    }
</style>