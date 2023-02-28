---
permalink: /
title: "academicpages is a ready-to-fork GitHub Pages template for academic personal websites"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

This is the front page of a website that is powered by the [academicpages template](https://github.com/academicpages/academicpages.github.io) and hosted on GitHub pages. [GitHub pages](https://pages.github.com) is a free service in which websites are built and hosted from code and data stored in a GitHub repository, automatically updating when a new commit is made to the respository. This template was forked from the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/) created by Michael Rose, and then extended to support the kinds of content that academics have: publications, talks, teaching, a portfolio, blog posts, and a dynamically-generated CV. You can fork [this repository](https://github.com/academicpages/academicpages.github.io) right now, modify the configuration and markdown files, add your own PDFs and other content, and have your own site for free, with no ads! An older version of this template powers my own personal website at [stuartgeiger.com](http://stuartgeiger.com), which uses [this Github repository](https://github.com/staeiou/staeiou.github.io).

A data-driven personal website
======
Like many other Jekyll-based GitHub Pages templates, academicpages makes you separate the website's content from its form. The content & metadata of your website are in structured markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over -- just be sure to save the markdown files! Finally, you can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html).

Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

I have also created [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the academicpages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring academicpages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.

<table boarder="0" cellspacing="0" cellpadding="0">
    <tr>
        <td width="20%">2018</td>
        <td>我转专业至上海交通大学设计学院建筑学系</td>
    </tr>
    <tr>
        <td width="20%">2023</td>
        <td>本科毕业</td>
    </tr>
</table>

[时间安排](%E6%AF%95%E4%B8%9A%E8%AE%BE%E8%AE%A1+aa487dfe-fbfc-4e8a-adb8-cd816b3b2904/%E6%97%B6%E9%97%B4%E5%AE%89%E6%8E%92%202d70eb94-3ecf-4053-a536-95b5381be321.csv)

# 文献阅读及调研、方案构思

- [上海一江一河规划以及黄浦江客运与水运规划与情况的调查](https://flowus.cn/5c6bb8ef-8b94-400b-be46-069c039a525d)；

- [国内外最新滨水步道、公共空间以及客运码头的案例、研究等收集整理](https://flowus.cn/dd7fdafd-d830-473b-b417-49fa7a59cf6f)；@周茉

- [国内外最新城市设计，组团和街区等设计的案例收集整理，关注非居住的商业和公共街区](https://flowus.cn/4a08fa26-9b13-495e-897e-3d852373de54)；@胡啸

- [国内外城市新技术在设计、建设、节能等方面的前沿应用与案例](https://flowus.cn/f8e763c2-9c6d-4e00-af0b-047b6f835eef)；@温世康

# 研究方向

基于VR和眼动追踪数据的TOD通道空间



  程序（游戏？）开发

    **支持建筑模型导入**
以便于重复修改迭代

      支持渲染？

    **面向大众发布**
以增加数据样本容量

      吸引力？

      元宇宙概念为平台？

    **后台收集数据**
以导出处理数据

  数据处理

    数据类型

      VR数据

        停留点

        某个停留点的停留时间

        行进路线

      眼动追踪数据

        视觉停留点

          街道界面

          街道路面

          不同材质的表皮

          ……

        扫描路径

        停留时间

        频次

    权重分配

    可视化

  目前问题

    如何与TOD联系起来？

    如何将论文中的城市设计成果迁移到建筑设计中去？
即该设计方法可以同时应用在城市设计和建筑设计中的哪些地方？我该怎样找到它们之间的联系

  研究问题

    ~~TOD垂直交通空间设计？~~

      空间节点

      空间边界

      空间组织方式

      与其他空间结合后形成的复杂界面对交通空间的干扰？

        有什么干扰

        为什么会干扰

          材质

          空间形态被改变

          空间氛围distract

        怎样干扰？

        干扰了哪一部分人

        在哪个场景最容易产生这种干扰

    TOD 通道空间设计

      引导性

        自然光线

        高宽比

        可视化、广告的影响

        材质

        ……

> ~~利用元宇宙可以快速建设和修改的特性，不断收集元宇宙中的虚拟数据（交通？、眼动数据）指导现实的TOD综合体设计（VTOD）~~

> ~~根据不同的设计建立沉浸式场景（全景图片、VR环境），收集眼球停留数据、在某个场景的停留时间、行走流线，指导设计方案的选择~~

> ~~根据相同的设计建立沉浸式场景（全景图片、VR环境），收集眼球停留数据、在某个场景的停留时间、行走流线，指导设计方案的深化~~

## 技术路线

### 硬件：集成眼动追踪技术的VR设备（PICO）





[zhuanlan.zhihu.com](https://zhuanlan.zhihu.com/p/210463354)
你需要了解的人类眼动的背景知识



[zhuanlan.zhihu.com](https://zhuanlan.zhihu.com/p/509381410)
PICO SDK导入Unity





[developer-cn.pico-interactive.com](https://developer-cn.pico-interactive.com/developer-program)
PICO开发者计划





### 软件：算法实现（数据收集、数据处理）





![Screenshot_2023-02-24-21-23-27-111_tv.danmaku.bili.jpg](毕业设计+aa487dfe-fbfc-4e8a-adb8-cd816b3b2904/Screenshot_2023-02-24-21-23-27-111_tv.danmaku.bili.jpg)

[HTC VIVE pro eye + Unity SDK 研究记录 · 语雀](https://www.yuque.com/ogongqingo/fac2z4/yu9vb3)
代码



[https://www.bilibili.com/video/BV1FL41157F2/?spm_id_from=333.999.0.0](https://www.bilibili.com/video/BV1FL41157F2/?spm_id_from=333.999.0.0)

[眼动追踪技术中8个常用指标与术语](https://zhuanlan.zhihu.com/p/73949336)
眼动追踪生成的数据类型

[Unity - Getting started - Tobii Pro SDK documentation](https://developer.tobiipro.com/unity/unity-getting-started.html)
Tobbi SDK API 

[HTC Vive Pro eye 眼动数据简单获取_htc vive pro eye眼动数据简单获取_Farewell弈的博客-CSDN博客](https://blog.csdn.net/qq_41205665/article/details/124409733)

【2022C#Unity3D/UnityVR零基础教程(U3D零基础教程/VR全景图片/VR视频播放/VR相机旋转/零基础U3D学习资源）B0315-哔哩哔哩】 [https://b23.tv/3DBtYiE](https://b23.tv/3DBtYiE)

![设计方法图解](毕业设计+aa487dfe-fbfc-4e8a-adb8-cd816b3b2904/7eb3aafa614d4b3aacf49105dcfdee7.jpg)
设计方法图解

## 文献阅读

[待读文献](%E6%AF%95%E4%B8%9A%E8%AE%BE%E8%AE%A1+aa487dfe-fbfc-4e8a-adb8-cd816b3b2904/%E5%BE%85%E8%AF%BB%E6%96%87%E7%8C%AE%20f7374b1b-d99a-4df2-a46d-88ca4d2ee210.md)





[基于Unity3D的眼动数据收集及处理方法](毕业设计+aa487dfe-fbfc-4e8a-adb8-cd816b3b2904/基于VR眼动数据的空间环境...喀什高台民居保护与设计为例_臧伟.pdf)
基于Unity3D的眼动数据收集及处理方法



[kns.cnki.net](https://kns.cnki.net/kcms2/article/abstract?v=3uoqIhG8C475KOm_zrgu4sq25HxUBNNTmIbFx6y0bOQ0cH_CuEtpsBxp_L8clkajdG2mwoGABMuN0gHRb3QEX1G3vNJp3Fit&uniplatform=NZKPT)
应用：基于VR和眼动仪的步行商业街侧界面形态设计与感知研究



