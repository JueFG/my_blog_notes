---
title: Hextra Theme
layout: hextra-home
---

<div style="display: flex; gap: 10px; justify-content: center; flex-wrap: wrap;">
{{< badge content="✨ 欢迎来到 Emily 的小宇宙" color="indigo" >}}
{{< badge content="🍜 理财、生活、学习，一锅乱炖才香" color="green" >}}
</div>

<div class="hx:mt-6 hx:mb-6">
{{< hextra/hero-headline >}}
<span class="hx:block hx:text-8xl sm:hx:text-8xl hx:font-bold">
Emily 的理财骚操作、
</span>
<div class="hx:h-6"></div>
<span class="hx:block hx:mt-4 hx:text-8xl sm:hx:text-5xl">
生活碎碎念和学习笔记
</span>
{{< /hextra/hero-headline >}}
</div>

<div class="hx:block hx:mt-3"></div>
{{< hextra/hero-subtitle >}}
  少点焦虑，多点好笑。攒钱像养猫，学习像追剧，生活像加点糖的气泡水。
{{< /hextra/hero-subtitle >}}


<div class="hx:mb-6 hx:mt-8">
{{< hextra/hero-button text="开始探索" link="docs" >}}
</div>

<div class="hx:mt-8"></div>

{{< hextra/feature-grid >}}
  {{< hextra/feature-card
    title="理财也要快乐存"
    subtitle="存钱像养猫，慢慢撸；别被 K 线吓到，小目标先把奶茶钱攒出来。"
    class="hx:aspect-auto hx:md:aspect-[1.1/1] hx:max-md:min-h-[340px]"
    image="images/hextra-doc.webp"
    imageClass="hx:top-[40%] hx:left-[24px] hx:w-[180%] hx:sm:w-[110%] hx:dark:opacity-80"
  >}}
  {{< hextra/feature-card
    title="学习不卷也进步"
    subtitle="笔记帮你记，表情包帮你记忆。Markdown 里夹着笑点和知识点。"
    class="hx:aspect-auto hx:md:aspect-[1.1/1] hx:max-lg:min-h-[340px]"
    image="images/hextra-markdown.webp"
    imageClass="hx:top-[40%] hx:left-[36px] hx:w-[180%] hx:sm:w-[110%] hx:dark:opacity-80"
  >}}
  {{< hextra/feature-card
    title="生活碎碎念"
    subtitle="踩坑、追剧、做饭、发呆都算成果。FlexSearch 负责帮你找回灵感。"
    class="hx:aspect-auto hx:md:aspect-[1.1/1] hx:max-md:min-h-[340px]"
    image="images/hextra-search.webp"
    imageClass="hx:top-[40%] hx:left-[36px] hx:w-[110%] hx:sm:w-[110%] hx:dark:opacity-80"
  >}}
  {{< hextra/feature-card
    title="轻得像气球"
    subtitle="没装 Node.js 也能飞，Hugo 一键起飞，博客比你的外卖还快到。"
  >}}
  {{< hextra/feature-card
    title="暗黑模式自动护眼"
    subtitle="白天晒太阳，晚上切暗黑，护眼不护懒，手机电脑都能好好看。"
  >}}
  {{< hextra/feature-card
    title="白嫖托管指南"
    subtitle="GitHub Actions 帮你干活，Pages 帮你省房租；想换宿主也没在怕。"
  >}}
  {{< hextra/feature-card
    title="多语言=多彩生活"
    subtitle="在文件名后面加个后缀就能多语种，像给生活加滤镜一样简单。"
  >}}
  {{< hextra/feature-card
    title="还有一堆好玩的"
    icon="sparkles"
    subtitle="代码高亮 / 目录 / RSS / LaTeX / Mermaid / 自定义… 统统安排上。"
  >}}
{{< /hextra/feature-grid >}}

<style>
  /* 1. 全局背景 */
  body {
    /* 渐变 */
    background: linear-gradient(135deg, #8ec5fc 0%, #29b9b4ff 100%);
    background-attachment: fixed;
    background-size: cover;
  }

  /* 深色模式背景 */
  .dark body {
    background: linear-gradient(135deg, #0f172a 0%, #312e81 100%);
  }
  
  /* 2. 毛玻璃核心代码 */
  /* 这里使用了 !important 强制覆盖主题默认的白色背景 */
  .hextra-feature-card {
    /* 背景色：白色，但是只有 20% 不透明度 (0.2) -> 越小越透 */
    background-color: rgba(216, 229, 251, 0.2) !important;
    
    /* 模糊滤镜：数字越大，背后的东西越模糊 */
    backdrop-filter: blur(15px);
    -webkit-backdrop-filter: blur(15px); /* 兼容 Safari */
    
    /* 玻璃边缘的高光描边（关键！） */
    border: 2px solid rgba(255, 255, 255, 0.5);
    box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1); /* 柔和阴影 */
  }

  /* 深色模式下的玻璃卡片 */
  .dark .hextra-feature-card {
    background-color: rgba(0, 0, 0, 0.2) !important; /* 黑色半透明 */
  }
</style>