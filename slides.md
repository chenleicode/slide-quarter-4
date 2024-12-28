---
# You can also start simply with 'default'
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
# background: https://cover.sli.dev
background: /home.jpg
# 网页的标题模板，`%s` 会被页面的标题(title)替换。默认值是 %s - Slidev
titleTemplate: '%s'
# some information about your slides (markdown enabled)
title: Slidev | 程序员的演示文稿工具
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# apply unocss classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
# take snapshot for each slide in the overview
overviewSnapshots: true # TODO 暂时没有明白什么意思
# HTML 标签属性
htmlAttrs:
  lang: zh
---

# Slidev | 程序员的演示文稿工具

分享人：陈磊

<div class="abs-br m-6 flex gap-2">
  <a href="https://github.com/chenlei0608/slide-quarter-4" target="_blank" alt="GitHub" title="GitHub 地址"
    class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
  <a href="https://chenlei0608.github.io/blog/" target="_blank" alt="GitHub" title="陈磊的博客"
    class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:earth-americas-filled />
  </a>
</div>



---
transition: fade-out
---

# 什么是 Slidev ？

Slidev 是一个为开发者设计的幻灯片制作和演示工具，具有以下特点：

- 📝 **Markdown 支持** - 专注于使用 Markdown 编写内容，然后再进行样式优化
- 🎨 **可主题化** - 主题可以作为 npm 包共享和重用
- 🧑‍💻 **对开发者友好** - 代码高亮、实时编码和自动补全
- 🤹 **交互性** - 嵌入 Vue 组件以增强表达
- 🎙 **演示者模式** - 可以使用另一个窗口，甚至是你的手机来控制幻灯片
- 🎥 **录制功能** - 内置录制和摄像头视图
- 📤 **便携性** - 导出为 PDF、PPTX、PNG，甚至是可托管的单页应用
- 🛠 **可定制** - 几乎任何在网页上可能实现的功能都可以在 Slidev 中实现

<br>
<br>

阅读更多关于 [为什么选择 Slidev？](https://sli.dev/guide/why)

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

<!-- 
Microsoft PowerPoint 和 Apple Keynote 。它们直观易学。

Slidev 旨在为程序员制作的幻灯片提供极强的灵活性和交互性，并帮助程序员使用熟悉的技术来使演示更加有趣、有表现力和吸引力。

Slidev 的幻灯片以 Markdown 的格式编写。这帮助您专注于内容。同时，Slidev 的幻灯片在浏览器中呈现，这意味着几乎没有什么效果不可能被实现，一切您在 Web 应用中能做的都可以应用到您的幻灯片中。

使用场景：面向开发团队的技术分享，主题演讲，学术研究与报告...
-->



---
transition: fade-out
---

# Slidev 技术栈

Slidev 基于以下工具和技术构建：

- [**Vite**](https://vitejs.dev) - 一款极速响应的下一代的前端工具链
- [**Vue 3**](https://v3.vuejs.org/) powered [**Markdown**](https://daringfireball.net/projects/markdown/syntax) - 用于编写幻灯片内容
- [**UnoCSS**](https://github.com/unocss/unocss) - 帮助快速构建幻灯片样式
- [**Shiki**](https://github.com/shikijs/shiki), [**Monaco Editor**](https://github.com/Microsoft/monaco-editor) - 为在幻灯片中嵌入代码提供一流支持
- [**RecordRTC**](https://recordrtc.org) - 内置的录制工具和摄像头视图
- [**VueUse**](https://vueuse.org) 系列 - [`@vueuse/core`](https://github.com/vueuse/vueuse), [`@vueuse/head`](https://github.com/vueuse/head), [`@vueuse/motion`](https://github.com/vueuse/motion), 等等
- [**Iconify**](https://iconify.design/) - 用图标集丰富你的幻灯片
- [**Drauu**](https://github.com/antfu/drauu) - 用于在幻灯片上绘图和批注
- [**KaTeX**](https://katex.org/) - 用于渲染 LaTeX 数学公式
- [**Mermaid**](https://mermaid-js.github.io/mermaid) - 基于文本的图表绘制工具
- ...

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
layout: intro
glowSeed: 15
glowOpacity: 0.3
class: pl-30
---

# Anthony Fu

<div class="[&>*]:important-leading-10 opacity-80">

<a href="https://vitejs.dev" target="_blank" class="no-underline">Vite</a>, 
<a href="https://vuejs.org" target="_blank" class="no-underline">Vue</a>, 
<a href="https://nuxtjs.org" target="_blank" class="no-underline">Nuxt</a> 核心团队成员<br>
<a href="https://vitest.dev" target="_blank" class="no-underline">Vitest</a>, 
<a href="https://sli.dev" target="_blank" class="no-underline">Slidev</a>, 
<a href="https://github.com/unocss/unocss" target="_blank" class="no-underline">UnoCSS, </a>
<a href="https://github.com/type-challenges/type-challenges" target="_blank" class="no-underline">Type Challenges, </a>
<a href="https://elk.zone" target="_blank" class="no-underline">Elk</a> 作者<br>
<a href="https://github.com/eslint-stylistic/eslint-stylistic" target="_blank" class="no-underline">ESLint Stylistic, </a>
<a href="https://shiki.matsu.io" target="_blank" class="no-underline">Shiki, </a>
<a href="https://github.com/microsoft/TypeScript-Twoslash" target="_blank" class="no-underline">Twoslash, </a>
<a href="https://github.com/wenyan-lang/wenyan" target="_blank" class="no-underline">wen-yan lang</a> 维护者<br>
就职于 <a href="https://nuxtlabs.com" target="_blank" class="no-underline">NuxtLabs</a><br>

</div>

<div my-10 w-min flex="~ gap-1" items-center justify-center>
  <div i-ri-user-3-line op50 ma text-xl></div>
  <div><a href="https://antfu.me" target="_blank" class="border-none! font-300">antfu.me</a></div>
  <div i-ri-github-line op50 ma text-xl ml4></div>
  <div><a href="https://github.com/antfu" target="_blank" class="border-none! font-300">antfu</a></div>
  <div i-ri-bluesky-line op50 ma text-xl ml4></div>
  <div><a href="https://bsky.app/antfu.me" target="_blank" class="border-none! font-300">antfu.me</a></div>
  <div i-ri-twitter-x-line op50 ma text-xl ml4></div>
  <div><a href="https://twitter.com/antfu7" target="_blank" class="border-none! font-300">antfu7</a></div>
  <div i-ri-bilibili-line op50 ma text-xl ml4></div>
  <div><a href="https://space.bilibili.com/668380" target="_blank" class="border-none! font-300" ws-nowrap>AnthonyFu 一个托尼</a></div>
</div>

<img src="https://antfu.me/avatar.png" absolute top-36 right-30 w-40 rounded-full />

<style>
.no-underline {
  border-bottom-width: 0;
}
</style>


---
transition: slide-up
level: 2
---

# 导航控制面板

将鼠标悬停在左下角以查看导航控制面板，[了解更多](https://cn.sli.dev/guide/ui#navigation-bar)

## 键盘快捷键

|     |     |
| --- | --- |
| <kbd>右</kbd> / <kbd>空格</kbd>| 下一个动画或幻灯片 |
| <kbd>左</kbd>  / <kbd>Shift</kbd><kbd>空格</kbd> | 上一个动画或幻灯片 |
| <kbd>上</kbd> | 上一张幻灯片 |
| <kbd>下</kbd> | 下一张幻灯片 |

<img
  v-click
  class="absolute -bottom-9 -left-7 w-80 opacity-50"
  src="https://sli.dev/assets/arrow-bottom-left.svg"
  alt=""
/>
<p v-after class="absolute bottom-23 left-45 opacity-30 transform -rotate-10">这儿!</p>



---
transition: fade-out
---

# 演讲者模式

点击 <carbon-user-speaker class="inline-icon-btn"/> 按钮或访问 `http://localhost:<port>/presenter` 来进入演讲者模式。

<div v-click>
在演讲中，建议打开两个浏览器窗口：一个在播放模式用于观众，另一个在演讲者模式用于你。然后你可以将第一个屏幕分享给观众，保留第二个屏幕给自己。每当你在演讲者模式中导航时，观众的屏幕也会同步更新。
</div>

<div v-click class="mt3">
  <img src="/presenter-mode.png" style="height: 320px" />
</div>



---
transition: fade-out
---

# 快速上手

<div v-click class="mt5">
1. 在终端运行以下命令:
</div>

<div v-click class="mt3">

```sh
npm init slidev@latest # npm
pnpm create slidev # pnpm
yarn create slidev # yarn
```

</div>

<div v-click class="mt8">
2. 根据指引，并按照提示完成项目创建
</div>

<div v-click class="mt3">
<img src="/get-started-tip.png" style="height: 230px" />
</div>



---

<img src="/quick-start.png" style="height: 100%; display: block; margin: 0 auto;" />


---
transition: fade-out
---

# Frontmatter & Headmatter

在每张幻灯片的开头，你可以添加一个可选的 frontmatter 来配置幻灯片。第一个 frontmatter 块称为 headmatter，可以配置整个幻灯片集。其余的是用于单个幻灯片的 frontmatters

```md
---
theme: seriph
title: Welcome to Slidev
---

# 第一页

第一页的 frontmatter 也是整个演示文稿的 headmatter

---
layout: center
background: /background-1.png
---

# 第二页

本页的布局是 `center`，背景是一张图片
```



---
transition: fade-out
---

# 备注

每张幻灯片的末尾的注释，将被视为幻灯片的备注。它们将在用户界面中显示，以供您在演示过程中参考

```md
---
layout: cover
---

# 第一页

封面页

<!-- 这是一段备注 -->

```



---
transition: fade-out
---

# 代码块

```ts  twoslash
/**
 * 钉钉环境下的标题设置
 */

import { onMounted } from 'vue'

export function useDDTitle(ddTitle: string) {
  function setTitle(ddTitle: string) {
      window.dd.biz.navigation.setTitle({
        title: ddTitle,
      })
  }

  onMounted(() => {
    setTitle(ddTitle)
  })
}
```

<arrow v-click x1="650" y1="220" x2="455" y2="275" color="#953" width="2" arrowSize="1" />


---
level: 2
---

# Shiki Magic Move

由 [shiki-magic-move](https://shiki-magic-move.netlify.app/) 提供支持，Slidev 支持跨多个代码片段的动画效果。

添加多个代码块并用 <code>````md magic-move</code>（四个反引号）包裹它们以启用魔法移动。例如：

````md magic-move {lines: true}
```ts {*|2|*}
// 第一步
const author = reactive({
  name: 'John Doe',
  books: [
    'Vue 2 - Advanced Guide',
    'Vue 3 - Basic Guide',
    'Vue 4 - The Mystery'
  ]
})
```

```ts {*|1-2|3-4|3-4,8}
// 第二步
export default {
  data() {
    return {
      author: {
        name: 'John Doe',
        books: [
          'Vue 2 - Advanced Guide',
          'Vue 3 - Basic Guide',
          'Vue 4 - The Mystery'
        ]
      }
    }
  }
}
```

```ts
// 第三步
export default {
  data: () => ({
    author: {
      name: 'John Doe',
      books: [
        'Vue 2 - Advanced Guide',
        'Vue 3 - Basic Guide',
        'Vue 4 - The Mystery'
      ]
    }
  })
}
```

非代码块将被忽略。

```vue
<!-- 第四步 -->
<script setup>
const author = {
  name: 'John Doe',
  books: [
    'Vue 2 - Advanced Guide',
    'Vue 3 - Basic Guide',
    'Vue 4 - The Mystery'
  ]
}
</script>
```
````


---

# Monaco 编辑器

Slidev 提供内置的 Monaco 编辑器支持。

在代码块中添加 `{monaco}` 将其转换为编辑器：

```ts {monaco}
import { ref } from 'vue'
import { emptyArray } from './external'

const arr = ref(emptyArray(10))
```

使用 `{monaco-run}` 创建一个可以直接在幻灯片中执行代码的编辑器：

```ts {monaco-run}
import { version } from 'vue'
import { emptyArray } from './external'

console.log(`vue ${version}`)
// 斐波那契
console.log(emptyArray<number>(10).reduce(fib => [...fib, fib.at(-1)! + fib.at(-2)!], [1, 1]))
```



---
transition: slide-up
---

# 内置组件 --- Arrow

绘制一个箭头。

```md
<Arrow x1="10" y1="20" x2="100" y2="200" />
```

参数：

- `x1` (`string | number`, 必要值): 起始 x 位置
- `y1` (`string | number`, 必要值): 起始 y 位置
- `x2` (`string | number`, 必要值): 终点 x 位置
- `y2` (`string | number`, 必要值): 终点 y 位置
- `width` (`string | number`, 默认为: `2`): 线宽
- `color` (`string`, 默认为: `'currentColor'`): 颜色
- `two-way` (`boolean`, default: `false`): draw a two-way arrow


---
transition: slide-up
---

# 内置布局

```md
---
layout: xxx # 布局
---
```

- center, 在屏幕中间展示内容。
- cover, 用来展示演讲稿的封面页，可以包含演讲的标题、演讲者、时间等。
- image-left, 在屏幕左侧展示图片，屏幕右侧展示内容。
- quote, 突出显示引文。
- none, 没有任何样式的布局。
- intro, 介绍演讲稿，通​​常带有演讲稿标题、简述、作者等信息。
- two-cols, 将页面内容分为两列。
- ...

<div class="mt10" v-click>除了以上内置布局，也可以自定义布局</div>



---

# 动画

你可以在元素上添加 `v-click` 来添加点击动画。

<div v-click>

点击幻灯片时显示：

```html
<div v-click>点击幻灯片时显示。</div>
```

</div>

<br>

<v-click>

<span v-mark.red="3"><code>v-mark</code> 指令</span>
还允许你添加
<span v-mark.circle.orange="4">内联标记</span>
， 由 [Rough Notation](https://roughnotation.com/) 提供支持：

```html
<span v-mark.red="3"><code>v-mark</code> 指令</span>
<span v-mark.underline.orange>内联标记</span>
```

</v-click>

<div mt-20 v-click>

[了解更多](https://sli.dev/guide/animations#click-animation)

</div>



---
layout: default
---

# 部署

使用 GitHub Pages 部署

通过 GitHub Actions 在 GitHub Pages 上部署你的幻灯片，请按照以下步骤操作：

1. 在你的仓库中上传所有项目文件（例如命名为 repo-name）
2. 创建 .github/workflows/deploy.yml 文件，编写合适的内容，以通过 GitHub Actions 将你的幻灯片部署到 GitHub Pages
3. 在你的仓库中，转到 Settings > Pages。在 Build and deployment 下，选择 GitHub Actions
4. 最后，将更改推送到 main 分支并等待 GitHub Action 工作流完成。你应该看到站点部署到 https://username.github.io/repo-name/ 或 https://custom-domain/ ，这取决于你的设置。你的站点将在每次推送到 main 分支时自动部署。



---

<img src="/deploy-settings.png" style="height: 100%; display: block; margin: 0 auto;" />



---

```md {all}{maxHeight: '100%'}
name: Deploy My Slides

on:
  workflow_dispatch: # 允许手动触发工作流
  push:
    branches: [main] # 当推送到 main 分支时，自动触发该工作流

permissions:
  contents: read # 允许读取仓库内容
  pages: write # 允许写入 Pages
  id-token: write # 允许生成 ID 令牌

concurrency:
  group: pages # 限制并发任务数，以避免同时部署多个 Pages 任务
  cancel-in-progress: false # 不取消正在运行的任务

jobs:
  build:
    runs-on: ubuntu-latest # 运行环境

    steps:
      - uses: actions/checkout@v4 # 检出代码

      - uses: actions/setup-node@v4 # 设置 Node.js 环境
        with:
          node-version: 'lts/*' # 使用最新 LTS 版本

      - name: Setup @antfu/ni
        run: npm i -g @antfu/ni

      - name: Install dependencies
        run: nci # 安装依赖

      - name: Build
        run: nr build --base /${{github.event.repository.name}}/ # 构建

      - name: Setup Pages
        uses: actions/configure-pages@v4 # 配置 Pages

      - uses: actions/upload-pages-artifact@v3 # 上传构建产物
        with:
          path: dist # 构建产物目录

  # 这个 job 负责将 build 作业构建出的静态文件部署到 GitHub Pages
  deploy:
    environment:
      name: github-pages
      url: ${{ steps.deployment.outputs.page_url }}
    needs: build # 依赖 build job
    runs-on: ubuntu-latest
    name: Deploy
    steps:
      - name: Deploy to GitHub Pages
        id: deployment
        uses: actions/deploy-pages@v4

```



---

# LF

<div v-click>当前有两种主流换行符，分别是 LF(linux, mac)，CRLF(windows)</div>

<span v-click>对于 Windows 用户，应该使用哪一种呢？</span><span v-click style="color: red">LF</span>

<div v-click class="mt10">
原因：
</div>

<div v-click class="mt1">
1. 绝大多数项目都是强制使用 LF, 有的必须要在本地使用类似 editorconfig 的工具强制转换后才能提交
</div>

<div v-click class="mt1">
2. 讨厌的 warning
<img class="mt1" src="/git-add.png" />
</div>

<div v-click class="mt1">
4. 使用多数前端脚手架生成的代码都是 LF，原有代码是 CRLF
</div>

<div v-click class="mt1">
5. 提高跨平台兼容性
</div>

<div v-click>
  ...
</div>



---

# LF

<div class="mt8">

如何使用：

```sh
# Git 全局设置
git config --global core.autocrlf input
```

```json
// vscode settings.json
"files.eol": "\n",
```

</div>



---

# 线性提交历史

<div>
场景：同事a和同事b因某种原因共用一个开发分支 git-test-1，同事a写了一堆代码，提交了代码，同事b此时也写了一堆代码，也要提交代码。
</div>

<div v-click class="mt2"><img src="/git-commit.png" /></div>

<div v-click class="mt8">如果稍不注意，提交历史就会不那么好看了</div>

<div v-click class="mt2">

<img src="/chaotic-git-commit-history.png" />
</div>

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

<!--
这是在一个分支上的提交记录
这种历史记录包含了多个分叉点和合并提交，就会导致 git 提交历史看起来非常混乱
-->



---
layout: center
---

# git pull = git fetch + git merge

<style>
h1 {
  color: white;
}
</style>

<!--
在执行 git pull 时，其实是有一步合并操作的
-->



---

# 解决办法1（99%情况下可行）

<div v-click class="mt5">
每次 add 前先执行 pull，如果有冲突，本地解决冲突(stash 解决)，然后提交
</div>

<div v-click class="mt5">
上文说到 git pull 其实是有 merge 操作的，那这样为什么可以保证线性提交历史呢？
</div>

<div v-click class="mt5">
原因：

1. 没有冲突的情况下，默认执行了快进合并，此时不会强制创建合并提交的
2. 有冲突的情况下，打断了 merge 操作，当处理完冲突并标记冲突已解决，然后 commit，push，这个过程只有一次 commit，还是保持线性提交历史

> 如果使用 commit 解决冲突，还是保证不了线性提交历史
</div>

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

<!-- 
这种情况是大多数
-->



---


# 解决办法2（有冲突情况下）

使用 git pull --rebase

```sh {all|1|2|3|4|5|6|7|all} twoslash
git add .
git commit -m "first commit message"
git push
git pull --rebase # 此时会有冲突，解决冲突
git commit -m "second commit message"
git rebase --continue
git push
```


<div v-if="$clicks == 3" v-click="[3, 4]" class="mt3">
  <img src="/git-push-error.png" />
</div>

<div v-if="$clicks == 4" v-click="[4, 5]" class="mt3">
  <img src="/git-pull-rebase-error.png" style="height: 220px" />
</div>

<div v-if="$clicks == 6" v-click="[6, 7]" class="mt3">
  <img src="/git-rebase--continue-conflict.png" />
</div>

<div v-if="$clicks == 8" v-click="[8, 9]" class="mt3">
  <img src="/git-graph-conflict.png" style="height: 220px" />
</div>

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

# 解决办法2（无冲突情况下）

使用 git pull --rebase

```sh {all|1|2|3|4|5|all} twoslash
git add .
git commit -m "first commit message"
git push
git pull --rebase
git push
```


<div v-if="$clicks == 3" v-click="[3, 4]" class="mt3">
  <img src="/git-push-error.png" />
</div>

<div v-if="$clicks == 4" v-click="[4, 5]" class="mt3">
  <img src="/git-pull--rebase-sucess.png" style="height: 220px" />
</div>

<div v-if="$clicks == 6" v-click="[6, 7]" class="mt3">
  <img src="/git-graph-noconflict.png" style="height: 220px" />
</div>

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
layout: two-cols
---

<img v-click src="/git-conflict.png" style="height: 100%" class="mr2" />

::right::

<img v-click src="/git-noconflict.png" class="ml2" />



---
layout: intro
class: text-center pb-5
glowX: 50
glowY: 120
---

# 谢谢
