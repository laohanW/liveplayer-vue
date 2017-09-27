<template>
    <div class="root" @click="rootClick" bubble="true">
        <text style="font-size: 40px;">{{rootText}}</text>
        <div class="outer" @click="parentClick">
            <div>
                <text style="font-size: 40px;">{{parentText}}</text>
            </div>
            <text class="inner" @click="click">{{innerText}}</text>
        </div>
    </div>
</template>
<script>
    module.exports = {
        data: {
            innerText: 'click me',
            parentText: '',
            rootText: ''
        },
        methods: {
            clic: function (e) {
                this.innerText = 'inner bubble'
            },
            parentClick: function (e) {
                this.parentText = 'parent bubble'
            },
            rootClick: function (e) {
                this.rootText = 'root bubble'
            }
        }
    };
</script>
<style scoped>
    .inner {
        font-size: 40px;
        text-align: center;
        background-color: #7a9b1b;
        padding: 40px;
    }

    .outer {
        font-size: 40px;
        text-align: center;
        background-color: rgba(155, 122, 27, 0.4);
        padding: 120px;
    }

    .root {
        font-size: 40px;
        text-align: center;
        background-color: #7a1b9b;
        padding: 80px;
    }
</style>