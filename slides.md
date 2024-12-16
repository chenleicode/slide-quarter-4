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
title: 陈磊的 Web PPT
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
---

# 第四季度技术分享

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
layout: two-cols
hideInToc: true
---

# 目录

::right::

<Toc v-click minDepth="1" maxDepth="1" columns="1" class="toc-class" />

<style>
.toc-class {}
h1 {
  margin-top: 200px;
  margin-left: 100px;
}
</style>



---
transition: fade-out
---

# 什么是 Slidev ？

Slidev 是一个为开发者设计的幻灯片制作和演示工具，具有以下特点：

- 📝 [**Markdown 支持**](https://cn.sli.dev/guide/syntax.html) —— 使用你最喜欢的编辑器和工作流编写 Markdown 文件
- 🧑‍💻 [**对开发者友好**](https://cn.sli.dev/guide/syntax.html#code-blocks) —— 内置代码高亮、实时编码等功能
- 🌈 [**灵活样式**](https://cn.sli.dev/guide/syntax.html#embedded-styles) —— 使用 [Windi CSS](https://windicss.org/) 按需使用的实用类和易用的内嵌样式表
- 🤹 [**交互**](https://cn.sli.dev/custom/directory-structure.html#components) —— 无缝嵌入 Vue 组件
- 🎙 [**演示者模式**](https://cn.sli.dev/guide/presenter-mode.html) —— 可以使用另一个窗口，甚至是你的手机来控制幻灯片
- 📰 [**图表支持**](https://cn.sli.dev/guide/syntax.html#diagrams) —— 使用文本描述语言创建图表
- 🌟 [**图标**](https://cn.sli.dev/guide/syntax.html#icons) —— 能够直接从任意图标库中获取图标
- 🎥 [**录制**](https://cn.sli.dev/guide/recording.html) —— 内置录制功能和摄像头视图
- 📤 [**跨平台**](https://cn.sli.dev/guide/exporting.html) —— 能够导出 PDF、PNG 文件，甚至是一个可以托管的单页应用
- ⚡️ [**快速**](https://vitejs.dev) —— 基于 [Vite](https://vitejs.dev) 的即时重载
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



---
transition: fade-out
---

# 快速上手

<div v-click>在终端运行以下命令来创建一个新的 Slidev 项目：</div>

<div v-click>

```sh
npm init slidev@latest # npm

pnpm create slidev # pnpm

yarn create slidev # yarn
```

</div>

<div v-click class="mt5">根据指引，输入项目名称，并按照提示完成项目创建</div>

<div v-click class="mt5">幻灯片内容在 slides.md 文件中，初始内容包含了 Slidev 的大部分功能的演示</div>



---

<img src="/quick-start.png" style="height: 100%; display: block; margin: 0 auto;" />


---
transition: fade-out
---

# 语法 --- Frontmatter 和 Headmatter

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

# 语法 --- 备注

每张幻灯片的末尾的注释块（若有），将被视为幻灯片的备注。它们将在用户界面中显示，以供您在演示过程中参考

```md
---
layout: cover
---

# 第一页

封面页

<!-- 这是一段备注 -->

```



---
transition: slide-up
---

# 语法 --- 代码块

```ts {all|1|3-4|6|all} twoslash
import { computed, ref } from 'vue'

const count = ref(0)
const doubled = computed(() => count.value * 2)

doubled.value = 2

// 无论代码块的第一行代码代码是什么位置，行号都是从1开始
// 显示步骤：1全部代码高亮 2第一行代码高亮 3第三至第四行代码高亮 4第六行代码高亮 5全部代码高亮
```

<arrow v-click="[3, 4]" x1="350" y1="190" x2="155" y2="235" color="#953" width="2" arrowSize="1" />

[了解更多](https://cn.sli.dev/guide/syntax#code-block)



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
transition: slide-up
level: 2
---

# 导航

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
layout: default
---

# 部署

使用 GitHub + GitHub Pages 部署

通过 GitHub Actions 在 GitHub Pages 上部署你的幻灯片，请按照以下步骤操作：

1. 在你的仓库中上传所有项目文件（例如命名为 repo-name）
2. 创建 .github/workflows/deploy.yml 文件，编写合适的内容，以通过 GitHub Actions 将你的幻灯片部署到 GitHub Pages
3. 在你的仓库中，转到 Settings > Pages。在 Build and deployment 下，选择 GitHub Actions
4. 最后，将更改推送到 main 分支并等待 GitHub Action 工作流完成。你应该看到站点部署到 https://username.github.io/repo-name/ 或 https://custom-domain/，这取决于你的设置。你的站点将在每次推送到 main 分支时自动部署。



---


<img src="/deploy-settings.png" style="height: 100%; display: block; margin: 0 auto;" />



---

```md {all}{maxHeight: '100%'}
name: Deploy My Slide

on:
  workflow_dispatch:
  push:
    branches: [main]

permissions:
  contents: read
  pages: write
  id-token: write

concurrency:
  group: pages
  cancel-in-progress: false

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - uses: actions/checkout@v4

      - uses: actions/setup-node@v4
        with:
          node-version: 'lts/*'

      - name: Setup @antfu/ni
        run: npm i -g @antfu/ni

      - name: Install dependencies
        run: nci

      - name: Build
        run: nr build --base /${{github.event.repository.name}}/

      - name: Setup Pages
        uses: actions/configure-pages@v4

      - uses: actions/upload-pages-artifact@v3
        with:
          path: dist

  deploy:
    environment:
      name: github-pages
      url: ${{ steps.deployment.outputs.page_url }}
    needs: build
    runs-on: ubuntu-latest
    name: Deploy
    steps:
      - name: Deploy to GitHub Pages
        id: deployment
        uses: actions/deploy-pages@v4

```



---

# Clicks Animations

You can add `v-click` to elements to add a click animation.

<div v-click>

This shows up when you click the slide:

```html
<div v-click>This shows up when you click the slide.</div>
```

</div>

<br>

<v-click>

The <span v-mark.red="3"><code>v-mark</code> directive</span>
also allows you to add
<span v-mark.circle.orange="4">inline marks</span>
, powered by [Rough Notation](https://roughnotation.com/):

```html
<span v-mark.underline.orange>inline markers</span>
```

</v-click>

<div mt-20 v-click>

[Learn more](https://sli.dev/guide/animations#click-animation)

</div>



---

# LF

<div v-click>当前有两种主流换行符，分别是 LF(linux, mac)，CRLF(windows)</div>

<span v-click>对于 Windows 用户，应该使用哪一种呢？</span><span v-click style="color: red">LF</span>

<div v-click class="mt5">
原因：

- 绝大多数项目都是强制使用 LF, 有的必须要在本地使用类似 editorconfig 的工具强制转换后才能提交
- 讨厌的 warning
<img src="/git-add.png" />
- 使用多数前端脚手架生成的代码都是 LF，原有代码是 CRLF
- 提高跨平台兼容性
- ...

</div>



---

# LF

<div class="mt8">

如何使用：

```sh
# git 全局设置
git config --global core.autocrlf input
```

```json
// vscode settings.json
"files.eol": "\n",
```

</div>



---

<div v-click>场景：同事a和同事b因某种原因共用一个开发分支 git-test-1，同事a写了一堆代码，提交了代码，同事b此时也写了一堆代码，也要提交代码。</div>

<div v-click><img src="/git-commit.png" /></div>

<div v-click class="mt8">如果稍不注意，提交历史就会不那么好看了</div>

<div v-click class="mt2">
这种历史记录包含了多个分叉点和合并提交，就会导致 git 提交历史看起来非常混乱

<img src="/chaotic-git-commit-history.png" />
</div>



---
layout: center
---

git pull = git fetch + git merge

在执行 git pull 时，其实是有一步合并操作的



---

# 解决办法1

<div v-click>
每次 add 前先执行 pull，如果有冲突，本地解决冲突(stash 解决)，然后提交

上文说到 git pull 其实是有 merge 操作的，那这样为什么可以保证线性提交历史呢？原因：

1. 没有冲突的情况下是会默认执行了快进合并，此时不会强制创建合并提交历史的
2. 即使有冲突，此时还没有 commit 操作，解决冲突后，执行 add 和 commit 操作，还是会只有一次提交记录(如果使用commit解决冲突，还是保证不了线性提交历史)
</div>



---

# 解决办法2(终极解决办法)

使用 git pull --rebase

```sh {all|1-2|3|4|5-9|all} twoslash
git add .
git commit -m "新增一行打印（1）"
git push
# error
git pull --rebase
# 处理冲突
git commit -m "新增一行打印（2）"
git rebase --continue
git push
```


---

<img src="/git-pull--rebase.png" style="height: 100%; display: block; margin: 0 auto;" />



---
layout: center
class: text-center
---

# 谢谢！
