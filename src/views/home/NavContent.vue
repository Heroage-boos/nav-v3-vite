<template>
    <div class="container">
        <div class="column">
            <h3>左边栏</h3>
            <ul>
                <li>第一行数据</li>
                <li>第二行数据</li>
                <li>第三行数据</li>
            </ul>
        </div>
        <div class="column">
            <h3>中间栏</h3>
            <ul>
                <li>第一行数据</li>
                <li>第二行数据</li>
                <li>第三行数据</li>
            </ul>
        </div>
        <div class="column">
            <h3>右边栏</h3>
            <ul>
                <li>第一行数据</li>
                <li>第二行数据</li>
                <li>第三行数据</li>
            </ul>
        </div>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    name: 'NavContent',

});
</script>

<style lang="scss" scoped>
.container {
    display: flex;
    justify-content: space-between;
}

.column {
    width: 30%;
    padding: 20px;
    border: 1px solid #ccc;
    border-radius: 5px;
}

.column h3 {
    margin-top: 0;
}

ul {
    list-style: none;
    margin: 0;
    padding: 0;
}

li {
    margin-bottom: 10px;
}
</style>