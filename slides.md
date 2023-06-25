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
<PageOne title="2023上半年工作总结" />
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
<PageFour />
---
layout: image
image: 'bg.jpg'
---
<PageFive />
---
layout: image
image: 'huawen.jpg'
transition: slide-up
---
<Page title="一点问题及建议">
<template #default>
<div class="slot">
<div style="text-indent: 2em; text-decoration: underline" v-click="1">
从以上的过程可以看出来，
稳定、明确的需求对代码的整体质量有明显重要的影响，
建议开发过程流程化，以原型为核心和驱动，
需求的变更从原型开始，到设计到开发到测试，
降低沟通成本，减少需求扯皮的情况，
对设计，可以整体把控产品的样式和美观
对开发，有明显清晰的开发需求
对测试，有清晰的测试参照
</div>
</div>
</template>
</Page>
