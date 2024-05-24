<template>
    <div id="gitalk-container">
    </div>
</template>

<script lang="ts" setup>
import "gitalk/dist/gitalk.css";
import Gitalk from "gitalk";
import { onMounted } from "vue";
// import { useData } from "vitepress";
// const relativePath = useData().page.value.relativePath;

const gitalk = new Gitalk({
    clientID: "Ov23licokG6VwYrzJEb3", // 修改 clinetID（参考：https://zhuanlan.zhihu.com/p/260781932）
    clientSecret: "80cbd3ead32aac4722bb7dc299079e6bd9ef6958",
    repo: "teatools.github.io",
    owner: "teatools",
    admin: ["teatools"],
    id: location.pathname.substring(0, 50), // Ensure uniqueness and length less than 50
    language: "zh-CN",
    distractionFreeMode: true, // Facebook-like distraction free mode
});

onMounted(() => {
    gitalk.render("gitalk-container");
});
</script>

<style scoped>

</style>
