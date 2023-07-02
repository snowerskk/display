---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/collection/94734566/1920x1080
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# persist drawings in exports and build
drawings:
  persist: false
# page transition
transition: fade-out
# use UnoCSS
css: unocss
---

# 述 职 报 告
It is the unforeseen that always happens.

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    陈 龙 <carbon:arrow-right class="inline"/>
  </span>
</div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
layout: image
image: 'bg2.jpg'
---
<PageOne />
<!--
You can have `style` tag in markdown to override the style for the current page.
Learn more: https://sli.dev/guide/syntax#embedded-styles
-->

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>
---
layout: image
image: 'bg.jpg'
---
<PageTwo />
---
layout: image
image: 'bg.jpg'
---
<PageThree />
---
layout: image
image: 'bg.jpg'
---
<PageEight />
---
layout: image
image: 'bg.jpg'
---
<PageFour />
---
layout: image
image: 'bg.jpg'
---
<PageFive />
---
layout: image
image: 'bg.jpg'
---
<PageSix />
---
layout: image
image: 'huawen.jpg'
transition: slide-up
---
<Page title="存在的问题">
<template #default>
<div class="slot">
<div style="text-indent: 2em;" v-click="1">
由于将一部分代码逻辑转移到了业务中台，同时由于存在多个不同的项目和多个不同的服务器环境，出现了代码与表单配置、代码与服务器环境、表单配置与服务器环境三者之间相互多对多的情况，由此产生的问题：
</div>
<Item v-click="2" text="1.配置表单占了较大的工作量，测试提的bug有相当一部分是配置问题" />
<Item v-click="3" text="2.同时在多个项目与环境之间来回切换，极大增加了开发难度" />
<Item v-click="4" text="3.降低了开发效率，增加了出bug的可能" />
</div>
</template>
</Page>
---
<End />