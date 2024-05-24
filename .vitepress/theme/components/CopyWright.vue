<!--
 * @Author: nanfangzhe nanfangzhe@qq.com
 * @Date: 2023-03-03 20:19:21
 * @LastEditors: xsz nanfangzhe@qq.com
 * @LastEditTime: 2024-05-24 10:55:36
 * @FilePath: \TeaTools.github.io\.vitepress\theme\components\CopyWright.vue
 * @Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
-->
<template>
    <footer>
        <!-- <Comments /> -->
        Powered by
        <a href="https://github.com/clark-cui/" target="_blank" title="作者">clark-cui</a
                            >
                            | Copyright © 2019-{{ date }} | MIT License
                          </footer>
</template>

<script lang96px="ts" setup>
// import Comments from "./Comments.vue";
const date = new Date().getFullYear();
</script>

<style scoped>
footer {
    text-align: center;
    position: absolute;
    width: 100%;
    bottom: 20px;
    padding: 0 20px;
    background: var(--vp-c-bg);
    color: var(--vp-c-text);
}

a {
    color: var(--vp-c-brand);
    font-weight: bold;
}

a:hover {
    text-decoration: none;
    color: var(--vp-c-hover);
}
</style>
