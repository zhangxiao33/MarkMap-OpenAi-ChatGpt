<template>
    <div class="about-container">
        <h1>关于</h1>
        <MarkdownRenderer :content="markdownContent" />
<h4>原项目收款码让我删了，免费的东西不收钱,要支持上主页点个赞好了</h4>
    </div>
</template>

<script>
import MarkdownRenderer from '@/components/MarkdownRenderer.vue';

export default {
    name: 'About',
    components: {
        MarkdownRenderer,
    },
    data() {
        return {
            markdownContent: `
# 开发的目的

_开源是为了_ 让所有朋友用上免费的 GPT AI 思维导图。

# 作者

**原作者**
PastKing

**现作者**
MistPeak

# 原项目地址(GitHub)

[MarkMap-OpenAi-ChatGpt](https://github.com/PastKing/MarkMap-OpenAi-ChatGpt)

# 现项目地址(GitHub)

[MarkMap-OpenAi-ChatGpt](https://github.com/zhanghxiao/MarkMap-OpenAi-ChatGpt)

# 项目改进

原项目仅支持通过标题生成思维导图，并可进行编辑。

优化后的项目不仅可以通过标题生成思维导图，还可以添加参考资料进行编辑。

# 赞助/支持
`
        };
    }
};
</script>

<style scoped>
.about-container {
    padding: 20px;
    max-width: 800px;
    margin: 0 auto;
    font-family: Arial, sans-serif;
}

h1 {
    text-align: center;
    color: #2c3e50;
    margin-bottom: 20px;
}

.donation-qr-code {
    display: block;
    margin: 20px auto;
    width: 200px;
    border: 1px solid #ccc;
    border-radius: 10px;
}
</style>
