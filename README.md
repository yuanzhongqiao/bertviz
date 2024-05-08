<div class="Box-sc-g0xbh4-0 bJMeLZ js-snippet-clipboard-copy-unpositioned" data-hpc="true"><article class="markdown-body entry-content container-lg" itemprop="text"><div class="markdown-heading" dir="auto"><h1 align="center" tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">
    伯特维兹
</font></font></h1><a id="user-content-----bertviz" class="anchor" aria-label="永久链接：BertViz
" href="#----bertviz"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-heading" dir="auto"><h3 align="center" tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">
 可视化 NLP 模型中的注意力
</font></font></h3><a id="user-content--visualize-attention-in-nlp-models" class="anchor" aria-label="永久链接：可视化 NLP 模型中的注意力
" href="#-visualize-attention-in-nlp-models"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-heading" dir="auto"><h3 align="center" tabindex="-1" class="heading-element" dir="auto">
    <a href="#-quick-tour"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">快速浏览</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">•
    </font></font><a href="#%EF%B8%8F-getting-started"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">入门</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">•
     </font></font><a href="https://colab.research.google.com/drive/1hXIQ77A4TYS4y3UthWF-Ci7V7vVUoxmQ?usp=sharing" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Colab 教程</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">•
    </font></font><a href="#-paper"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">论文</font></font></a>
</h3><a id="user-content-----quick-tour-----getting-started-----colab-tutorial-----paper" class="anchor" aria-label="永久链接：快速浏览 • 入门 • Colab 教程 • 论文" href="#----quick-tour-----getting-started-----colab-tutorial-----paper"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">BertViz 是一种交互式工具，用于可视化</font></font><a href="https://jalammar.github.io/illustrated-transformer/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Transformer</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">语言模型（例如 BERT、GPT2 或 T5）中的注意力。它可以通过支持大多数</font></font><a href="https://huggingface.co/models" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Huggingface 模型</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">的简单 Python API 在 Jupyter 或 Colab 笔记本中运行</font><font style="vertical-align: inherit;">。 BertViz 扩展了
</font><a href="https://medium.com/@llionj" rel="nofollow"><font style="vertical-align: inherit;">Llion Jones</font></a><font style="vertical-align: inherit;">
的</font></font><a href="https://github.com/tensorflow/tensor2tensor/tree/master/tensor2tensor/visualization"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Tensor2Tensor 可视化工具</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，提供了多个视图，每个视图都为注意力机制提供了独特的视角。</font></font><a href="https://medium.com/@llionj" rel="nofollow"><font style="vertical-align: inherit;"></font></a><font style="vertical-align: inherit;"></font></p>
<p dir="auto"><font style="vertical-align: inherit;"></font><a href="https://twitter.com/jesse_vig" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在Twitter
</font></font><img src="/jessevig/bertviz/raw/master/images/twitter.svg" alt="推特标志" style="max-width: 100%;"></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">上获取此项目及相关项目的更新</font><font style="vertical-align: inherit;">。</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">🚀 快速浏览</font></font></h2><a id="user-content--quick-tour" class="anchor" aria-label="永久链接：🚀 快速浏览" href="#-quick-tour"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">头部视图</font></font></h3><a id="user-content-head-view" class="anchor" aria-label="永久链接：头部视图" href="#head-view"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">头部</font></font><em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">视图</font></font></em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">可视化同一层中一个或多个注意力头的注意力。它基于</font><a href="https://medium.com/@llionj" rel="nofollow"><font style="vertical-align: inherit;">Llion Jones</font></a><font style="vertical-align: inherit;">出色的</font></font><a href="https://github.com/tensorflow/tensor2tensor/tree/master/tensor2tensor/visualization"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Tensor2Tensor 可视化工具</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font><a href="https://medium.com/@llionj" rel="nofollow"><font style="vertical-align: inherit;"></font></a><font style="vertical-align: inherit;"></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">🕹 尝试</font></font><a href="https://colab.research.google.com/drive/1hXIQ77A4TYS4y3UthWF-Ci7V7vVUoxmQ?usp=sharing" rel="nofollow"><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">交互式 Colab 教程</font></font></b></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">中的头部视图（所有可视化效果均已预加载）。</font></font></p>
<p dir="auto">
    <animated-image data-catalyst="" style="width: 425px;"><a target="_blank" rel="noopener noreferrer nofollow" href="https://raw.githubusercontent.com/jessevig/bertviz/master/images/head-view.gif" data-target="animated-image.originalLink"><img src="https://raw.githubusercontent.com/jessevig/bertviz/master/images/head-view.gif" style="max-width: 100%; display: inline-block;" data-target="animated-image.originalImage"></a>
      <span class="AnimatedImagePlayer" data-target="animated-image.player" hidden="">
        <a data-target="animated-image.replacedLink" class="AnimatedImagePlayer-images" href="https://raw.githubusercontent.com/jessevig/bertviz/master/images/head-view.gif" target="_blank">
          
        <span data-target="animated-image.imageContainer">
            <img data-target="animated-image.replacedImage" alt="head-view.gif" class="AnimatedImagePlayer-animatedImage" src="https://raw.githubusercontent.com/jessevig/bertviz/master/images/head-view.gif" style="display: block; opacity: 1;">
          <canvas class="AnimatedImagePlayer-stillImage" aria-hidden="true" width="425" height="374"></canvas></span></a>
        <button data-target="animated-image.imageButton" class="AnimatedImagePlayer-images" tabindex="-1" aria-label="Play head-view.gif" hidden=""></button>
        <span class="AnimatedImagePlayer-controls" data-target="animated-image.controls" hidden="">
          <button data-target="animated-image.playButton" class="AnimatedImagePlayer-button" aria-label="Play head-view.gif">
            <svg aria-hidden="true" focusable="false" class="octicon icon-play" width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M4 13.5427V2.45734C4 1.82607 4.69692 1.4435 5.2295 1.78241L13.9394 7.32507C14.4334 7.63943 14.4334 8.36057 13.9394 8.67493L5.2295 14.2176C4.69692 14.5565 4 14.1739 4 13.5427Z">
            </path></svg>
            <svg aria-hidden="true" focusable="false" class="octicon icon-pause" width="16" height="16" viewBox="0 0 16 16" xmlns="http://www.w3.org/2000/svg">
              <rect x="4" y="2" width="3" height="12" rx="1"></rect>
              <rect x="9" y="2" width="3" height="12" rx="1"></rect>
            </svg>
          </button>
          <a data-target="animated-image.openButton" aria-label="Open head-view.gif in new window" class="AnimatedImagePlayer-button" href="https://raw.githubusercontent.com/jessevig/bertviz/master/images/head-view.gif" target="_blank">
            <svg aria-hidden="true" class="octicon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" width="16" height="16">
              <path fill-rule="evenodd" d="M10.604 1h4.146a.25.25 0 01.25.25v4.146a.25.25 0 01-.427.177L13.03 4.03 9.28 7.78a.75.75 0 01-1.06-1.06l3.75-3.75-1.543-1.543A.25.25 0 0110.604 1zM3.75 2A1.75 1.75 0 002 3.75v8.5c0 .966.784 1.75 1.75 1.75h8.5A1.75 1.75 0 0014 12.25v-3.5a.75.75 0 00-1.5 0v3.5a.25.25 0 01-.25.25h-8.5a.25.25 0 01-.25-.25v-8.5a.25.25 0 01.25-.25h3.5a.75.75 0 000-1.5h-3.5z"></path>
            </svg>
          </a>
        </span>
      </span></animated-image>
</p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">模型视图</font></font></h3><a id="user-content-model-view" class="anchor" aria-label="永久链接：模型视图" href="#model-view"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">模型</font></font><em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">视图</font></font></em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">显示了所有层和头的注意力的鸟瞰图。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">🕹 尝试</font></font><a href="https://colab.research.google.com/drive/1hXIQ77A4TYS4y3UthWF-Ci7V7vVUoxmQ?usp=sharing" rel="nofollow"><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">交互式 Colab 教程</font></font></b></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">中的模型视图（所有可视化均已预加载）。</font></font></p>
<p dir="auto"><animated-image data-catalyst=""><a target="_blank" rel="noopener noreferrer" href="/jessevig/bertviz/blob/master/images/model-view-noscroll.gif" data-target="animated-image.originalLink"><img src="/jessevig/bertviz/raw/master/images/model-view-noscroll.gif" alt="模型视图" style="max-width: 100%; display: inline-block;" data-target="animated-image.originalImage"></a>
      <span class="AnimatedImagePlayer" data-target="animated-image.player" hidden="">
        <a data-target="animated-image.replacedLink" class="AnimatedImagePlayer-images" href="https://github.com/jessevig/bertviz/blob/master/images/model-view-noscroll.gif" target="_blank">
          
        <span data-target="animated-image.imageContainer">
            <img data-target="animated-image.replacedImage" alt="model view" class="AnimatedImagePlayer-animatedImage" src="https://github.com/jessevig/bertviz/raw/master/images/model-view-noscroll.gif" style="display: block; opacity: 1;">
          <canvas class="AnimatedImagePlayer-stillImage" aria-hidden="true" width="814" height="757"></canvas></span></a>
        <button data-target="animated-image.imageButton" class="AnimatedImagePlayer-images" tabindex="-1" aria-label="Play model view" hidden=""></button>
        <span class="AnimatedImagePlayer-controls" data-target="animated-image.controls" hidden="">
          <button data-target="animated-image.playButton" class="AnimatedImagePlayer-button" aria-label="Play model view">
            <svg aria-hidden="true" focusable="false" class="octicon icon-play" width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M4 13.5427V2.45734C4 1.82607 4.69692 1.4435 5.2295 1.78241L13.9394 7.32507C14.4334 7.63943 14.4334 8.36057 13.9394 8.67493L5.2295 14.2176C4.69692 14.5565 4 14.1739 4 13.5427Z">
            </path></svg>
            <svg aria-hidden="true" focusable="false" class="octicon icon-pause" width="16" height="16" viewBox="0 0 16 16" xmlns="http://www.w3.org/2000/svg">
              <rect x="4" y="2" width="3" height="12" rx="1"></rect>
              <rect x="9" y="2" width="3" height="12" rx="1"></rect>
            </svg>
          </button>
          <a data-target="animated-image.openButton" aria-label="Open model view in new window" class="AnimatedImagePlayer-button" href="https://github.com/jessevig/bertviz/blob/master/images/model-view-noscroll.gif" target="_blank">
            <svg aria-hidden="true" class="octicon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" width="16" height="16">
              <path fill-rule="evenodd" d="M10.604 1h4.146a.25.25 0 01.25.25v4.146a.25.25 0 01-.427.177L13.03 4.03 9.28 7.78a.75.75 0 01-1.06-1.06l3.75-3.75-1.543-1.543A.25.25 0 0110.604 1zM3.75 2A1.75 1.75 0 002 3.75v8.5c0 .966.784 1.75 1.75 1.75h8.5A1.75 1.75 0 0014 12.25v-3.5a.75.75 0 00-1.5 0v3.5a.25.25 0 01-.25.25h-8.5a.25.25 0 01-.25-.25v-8.5a.25.25 0 01.25-.25h3.5a.75.75 0 000-1.5h-3.5z"></path>
            </svg>
          </a>
        </span>
      </span></animated-image></p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">神经元视图</font></font></h3><a id="user-content-neuron-view" class="anchor" aria-label="永久链接：神经元视图" href="#neuron-view"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"></font><em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">神经元视图</font></font></em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">可视</font><font style="vertical-align: inherit;">化查询和关键向量中的各个神经元，并显示它们如何用于计算注意力。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">🕹 尝试</font></font><a href="https://colab.research.google.com/drive/1hXIQ77A4TYS4y3UthWF-Ci7V7vVUoxmQ?usp=sharing" rel="nofollow"><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">交互式 Colab 教程</font></font></b></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">中的神经元视图（所有可视化均已预加载）。</font></font></p>
<p dir="auto"><animated-image data-catalyst=""><a target="_blank" rel="noopener noreferrer" href="/jessevig/bertviz/blob/master/images/neuron-view-dark.gif" data-target="animated-image.originalLink"><img src="/jessevig/bertviz/raw/master/images/neuron-view-dark.gif" alt="神经元视图" style="max-width: 100%; display: inline-block;" data-target="animated-image.originalImage"></a>
      <span class="AnimatedImagePlayer" data-target="animated-image.player" hidden="">
        <a data-target="animated-image.replacedLink" class="AnimatedImagePlayer-images" href="https://github.com/jessevig/bertviz/blob/master/images/neuron-view-dark.gif" target="_blank">
          
        <span data-target="animated-image.imageContainer">
            <img data-target="animated-image.replacedImage" alt="neuron view" class="AnimatedImagePlayer-animatedImage" src="https://github.com/jessevig/bertviz/raw/master/images/neuron-view-dark.gif" style="display: block; opacity: 1;">
          <canvas class="AnimatedImagePlayer-stillImage" aria-hidden="true" width="814" height="403"></canvas></span></a>
        <button data-target="animated-image.imageButton" class="AnimatedImagePlayer-images" tabindex="-1" aria-label="Play neuron view" hidden=""></button>
        <span class="AnimatedImagePlayer-controls" data-target="animated-image.controls" hidden="">
          <button data-target="animated-image.playButton" class="AnimatedImagePlayer-button" aria-label="Play neuron view">
            <svg aria-hidden="true" focusable="false" class="octicon icon-play" width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M4 13.5427V2.45734C4 1.82607 4.69692 1.4435 5.2295 1.78241L13.9394 7.32507C14.4334 7.63943 14.4334 8.36057 13.9394 8.67493L5.2295 14.2176C4.69692 14.5565 4 14.1739 4 13.5427Z">
            </path></svg>
            <svg aria-hidden="true" focusable="false" class="octicon icon-pause" width="16" height="16" viewBox="0 0 16 16" xmlns="http://www.w3.org/2000/svg">
              <rect x="4" y="2" width="3" height="12" rx="1"></rect>
              <rect x="9" y="2" width="3" height="12" rx="1"></rect>
            </svg>
          </button>
          <a data-target="animated-image.openButton" aria-label="在新窗口中打开神经元视图" class="AnimatedImagePlayer-button" href="https://github.com/jessevig/bertviz/blob/master/images/neuron-view-dark.gif" target="_blank">
            <svg aria-hidden="true" class="octicon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" width="16" height="16">
              <path fill-rule="evenodd" d="M10.604 1h4.146a.25.25 0 01.25.25v4.146a.25.25 0 01-.427.177L13.03 4.03 9.28 7.78a.75.75 0 01-1.06-1.06l3.75-3.75-1.543-1.543A.25.25 0 0110.604 1zM3.75 2A1.75 1.75 0 002 3.75v8.5c0 .966.784 1.75 1.75 1.75h8.5A1.75 1.75 0 0014 12.25v-3.5a.75.75 0 00-1.5 0v3.5a.25.25 0 01-.25.25h-8.5a.25.25 0 01-.25-.25v-8.5a.25.25 0 01.25-.25h3.5a.75.75 0 000-1.5h-3.5z"></path>
            </svg>
          </a>
        </span>
      </span></animated-image></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">⚡️ 开始使用</font></font></h2><a id="user-content-️-getting-started" class="anchor" aria-label="永久链接：⚡️ 入门" href="#️-getting-started"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在 Jupyter Notebook 中运行 BertViz</font></font></h3><a id="user-content-running-bertviz-in-a-jupyter-notebook" class="anchor" aria-label="永久链接：在 Jupyter Notebook 中运行 BertViz" href="#running-bertviz-in-a-jupyter-notebook"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">从命令行：</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>pip install bertviz</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="pip install bertviz" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">您还必须安装 Jupyter Notebook 和 ipywidgets：</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>pip install jupyterlab
pip install ipywidgets</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="pip install jupyterlab
pip install ipywidgets" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（如果您在安装 Jupyter 或 ipywidgets 时遇到任何问题，请参阅</font></font><a href="https://jupyter.org/install" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">此处</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">和</font></font><a href="https://ipywidgets.readthedocs.io/en/stable/user_install.html" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">此处的</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">文档。）</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">要创建新的 Jupyter 笔记本，只需运行：</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>jupyter notebook</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="jupyter notebook" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">然后如果出现提示，请单击</font></font><code>New</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">并选择</font></font><code>Python 3 (ipykernel)</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto">Running BertViz in Colab</h3><a id="user-content-running-bertviz-in-colab" class="anchor" aria-label="永久链接：在 Colab 中运行 BertViz" href="#running-bertviz-in-colab"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">To run in <a href="https://colab.research.google.com/" rel="nofollow">Colab</a>, simply add the following cell at the beginning of your Colab notebook:</p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>!pip install bertviz
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="!pip install bertviz" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto">Sample code</h3><a id="user-content-sample-code" class="anchor" aria-label="永久链接：示例代码" href="#sample-code"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">Run the following code to load the <code>xtremedistil-l12-h384-uncased</code> model and display it in the model view:</p>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-k">from</span> <span class="pl-s1">transformers</span> <span class="pl-k">import</span> <span class="pl-v">AutoTokenizer</span>, <span class="pl-v">AutoModel</span>, <span class="pl-s1">utils</span>
<span class="pl-k">from</span> <span class="pl-s1">bertviz</span> <span class="pl-k">import</span> <span class="pl-s1">model_view</span>
<span class="pl-s1">utils</span>.<span class="pl-s1">logging</span>.<span class="pl-en">set_verbosity_error</span>()  <span class="pl-c"># Suppress standard warnings</span>

<span class="pl-s1">model_name</span> <span class="pl-c1">=</span> <span class="pl-s">"microsoft/xtremedistil-l12-h384-uncased"</span>  <span class="pl-c"># Find popular HuggingFace models here: https://huggingface.co/models</span>
<span class="pl-s1">input_text</span> <span class="pl-c1">=</span> <span class="pl-s">"The cat sat on the mat"</span>  
<span class="pl-s1">model</span> <span class="pl-c1">=</span> <span class="pl-v">AutoModel</span>.<span class="pl-en">from_pretrained</span>(<span class="pl-s1">model_name</span>, <span class="pl-s1">output_attentions</span><span class="pl-c1">=</span><span class="pl-c1">True</span>)  <span class="pl-c"># Configure model to return attention values</span>
<span class="pl-s1">tokenizer</span> <span class="pl-c1">=</span> <span class="pl-v">AutoTokenizer</span>.<span class="pl-en">from_pretrained</span>(<span class="pl-s1">model_name</span>)
<span class="pl-s1">inputs</span> <span class="pl-c1">=</span> <span class="pl-s1">tokenizer</span>.<span class="pl-en">encode</span>(<span class="pl-s1">input_text</span>, <span class="pl-s1">return_tensors</span><span class="pl-c1">=</span><span class="pl-s">'pt'</span>)  <span class="pl-c"># Tokenize input text</span>
<span class="pl-s1">outputs</span> <span class="pl-c1">=</span> <span class="pl-en">model</span>(<span class="pl-s1">inputs</span>)  <span class="pl-c"># Run model</span>
<span class="pl-s1">attention</span> <span class="pl-c1">=</span> <span class="pl-s1">outputs</span>[<span class="pl-c1">-</span><span class="pl-c1">1</span>]  <span class="pl-c"># Retrieve attention from model outputs</span>
<span class="pl-s1">tokens</span> <span class="pl-c1">=</span> <span class="pl-s1">tokenizer</span>.<span class="pl-en">convert_ids_to_tokens</span>(<span class="pl-s1">inputs</span>[<span class="pl-c1">0</span>])  <span class="pl-c"># Convert input ids to token strings</span>
<span class="pl-en">model_view</span>(<span class="pl-s1">attention</span>, <span class="pl-s1">tokens</span>)  <span class="pl-c"># Display model view</span></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="from transformers import AutoTokenizer, AutoModel, utils
from bertviz import model_view
utils.logging.set_verbosity_error()  # Suppress standard warnings

model_name = &quot;microsoft/xtremedistil-l12-h384-uncased&quot;  # Find popular HuggingFace models here: https://huggingface.co/models
input_text = &quot;The cat sat on the mat&quot;  
model = AutoModel.from_pretrained(model_name, output_attentions=True)  # Configure model to return attention values
tokenizer = AutoTokenizer.from_pretrained(model_name)
inputs = tokenizer.encode(input_text, return_tensors='pt')  # Tokenize input text
outputs = model(inputs)  # Run model
attention = outputs[-1]  # Retrieve attention from model outputs
tokens = tokenizer.convert_ids_to_tokens(inputs[0])  # Convert input ids to token strings
model_view(attention, tokens)  # Display model view" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto">The visualization may take a few seconds to load. Feel free to experiment with different input texts and
<a href="https://huggingface.co/models" rel="nofollow">models</a>.
See <a href="#-documentation">Documentation</a> for additional use cases and examples, e.g., encoder-decoder models.</p>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto">Running sample notebooks</h4><a id="user-content-running-sample-notebooks" class="anchor" aria-label="永久链接：运行示例笔记本" href="#running-sample-notebooks"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">You may also run any of the sample <a href="/jessevig/bertviz/blob/master/notebooks">notebooks</a> included with BertViz:</p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>git clone --depth 1 git@github.com:jessevig/bertviz.git
<span class="pl-c1">cd</span> bertviz/notebooks
jupyter notebook</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="git clone --depth 1 git@github.com:jessevig/bertviz.git
cd bertviz/notebooks
jupyter notebook" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto">🕹 Interactive Tutorial</h2><a id="user-content--interactive-tutorial" class="anchor" aria-label="永久链接：🕹互动教程" href="#-interactive-tutorial"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">Check out the <a href="https://colab.research.google.com/drive/1hXIQ77A4TYS4y3UthWF-Ci7V7vVUoxmQ?usp=sharing" rel="nofollow"><b>Interactive Colab Tutorial</b></a>
to learn more about BertViz and try out the tool. <b>Note</b>: all visualizations are pre-loaded, so there is no need to execute any cells.</p>
<p dir="auto"><a href="https://colab.research.google.com/drive/1hXIQ77A4TYS4y3UthWF-Ci7V7vVUoxmQ?usp=sharing" rel="nofollow"><img src="/jessevig/bertviz/raw/master/images/tutorial-screenshots.jpg" alt="教程" style="max-width: 100%;"></a></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto">📖 Documentation</h2><a id="user-content--documentation" class="anchor" aria-label="永久链接：📖 文档" href="#-documentation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto">Table of contents</h3><a id="user-content-table-of-contents" class="anchor" aria-label="永久链接：目录" href="#table-of-contents"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="auto">
<li><a href="#self-attention-models-bert-gpt-2-etc">Self-attention models (BERT, GPT-2, etc.)</a>
<ul dir="auto">
<li><a href="#head-and-model-views">Head and Model Views</a></li>
<li><a href="#neuron-view-1">Neuron View</a></li>
</ul>
</li>
<li><a href="#encoder-decoder-models-bart-t5-etc">Encoder-decoder models (BART, T5, etc.)</a></li>
<li><a href="#installing-from-source">Installing from source</a></li>
<li><a href="#additional-options">Additional options</a>
<ul dir="auto">
<li><a href="#dark--light-mode">Dark / light mode</a></li>
<li><a href="#filtering-layers">Filtering layers</a></li>
<li><a href="#setting-default-layerheads">Setting default layer/head(s)</a></li>
<li><a href="#visualizing-sentence-pairs">Visualizing sentence pairs</a></li>
<li><a href="#obtain-HTML-representations">Obtain HTML representations</a></li>
<li><a href="#non-huggingface-models">Non-Huggingface models</a></li>
</ul>
</li>
<li><a href="#%EF%B8%8F-limitations">Limitations</a></li>
</ul>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto">Self-attention models (BERT, GPT-2, etc.)</h3><a id="user-content-self-attention-models-bert-gpt-2-etc" class="anchor" aria-label="永久链接：自注意力模型（BERT、GPT-2 等）" href="#self-attention-models-bert-gpt-2-etc"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto">Head and Model Views</h4><a id="user-content-head-and-model-views" class="anchor" aria-label="永久链接：头部和模型视图" href="#head-and-model-views"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">First load a Huggingface model, either a pre-trained model as shown below, or your own fine-tuned model.
Be sure to set <code>output_attentions=True</code>.</p>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-k">from</span> <span class="pl-s1">transformers</span> <span class="pl-k">import</span> <span class="pl-v">AutoTokenizer</span>, <span class="pl-v">AutoModel</span>, <span class="pl-s1">utils</span>
<span class="pl-s1">utils</span>.<span class="pl-s1">logging</span>.<span class="pl-en">set_verbosity_error</span>()  <span class="pl-c"># Suppress standard warnings</span>
<span class="pl-s1">tokenizer</span> <span class="pl-c1">=</span> <span class="pl-v">AutoTokenizer</span>.<span class="pl-en">from_pretrained</span>(<span class="pl-s">"bert-base-uncased"</span>)
<span class="pl-s1">model</span> <span class="pl-c1">=</span> <span class="pl-v">AutoModel</span>.<span class="pl-en">from_pretrained</span>(<span class="pl-s">"bert-base-uncased"</span>, <span class="pl-s1">output_attentions</span><span class="pl-c1">=</span><span class="pl-c1">True</span>)</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="from transformers import AutoTokenizer, AutoModel, utils
utils.logging.set_verbosity_error()  # Suppress standard warnings
tokenizer = AutoTokenizer.from_pretrained(&quot;bert-base-uncased&quot;)
model = AutoModel.from_pretrained(&quot;bert-base-uncased&quot;, output_attentions=True)" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto">Then prepare inputs and compute attention:</p>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-s1">inputs</span> <span class="pl-c1">=</span> <span class="pl-s1">tokenizer</span>.<span class="pl-en">encode</span>(<span class="pl-s">"The cat sat on the mat"</span>, <span class="pl-s1">return_tensors</span><span class="pl-c1">=</span><span class="pl-s">'pt'</span>)
<span class="pl-s1">outputs</span> <span class="pl-c1">=</span> <span class="pl-en">model</span>(<span class="pl-s1">inputs</span>)
<span class="pl-s1">attention</span> <span class="pl-c1">=</span> <span class="pl-s1">outputs</span>[<span class="pl-c1">-</span><span class="pl-c1">1</span>]  <span class="pl-c"># Output includes attention weights when output_attentions=True</span>
<span class="pl-s1">tokens</span> <span class="pl-c1">=</span> <span class="pl-s1">tokenizer</span>.<span class="pl-en">convert_ids_to_tokens</span>(<span class="pl-s1">inputs</span>[<span class="pl-c1">0</span>]) </pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="inputs = tokenizer.encode(&quot;The cat sat on the mat&quot;, return_tensors='pt')
outputs = model(inputs)
attention = outputs[-1]  # Output includes attention weights when output_attentions=True
tokens = tokenizer.convert_ids_to_tokens(inputs[0]) " tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto">Finally, display the attention weights using the <a href="/jessevig/bertviz/blob/master/bertviz/head_view.py"><code>head_view</code></a> or <a href="/jessevig/bertviz/blob/master/bertviz/model_view.py"><code>model_view</code></a>
functions:</p>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-k">from</span> <span class="pl-s1">bertviz</span> <span class="pl-k">import</span> <span class="pl-s1">head_view</span>
<span class="pl-en">head_view</span>(<span class="pl-s1">attention</span>, <span class="pl-s1">tokens</span>)</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="from bertviz import head_view
head_view(attention, tokens)" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><b>Examples</b>: DistilBERT (<a href="/jessevig/bertviz/blob/master/notebooks/model_view_distilbert.ipynb">Model View Notebook</a>, <a href="/jessevig/bertviz/blob/master/notebooks/head_view_distilbert.ipynb">Head View Notebook</a>)</p>
<p dir="auto">For full API, please refer to the source code for the <a href="/jessevig/bertviz/blob/master/bertviz/head_view.py">head view</a> or <a href="/jessevig/bertviz/blob/master/bertviz/model_view.py">model view</a>.</p>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto">Neuron View</h4><a id="user-content-neuron-view-1" class="anchor" aria-label="永久链接：神经元视图" href="#neuron-view-1"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">The neuron view is invoked differently than the head view or model view, due to requiring access to the model's
query/key vectors, which are not returned through the Huggingface API. It is currently limited to custom versions of BERT, GPT-2, and
RoBERTa included with BertViz.</p>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c"># Import specialized versions of models (that return query/key vectors)</span>
<span class="pl-k">from</span> <span class="pl-s1">bertviz</span>.<span class="pl-s1">transformers_neuron_view</span> <span class="pl-k">import</span> <span class="pl-v">BertModel</span>, <span class="pl-v">BertTokenizer</span>
<span class="pl-k">from</span> <span class="pl-s1">bertviz</span>.<span class="pl-s1">neuron_view</span> <span class="pl-k">import</span> <span class="pl-s1">show</span>

<span class="pl-s1">model_type</span> <span class="pl-c1">=</span> <span class="pl-s">'bert'</span>
<span class="pl-s1">model_version</span> <span class="pl-c1">=</span> <span class="pl-s">'bert-base-uncased'</span>
<span class="pl-s1">do_lower_case</span> <span class="pl-c1">=</span> <span class="pl-c1">True</span>
<span class="pl-s1">sentence_a</span> <span class="pl-c1">=</span> <span class="pl-s">"The cat sat on the mat"</span>
<span class="pl-s1">sentence_b</span> <span class="pl-c1">=</span> <span class="pl-s">"The cat lay on the rug"</span>
<span class="pl-s1">model</span> <span class="pl-c1">=</span> <span class="pl-v">BertModel</span>.<span class="pl-en">from_pretrained</span>(<span class="pl-s1">model_version</span>, <span class="pl-s1">output_attentions</span><span class="pl-c1">=</span><span class="pl-c1">True</span>)
<span class="pl-s1">tokenizer</span> <span class="pl-c1">=</span> <span class="pl-v">BertTokenizer</span>.<span class="pl-en">from_pretrained</span>(<span class="pl-s1">model_version</span>, <span class="pl-s1">do_lower_case</span><span class="pl-c1">=</span><span class="pl-s1">do_lower_case</span>)
<span class="pl-en">show</span>(<span class="pl-s1">model</span>, <span class="pl-s1">model_type</span>, <span class="pl-s1">tokenizer</span>, <span class="pl-s1">sentence_a</span>, <span class="pl-s1">sentence_b</span>, <span class="pl-s1">layer</span><span class="pl-c1">=</span><span class="pl-c1">2</span>, <span class="pl-s1">head</span><span class="pl-c1">=</span><span class="pl-c1">0</span>)</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="# Import specialized versions of models (that return query/key vectors)
from bertviz.transformers_neuron_view import BertModel, BertTokenizer
from bertviz.neuron_view import show

model_type = 'bert'
model_version = 'bert-base-uncased'
do_lower_case = True
sentence_a = &quot;The cat sat on the mat&quot;
sentence_b = &quot;The cat lay on the rug&quot;
model = BertModel.from_pretrained(model_version, output_attentions=True)
tokenizer = BertTokenizer.from_pretrained(model_version, do_lower_case=do_lower_case)
show(model, model_type, tokenizer, sentence_a, sentence_b, layer=2, head=0)" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><b>Examples</b>:
BERT (<a href="/jessevig/bertviz/blob/master/notebooks/neuron_view_bert.ipynb">Notebook</a>,
<a href="https://colab.research.google.com/drive/1m37iotFeubMrp9qIf9yscXEL1zhxTN2b" rel="nofollow">Colab</a>) •
GPT-2 (<a href="/jessevig/bertviz/blob/master/notebooks/neuron_view_gpt2.ipynb">Notebook</a>,
<a href="https://colab.research.google.com/drive/1s8XCCyxsKvNRWNzjWi5Nl8ZAYZ5YkLm_" rel="nofollow">Colab</a>) •
RoBERTa
(<a href="/jessevig/bertviz/blob/master/notebooks/neuron_view_roberta.ipynb">Notebook</a>)</p>
<p dir="auto">For full API, please refer to the <a href="/jessevig/bertviz/blob/master/bertviz/neuron_view.py">source</a>.</p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto">Encoder-decoder models (BART, T5, etc.)</h3><a id="user-content-encoder-decoder-models-bart-t5-etc" class="anchor" aria-label="永久链接：编码器-解码器模型（BART、T5 等）" href="#encoder-decoder-models-bart-t5-etc"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">The head view and model view both support encoder-decoder models.</p>
<p dir="auto">First, load an encoder-decoder model:</p>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-k">from</span> <span class="pl-s1">transformers</span> <span class="pl-k">import</span> <span class="pl-v">AutoTokenizer</span>, <span class="pl-v">AutoModel</span>

<span class="pl-s1">tokenizer</span> <span class="pl-c1">=</span> <span class="pl-v">AutoTokenizer</span>.<span class="pl-en">from_pretrained</span>(<span class="pl-s">"Helsinki-NLP/opus-mt-en-de"</span>)
<span class="pl-s1">model</span> <span class="pl-c1">=</span> <span class="pl-v">AutoModel</span>.<span class="pl-en">from_pretrained</span>(<span class="pl-s">"Helsinki-NLP/opus-mt-en-de"</span>, <span class="pl-s1">output_attentions</span><span class="pl-c1">=</span><span class="pl-c1">True</span>)</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="from transformers import AutoTokenizer, AutoModel

tokenizer = AutoTokenizer.from_pretrained(&quot;Helsinki-NLP/opus-mt-en-de&quot;)
model = AutoModel.from_pretrained(&quot;Helsinki-NLP/opus-mt-en-de&quot;, output_attentions=True)" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto">Then prepare the inputs and compute attention:</p>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-s1">encoder_input_ids</span> <span class="pl-c1">=</span> <span class="pl-en">tokenizer</span>(<span class="pl-s">"She sees the small elephant."</span>, <span class="pl-s1">return_tensors</span><span class="pl-c1">=</span><span class="pl-s">"pt"</span>, <span class="pl-s1">add_special_tokens</span><span class="pl-c1">=</span><span class="pl-c1">True</span>).<span class="pl-s1">input_ids</span>
<span class="pl-k">with</span> <span class="pl-s1">tokenizer</span>.<span class="pl-en">as_target_tokenizer</span>():
    <span class="pl-s1">decoder_input_ids</span> <span class="pl-c1">=</span> <span class="pl-en">tokenizer</span>(<span class="pl-s">"Sie sieht den kleinen Elefanten."</span>, <span class="pl-s1">return_tensors</span><span class="pl-c1">=</span><span class="pl-s">"pt"</span>, <span class="pl-s1">add_special_tokens</span><span class="pl-c1">=</span><span class="pl-c1">True</span>).<span class="pl-s1">input_ids</span>

<span class="pl-s1">outputs</span> <span class="pl-c1">=</span> <span class="pl-en">model</span>(<span class="pl-s1">input_ids</span><span class="pl-c1">=</span><span class="pl-s1">encoder_input_ids</span>, <span class="pl-s1">decoder_input_ids</span><span class="pl-c1">=</span><span class="pl-s1">decoder_input_ids</span>)

<span class="pl-s1">encoder_text</span> <span class="pl-c1">=</span> <span class="pl-s1">tokenizer</span>.<span class="pl-en">convert_ids_to_tokens</span>(<span class="pl-s1">encoder_input_ids</span>[<span class="pl-c1">0</span>])
<span class="pl-s1">decoder_text</span> <span class="pl-c1">=</span> <span class="pl-s1">tokenizer</span>.<span class="pl-en">convert_ids_to_tokens</span>(<span class="pl-s1">decoder_input_ids</span>[<span class="pl-c1">0</span>])</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="encoder_input_ids = tokenizer(&quot;She sees the small elephant.&quot;, return_tensors=&quot;pt&quot;, add_special_tokens=True).input_ids
with tokenizer.as_target_tokenizer():
    decoder_input_ids = tokenizer(&quot;Sie sieht den kleinen Elefanten.&quot;, return_tensors=&quot;pt&quot;, add_special_tokens=True).input_ids

outputs = model(input_ids=encoder_input_ids, decoder_input_ids=decoder_input_ids)

encoder_text = tokenizer.convert_ids_to_tokens(encoder_input_ids[0])
decoder_text = tokenizer.convert_ids_to_tokens(decoder_input_ids[0])" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto">Finally, display the visualization using either <a href="/jessevig/bertviz/blob/master/bertviz/head_view.py"><code>head_view</code></a> or <a href="/jessevig/bertviz/blob/master/bertviz/model_view.py"><code>model_view</code></a>.</p>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-k">from</span> <span class="pl-s1">bertviz</span> <span class="pl-k">import</span> <span class="pl-s1">model_view</span>
<span class="pl-en">model_view</span>(
    <span class="pl-s1">encoder_attention</span><span class="pl-c1">=</span><span class="pl-s1">outputs</span>.<span class="pl-s1">encoder_attentions</span>,
    <span class="pl-s1">decoder_attention</span><span class="pl-c1">=</span><span class="pl-s1">outputs</span>.<span class="pl-s1">decoder_attentions</span>,
    <span class="pl-s1">cross_attention</span><span class="pl-c1">=</span><span class="pl-s1">outputs</span>.<span class="pl-s1">cross_attentions</span>,
    <span class="pl-s1">encoder_tokens</span><span class="pl-c1">=</span> <span class="pl-s1">encoder_text</span>,
    <span class="pl-s1">decoder_tokens</span> <span class="pl-c1">=</span> <span class="pl-s1">decoder_text</span>
)</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="from bertviz import model_view
model_view(
    encoder_attention=outputs.encoder_attentions,
    decoder_attention=outputs.decoder_attentions,
    cross_attention=outputs.cross_attentions,
    encoder_tokens= encoder_text,
    decoder_tokens = decoder_text
)" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto">You may select <code>Encoder</code>, <code>Decoder</code>, or <code>Cross</code> attention from the drop-down in the upper left corner of the visualization.</p>
<p dir="auto"><b>Examples</b>: MarianMT (<a href="/jessevig/bertviz/blob/master/notebooks/model_view_encoder_decoder.ipynb">Notebook</a>) • BART (<a href="/jessevig/bertviz/blob/master/notebooks/model_view_bart.ipynb">Notebook</a>)</p>
<p dir="auto">For full API, please refer to the source code for the <a href="/jessevig/bertviz/blob/master/bertviz/head_view.py">head view</a> or <a href="/jessevig/bertviz/blob/master/bertviz/model_view.py">model view</a>.</p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto">Installing from source</h3><a id="user-content-installing-from-source" class="anchor" aria-label="永久链接：从源安装" href="#installing-from-source"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>git clone https://github.com/jessevig/bertviz.git
<span class="pl-c1">cd</span> bertviz
python setup.py develop</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="git clone https://github.com/jessevig/bertviz.git
cd bertviz
python setup.py develop" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto">Additional options</h3><a id="user-content-additional-options" class="anchor" aria-label="永久链接：附加选项" href="#additional-options"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto">Dark / light mode</h4><a id="user-content-dark--light-mode" class="anchor" aria-label="永久链接：暗/亮模式" href="#dark--light-mode"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">The model view and neuron view support dark (default) and light modes. You may set the mode using
the <code>display_mode</code> parameter:</p>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-en">model_view</span>(<span class="pl-s1">attention</span>, <span class="pl-s1">tokens</span>, <span class="pl-s1">display_mode</span><span class="pl-c1">=</span><span class="pl-s">"light"</span>)</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="model_view(attention, tokens, display_mode=&quot;light&quot;)" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto">Filtering layers</h4><a id="user-content-filtering-layers" class="anchor" aria-label="永久链接：过滤层" href="#filtering-layers"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">To improve the responsiveness of the tool when visualizing larger models or inputs, you may set the <code>include_layers</code>
parameter to restrict the visualization to a subset of layers (zero-indexed). This option is available in the head view and model
view.</p>
<p dir="auto"><strong>Example:</strong> Render model view with only layers 5 and 6 displayed</p>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-en">model_view</span>(<span class="pl-s1">attention</span>, <span class="pl-s1">tokens</span>, <span class="pl-s1">include_layers</span><span class="pl-c1">=</span>[<span class="pl-c1">5</span>, <span class="pl-c1">6</span>])</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="model_view(attention, tokens, include_layers=[5, 6])" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto">For the model view, you may also restrict the visualization to a subset of attention heads (zero-indexed) by setting the
<code>include_heads</code> parameter.</p>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto">Setting default layer/head(s)</h4><a id="user-content-setting-default-layerheads" class="anchor" aria-label="永久链接：设置默认图层/头" href="#setting-default-layerheads"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">In the head view, you may choose a specific <code>layer</code> and collection of <code>heads</code> as the default selection when the
visualization first renders. Note: this is different from the <code>include_heads</code>/<code>include_layers</code> parameter (above), which
removes layers and heads from the visualization completely.</p>
<p dir="auto"><strong>Example:</strong> Render head view with layer 2 and heads 3 and 5 pre-selected</p>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-en">head_view</span>(<span class="pl-s1">attention</span>, <span class="pl-s1">tokens</span>, <span class="pl-s1">layer</span><span class="pl-c1">=</span><span class="pl-c1">2</span>, <span class="pl-s1">heads</span><span class="pl-c1">=</span>[<span class="pl-c1">3</span>,<span class="pl-c1">5</span>])</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="head_view(attention, tokens, layer=2, heads=[3,5])" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto">You may also pre-select a specific <code>layer</code> and single <code>head</code> for the neuron view.</p>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto">Visualizing sentence pairs</h4><a id="user-content-visualizing-sentence-pairs" class="anchor" aria-label="永久链接：可视化句子对" href="#visualizing-sentence-pairs"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">Some models, e.g. BERT, accept a pair of sentences as input. BertViz optionally supports a drop-down menu that allows
user to filter attention based on which sentence the tokens are in, e.g. only show attention between tokens in first
sentence and tokens in second sentence.</p>
<div class="markdown-heading" dir="auto"><h5 tabindex="-1" class="heading-element" dir="auto">Head and model views</h5><a id="user-content-head-and-model-views-1" class="anchor" aria-label="永久链接：头部和模型视图" href="#head-and-model-views-1"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">To enable this feature when invoking the <a href="/jessevig/bertviz/blob/master/bertviz/head_view.py"><code>head_view</code></a> or <a href="/jessevig/bertviz/blob/master/bertviz/model_view.py"><code>model_view</code></a> functions, set
the <code>sentence_b_start</code> parameter to the start index of the second sentence. Note that the method for computing this
index will depend on the model.</p>
<p dir="auto">Example (BERT):</p>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-k">from</span> <span class="pl-s1">bertviz</span> <span class="pl-k">import</span> <span class="pl-s1">head_view</span>
<span class="pl-k">from</span> <span class="pl-s1">transformers</span> <span class="pl-k">import</span> <span class="pl-v">AutoTokenizer</span>, <span class="pl-v">AutoModel</span>, <span class="pl-s1">utils</span>
<span class="pl-s1">utils</span>.<span class="pl-s1">logging</span>.<span class="pl-en">set_verbosity_error</span>()  <span class="pl-c"># Suppress standard warnings</span>

<span class="pl-c"># NOTE: This code is model-specific</span>
<span class="pl-s1">model_version</span> <span class="pl-c1">=</span> <span class="pl-s">'bert-base-uncased'</span>
<span class="pl-s1">model</span> <span class="pl-c1">=</span> <span class="pl-v">AutoModel</span>.<span class="pl-en">from_pretrained</span>(<span class="pl-s1">model_version</span>, <span class="pl-s1">output_attentions</span><span class="pl-c1">=</span><span class="pl-c1">True</span>)
<span class="pl-s1">tokenizer</span> <span class="pl-c1">=</span> <span class="pl-v">AutoTokenizer</span>.<span class="pl-en">from_pretrained</span>(<span class="pl-s1">model_version</span>)
<span class="pl-s1">sentence_a</span> <span class="pl-c1">=</span> <span class="pl-s">"the rabbit quickly hopped"</span>
<span class="pl-s1">sentence_b</span> <span class="pl-c1">=</span> <span class="pl-s">"The turtle slowly crawled"</span>
<span class="pl-s1">inputs</span> <span class="pl-c1">=</span> <span class="pl-s1">tokenizer</span>.<span class="pl-en">encode_plus</span>(<span class="pl-s1">sentence_a</span>, <span class="pl-s1">sentence_b</span>, <span class="pl-s1">return_tensors</span><span class="pl-c1">=</span><span class="pl-s">'pt'</span>)
<span class="pl-s1">input_ids</span> <span class="pl-c1">=</span> <span class="pl-s1">inputs</span>[<span class="pl-s">'input_ids'</span>]
<span class="pl-s1">token_type_ids</span> <span class="pl-c1">=</span> <span class="pl-s1">inputs</span>[<span class="pl-s">'token_type_ids'</span>] <span class="pl-c"># token type id is 0 for Sentence A and 1 for Sentence B</span>
<span class="pl-s1">attention</span> <span class="pl-c1">=</span> <span class="pl-en">model</span>(<span class="pl-s1">input_ids</span>, <span class="pl-s1">token_type_ids</span><span class="pl-c1">=</span><span class="pl-s1">token_type_ids</span>)[<span class="pl-c1">-</span><span class="pl-c1">1</span>]
<span class="pl-s1">sentence_b_start</span> <span class="pl-c1">=</span> <span class="pl-s1">token_type_ids</span>[<span class="pl-c1">0</span>].<span class="pl-en">tolist</span>().<span class="pl-en">index</span>(<span class="pl-c1">1</span>) <span class="pl-c"># Sentence B starts at first index of token type id 1</span>
<span class="pl-s1">token_ids</span> <span class="pl-c1">=</span> <span class="pl-s1">input_ids</span>[<span class="pl-c1">0</span>].<span class="pl-en">tolist</span>() <span class="pl-c"># Batch index 0</span>
<span class="pl-s1">tokens</span> <span class="pl-c1">=</span> <span class="pl-s1">tokenizer</span>.<span class="pl-en">convert_ids_to_tokens</span>(<span class="pl-s1">token_ids</span>)    
<span class="pl-en">head_view</span>(<span class="pl-s1">attention</span>, <span class="pl-s1">tokens</span>, <span class="pl-s1">sentence_b_start</span>)</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="from bertviz import head_view
from transformers import AutoTokenizer, AutoModel, utils
utils.logging.set_verbosity_error()  # Suppress standard warnings

# NOTE: This code is model-specific
model_version = 'bert-base-uncased'
model = AutoModel.from_pretrained(model_version, output_attentions=True)
tokenizer = AutoTokenizer.from_pretrained(model_version)
sentence_a = &quot;the rabbit quickly hopped&quot;
sentence_b = &quot;The turtle slowly crawled&quot;
inputs = tokenizer.encode_plus(sentence_a, sentence_b, return_tensors='pt')
input_ids = inputs['input_ids']
token_type_ids = inputs['token_type_ids'] # token type id is 0 for Sentence A and 1 for Sentence B
attention = model(input_ids, token_type_ids=token_type_ids)[-1]
sentence_b_start = token_type_ids[0].tolist().index(1) # Sentence B starts at first index of token type id 1
token_ids = input_ids[0].tolist() # Batch index 0
tokens = tokenizer.convert_ids_to_tokens(token_ids)    
head_view(attention, tokens, sentence_b_start)" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h5 tabindex="-1" class="heading-element" dir="auto">Neuron view</h5><a id="user-content-neuron-view-2" class="anchor" aria-label="永久链接：神经元视图" href="#neuron-view-2"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">To enable this option in the neuron view, simply set the <code>sentence_a</code> and <code>sentence_b</code> parameters in <a href="/jessevig/bertviz/blob/master/bertviz/neuron_view.py"><code>neuron_view.show()</code></a>.</p>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto">Obtain HTML representations</h4><a id="user-content-obtain-html-representations" class="anchor" aria-label="永久链接：获取 HTML 表示" href="#obtain-html-representations"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">Support to retrieve the generated HTML representations has been added to head_view, model_view and neuron_view.</p>
<p dir="auto">Setting the 'html_action' parameter to 'return' will make the function call return a single HTML Python object that can be further processed. Remember you can access the HTML source using the data attribute of a Python HTML object.</p>
<p dir="auto">The default behavior for 'html_action' is 'view', which will display the visualization but won't return the HTML object.</p>
<p dir="auto">This functionality is useful if you need to:</p>
<ul dir="auto">
<li>Save the representation as an independent HTML file that can be accessed via web browser</li>
<li>Use custom display methods as the ones needed in Databricks to visualize HTML objects</li>
</ul>
<p dir="auto">Example (head and model views):</p>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-k">from</span> <span class="pl-s1">transformers</span> <span class="pl-k">import</span> <span class="pl-v">AutoTokenizer</span>, <span class="pl-v">AutoModel</span>, <span class="pl-s1">utils</span>
<span class="pl-k">from</span> <span class="pl-s1">bertviz</span> <span class="pl-k">import</span> <span class="pl-s1">head_view</span>

<span class="pl-s1">utils</span>.<span class="pl-s1">logging</span>.<span class="pl-en">set_verbosity_error</span>()  <span class="pl-c"># Suppress standard warnings</span>
<span class="pl-s1">tokenizer</span> <span class="pl-c1">=</span> <span class="pl-v">AutoTokenizer</span>.<span class="pl-en">from_pretrained</span>(<span class="pl-s">"bert-base-uncased"</span>)
<span class="pl-s1">model</span> <span class="pl-c1">=</span> <span class="pl-v">AutoModel</span>.<span class="pl-en">from_pretrained</span>(<span class="pl-s">"bert-base-uncased"</span>, <span class="pl-s1">output_attentions</span><span class="pl-c1">=</span><span class="pl-c1">True</span>)

<span class="pl-s1">inputs</span> <span class="pl-c1">=</span> <span class="pl-s1">tokenizer</span>.<span class="pl-en">encode</span>(<span class="pl-s">"The cat sat on the mat"</span>, <span class="pl-s1">return_tensors</span><span class="pl-c1">=</span><span class="pl-s">'pt'</span>)
<span class="pl-s1">outputs</span> <span class="pl-c1">=</span> <span class="pl-en">model</span>(<span class="pl-s1">inputs</span>)
<span class="pl-s1">attention</span> <span class="pl-c1">=</span> <span class="pl-s1">outputs</span>[<span class="pl-c1">-</span><span class="pl-c1">1</span>]  <span class="pl-c"># Output includes attention weights when output_attentions=True</span>
<span class="pl-s1">tokens</span> <span class="pl-c1">=</span> <span class="pl-s1">tokenizer</span>.<span class="pl-en">convert_ids_to_tokens</span>(<span class="pl-s1">inputs</span>[<span class="pl-c1">0</span>]) 

<span class="pl-s1">html_head_view</span> <span class="pl-c1">=</span> <span class="pl-en">head_view</span>(<span class="pl-s1">attention</span>, <span class="pl-s1">tokens</span>, <span class="pl-s1">html_action</span><span class="pl-c1">=</span><span class="pl-s">'return'</span>)

<span class="pl-k">with</span> <span class="pl-en">open</span>(<span class="pl-s">"PATH_TO_YOUR_FILE/head_view.html"</span>, <span class="pl-s">'w'</span>) <span class="pl-k">as</span> <span class="pl-s1">file</span>:
    <span class="pl-s1">file</span>.<span class="pl-en">write</span>(<span class="pl-s1">html_head_view</span>.<span class="pl-s1">data</span>)</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="from transformers import AutoTokenizer, AutoModel, utils
from bertviz import head_view

utils.logging.set_verbosity_error()  # Suppress standard warnings
tokenizer = AutoTokenizer.from_pretrained(&quot;bert-base-uncased&quot;)
model = AutoModel.from_pretrained(&quot;bert-base-uncased&quot;, output_attentions=True)

inputs = tokenizer.encode(&quot;The cat sat on the mat&quot;, return_tensors='pt')
outputs = model(inputs)
attention = outputs[-1]  # Output includes attention weights when output_attentions=True
tokens = tokenizer.convert_ids_to_tokens(inputs[0]) 

html_head_view = head_view(attention, tokens, html_action='return')

with open(&quot;PATH_TO_YOUR_FILE/head_view.html&quot;, 'w') as file:
    file.write(html_head_view.data)
" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto">Example (neuron view):</p>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c"># Import specialized versions of models (that return query/key vectors)</span>
<span class="pl-k">from</span> <span class="pl-s1">bertviz</span>.<span class="pl-s1">transformers_neuron_view</span> <span class="pl-k">import</span> <span class="pl-v">BertModel</span>, <span class="pl-v">BertTokenizer</span>
<span class="pl-k">from</span> <span class="pl-s1">bertviz</span>.<span class="pl-s1">neuron_view</span> <span class="pl-k">import</span> <span class="pl-s1">show</span>

<span class="pl-s1">model_type</span> <span class="pl-c1">=</span> <span class="pl-s">'bert'</span>
<span class="pl-s1">model_version</span> <span class="pl-c1">=</span> <span class="pl-s">'bert-base-uncased'</span>
<span class="pl-s1">do_lower_case</span> <span class="pl-c1">=</span> <span class="pl-c1">True</span>
<span class="pl-s1">sentence_a</span> <span class="pl-c1">=</span> <span class="pl-s">"The cat sat on the mat"</span>
<span class="pl-s1">sentence_b</span> <span class="pl-c1">=</span> <span class="pl-s">"The cat lay on the rug"</span>
<span class="pl-s1">model</span> <span class="pl-c1">=</span> <span class="pl-v">BertModel</span>.<span class="pl-en">from_pretrained</span>(<span class="pl-s1">model_version</span>, <span class="pl-s1">output_attentions</span><span class="pl-c1">=</span><span class="pl-c1">True</span>)
<span class="pl-s1">tokenizer</span> <span class="pl-c1">=</span> <span class="pl-v">BertTokenizer</span>.<span class="pl-en">from_pretrained</span>(<span class="pl-s1">model_version</span>, <span class="pl-s1">do_lower_case</span><span class="pl-c1">=</span><span class="pl-s1">do_lower_case</span>)
<span class="pl-s1">html_neuron_view</span> <span class="pl-c1">=</span> <span class="pl-en">show</span>(<span class="pl-s1">model</span>, <span class="pl-s1">model_type</span>, <span class="pl-s1">tokenizer</span>, <span class="pl-s1">sentence_a</span>, <span class="pl-s1">sentence_b</span>, <span class="pl-s1">layer</span><span class="pl-c1">=</span><span class="pl-c1">2</span>, <span class="pl-s1">head</span><span class="pl-c1">=</span><span class="pl-c1">0</span>, <span class="pl-s1">html_action</span><span class="pl-c1">=</span><span class="pl-s">'return'</span>)

<span class="pl-k">with</span> <span class="pl-en">open</span>(<span class="pl-s">"PATH_TO_YOUR_FILE/neuron_view.html"</span>, <span class="pl-s">'w'</span>) <span class="pl-k">as</span> <span class="pl-s1">file</span>:
    <span class="pl-s1">file</span>.<span class="pl-en">write</span>(<span class="pl-s1">html_neuron_view</span>.<span class="pl-s1">data</span>)</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="# Import specialized versions of models (that return query/key vectors)
from bertviz.transformers_neuron_view import BertModel, BertTokenizer
from bertviz.neuron_view import show

model_type = 'bert'
model_version = 'bert-base-uncased'
do_lower_case = True
sentence_a = &quot;The cat sat on the mat&quot;
sentence_b = &quot;The cat lay on the rug&quot;
model = BertModel.from_pretrained(model_version, output_attentions=True)
tokenizer = BertTokenizer.from_pretrained(model_version, do_lower_case=do_lower_case)
html_neuron_view = show(model, model_type, tokenizer, sentence_a, sentence_b, layer=2, head=0, html_action='return')

with open(&quot;PATH_TO_YOUR_FILE/neuron_view.html&quot;, 'w') as file:
    file.write(html_neuron_view.data)" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto">Non-Huggingface models</h4><a id="user-content-non-huggingface-models" class="anchor" aria-label="永久链接：非 Huggingface 模型" href="#non-huggingface-models"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">The head view and model view may be used to
visualize self-attention for any standard Transformer model,
as long as the attention weights are available and follow the format specified in <a href="/jessevig/bertviz/blob/master/bertviz/head_view.py"><code>head_view</code></a> and
<a href="/jessevig/bertviz/blob/master/bertviz/model_view.py"><code>model_view</code></a> (which is the format
returned from Huggingface models). In some case, Tensorflow checkpoints may be loaded as Huggingface models as described
in the
<a href="https://huggingface.co/transformers/" rel="nofollow">Huggingface docs</a>.</p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><g-emoji class="g-emoji" alias="warning">⚠️</g-emoji> Limitations</h3><a id="user-content-️-limitations" class="anchor" aria-label="永久链接：⚠️ 限制" href="#️-limitations"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto">Tool</h4><a id="user-content-tool" class="anchor" aria-label="永久链接：工具" href="#tool"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">该工具专为较短的输入而设计，如果输入文本很长和/或模型很大，则可能会运行缓慢。为了缓解这种情况，您可能希望通过设置参数</font><a href="#filtering-layers"><font style="vertical-align: inherit;">来</font></a><font style="vertical-align: inherit;">过滤显示的图层</font></font><strong><code>include_layers</code></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，如上所述</font><font style="vertical-align: inherit;">。</font></font><a href="#filtering-layers"><font style="vertical-align: inherit;"></font></a><font style="vertical-align: inherit;"></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在 Colab 上运行时，当输入文本较长时，某些可视化将失败（运行时断开连接）。为了缓解这种情况，您可能希望通过设置参数</font><a href="#filtering-layers"><font style="vertical-align: inherit;">来</font></a><font style="vertical-align: inherit;">过滤显示的图层</font></font><strong><code>include_layers</code></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，如上所述</font><font style="vertical-align: inherit;">。</font></font><a href="#filtering-layers"><font style="vertical-align: inherit;"></font></a><font style="vertical-align: inherit;"></font></li>
<li><font style="vertical-align: inherit;"></font><em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">神经元视图</font></font></em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">仅</font><font style="vertical-align: inherit;">支持该工具附带的自定义 BERT、GPT-2 和 RoBERTa 模型。该视图需要访问查询和键向量，这需要修改模型代码（参见</font></font><code>transformers_neuron_view</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">目录），仅对这三个模型进行了修改。</font></font></li>
</ul>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">注意力作为“解释”？</font></font></h4><a id="user-content-attention-as-explanation" class="anchor" aria-label="永久链接：注意力作为“解释”？" href="#attention-as-explanation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">可视化注意力</font><font style="vertical-align: inherit;">权</font><a href="https://arxiv.org/pdf/1908.04626.pdf" rel="nofollow"><font style="vertical-align: inherit;">重阐明了模型内的一种架构</font></a><a href="https://arxiv.org/abs/1902.10186" rel="nofollow"><font style="vertical-align: inherit;">，</font></a><font style="vertical-align: inherit;">但不一定为预测提供直接</font></font><em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">解释</font></font></em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">[ </font></font><a href="https://arxiv.org/pdf/1909.11218.pdf" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">1,2,3</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;"> ]。</font></font><a href="https://arxiv.org/abs/1902.10186" rel="nofollow"><font style="vertical-align: inherit;"></font></a><font style="vertical-align: inherit;"></font><a href="https://arxiv.org/pdf/1908.04626.pdf" rel="nofollow"><font style="vertical-align: inherit;"></font></a><font style="vertical-align: inherit;"></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如果您希望了解输入文本如何更直接地影响输出预测，请考虑</font><a href="https://github.com/PAIR-code/lit"><font style="vertical-align: inherit;">Language Interpretability Toolkit</font></a><font style="vertical-align: inherit;">或</font><a href="https://github.com/jalammar/ecco"><font style="vertical-align: inherit;">Ecco</font></a><font style="vertical-align: inherit;">等工具提供的</font></font><a href="https://arxiv.org/pdf/2010.05607.pdf" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">显着性方法</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font><a href="https://github.com/PAIR-code/lit"><font style="vertical-align: inherit;"></font></a><font style="vertical-align: inherit;"></font><a href="https://github.com/jalammar/ecco"><font style="vertical-align: inherit;"></font></a><font style="vertical-align: inherit;"></font></li>
</ul>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">🔬 纸</font></font></h2><a id="user-content--paper" class="anchor" aria-label="永久链接：🔬纸" href="#-paper"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><a href="https://www.aclweb.org/anthology/P19-3007.pdf" rel="nofollow"><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Transformer 模型中注意力的多尺度可视化</font></font></b></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（ACL 系统演示 2019）。</font></font></p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">引文</font></font></h3><a id="user-content-citation" class="anchor" aria-label="永久链接：引文" href="#citation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="highlight highlight-text-bibtex notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-k">@inproceedings</span>{<span class="pl-en">vig-2019-multiscale</span>,
    <span class="pl-s">title</span> = <span class="pl-s"><span class="pl-pds">"</span>A Multiscale Visualization of Attention in the Transformer Model<span class="pl-pds">"</span></span>,
    <span class="pl-s">author</span> = <span class="pl-s"><span class="pl-pds">"</span>Vig, Jesse<span class="pl-pds">"</span></span>,
    <span class="pl-s">booktitle</span> = <span class="pl-s"><span class="pl-pds">"</span>Proceedings of the 57th Annual Meeting of the Association for Computational Linguistics: System Demonstrations<span class="pl-pds">"</span></span>,
    <span class="pl-s">month</span> = jul,
    <span class="pl-s">year</span> = <span class="pl-s"><span class="pl-pds">"</span>2019<span class="pl-pds">"</span></span>,
    <span class="pl-s">address</span> = <span class="pl-s"><span class="pl-pds">"</span>Florence, Italy<span class="pl-pds">"</span></span>,
    <span class="pl-s">publisher</span> = <span class="pl-s"><span class="pl-pds">"</span>Association for Computational Linguistics<span class="pl-pds">"</span></span>,
    <span class="pl-s">url</span> = <span class="pl-s"><span class="pl-pds">"</span>https://www.aclweb.org/anthology/P19-3007<span class="pl-pds">"</span></span>,
    <span class="pl-s">doi</span> = <span class="pl-s"><span class="pl-pds">"</span>10.18653/v1/P19-3007<span class="pl-pds">"</span></span>,
    <span class="pl-s">pages</span> = <span class="pl-s"><span class="pl-pds">"</span>37--42<span class="pl-pds">"</span></span>,
}</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="@inproceedings{vig-2019-multiscale,
    title = &quot;A Multiscale Visualization of Attention in the Transformer Model&quot;,
    author = &quot;Vig, Jesse&quot;,
    booktitle = &quot;Proceedings of the 57th Annual Meeting of the Association for Computational Linguistics: System Demonstrations&quot;,
    month = jul,
    year = &quot;2019&quot;,
    address = &quot;Florence, Italy&quot;,
    publisher = &quot;Association for Computational Linguistics&quot;,
    url = &quot;https://www.aclweb.org/anthology/P19-3007&quot;,
    doi = &quot;10.18653/v1/P19-3007&quot;,
    pages = &quot;37--42&quot;,
}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">作者</font></font></h2><a id="user-content-authors" class="anchor" aria-label="永久链接：作者" href="#authors"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><a href="https://twitter.com/jesse_vig" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">杰西·维格</font></font></a></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">🙏致谢</font></font></h2><a id="user-content--acknowledgments" class="anchor" aria-label="永久链接：🙏致谢" href="#-acknowledgments"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们感谢以下项目的作者，这些项目已纳入此存储库：</font></font></p>
<ul dir="auto">
<li><a href="https://github.com/tensorflow/tensor2tensor"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">https://github.com/tensorflow/tensor2tensor</font></font></a></li>
<li><a href="https://github.com/huggingface/pytorch-pretrained-BERT"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">https://github.com/huggingface/pytorch-pretrained-BERT</font></font></a></li>
</ul>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">执照</font></font></h2><a id="user-content-license" class="anchor" aria-label="永久链接：许可证" href="#license"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">该项目根据 Apache 2.0 许可证获得许可 -</font><font style="vertical-align: inherit;">有关详细信息，请参阅</font></font><a href="/jessevig/bertviz/blob/master/LICENSE"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">许可证文件</font></font></a><font style="vertical-align: inherit;"></font></p>
</article></div>
