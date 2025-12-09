---
title: "PUC Minas | Mei a Mei"
date: 2024-11-29
draft: false
description: "一个描述"
tags: [ "featured project", "PUC Minas", "software", "development", "javascript", "mongoDB", "React.js", "React Native" ]
---
<head>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</head>
  <script>
    // 处理模态显示的脚本
    window.onclick = function(event) {
      var modal = document.getElementById('meiModal');
      if (event.target == modal) {
        modal.style.display = "none";
      }
    }
    // 处理使用 Esc 键关闭模态的脚本
    document.onkeydown = function(event) {
      var modal = document.getElementById('meiModal');
      if (event.key === "Escape") {
        modal.style.display = "none";
      }
    }
  </script>
{{< alert "star" >}}
**特色项目** - 第二学年
{{< /alert >}}

>**2024年第一学期**

一款面向处于 MEI 税制下创业者的移动应用与网页系统，旨在帮助他们管理营收并保持在法定限额之内。目标是创建提醒，当创业者接近该类别的营收上限时及时通知。此外，系统提供管理支出与收入的方式，生成报告和图表，帮助他们理解自身的财务状况。

<div style="display: flex; gap: 10px; align-items: center;">

### MEI

<button onclick="document.getElementById('meiModal').style.display='block'">
  <i class="fas fa-info-circle" title="点击了解更多关于 MEI 的信息"></i>
</button>

</div>

宣传视频（葡语）

{{< youtubeLite id="uXs_BRr0ye4" label="演示视频" >}}

**使用技术**：C#、.NET、ASP.NET Core、React.js、React Native、MongoDB、MongoDB Atlas、MongoDB Compass、RESTful API、Swagger、Postman、Visual Studio 2022、VSCode、Rider、Figma、Trello、Git、Github、NUnit、XUnit

- [网站演示](https://meiameipuc.azurewebsites.net/)

- 登录：gg@email.com

- 密码：12345

> 部署在免费的 Azure 服务器上，因此启动可能需要一些时间。

### 网页系统

{{< gallery >}}
  <img src="featured.png"           class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei1.png" class="grid-w500 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei2.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei3.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei4.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei5.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
{{< /gallery >}}

### 移动应用

{{< gallery >}}
  <img src="gallery/Mei01.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei02.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei03.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei04.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei05.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei06.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
{{< /gallery >}}

您可以在 `GitHub Repository` 中找到更多项目信息。
{{< github repo="ICEI-PUC-Minas-PMV-ADS/pmv-ads-2024-1-e4-proj-dad-t3-mei" >}}

<!-- 模态框 -->
<div id="meiModal" class="modal">
  <div class="modal-content">
    <span class="close" onclick="document.getElementById('meiModal').style.display='none'">&times;</span>
    <h2>
      <i class="fas fa-info-circle" ></i>
      什么是 MEI？
      </h2>
      <p>MEI 是 “Microempreendedor Individual”（个体微型企业家）的缩写。这是巴西为希望将业务正规化的小企业主设立的一种企业类型。MEI 享有简化的税务义务与较少的官僚手续。</p>
  </div>
</div>
