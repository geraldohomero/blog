---
title: "PUC Minas | Mei a Mei"
date: 2024-11-29
draft: false
description: "a description"
tags: [ "featured project", "PUC Minas", "software", "development", "javascript", "mongoDB", "React.js", "React Native" ]
---
<head>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</head>
  <script>
    // Script to handle modal display
    window.onclick = function(event) {
      var modal = document.getElementById('meiModal');
      if (event.target == modal) {
        modal.style.display = "none";
      }
    }
    // Script to handle closing modal with Esc key
    document.onkeydown = function(event) {
      var modal = document.getElementById('meiModal');
      if (event.key === "Escape") {
        modal.style.display = "none";
      }
    }
  </script>
{{< alert "star" >}}
**Featured Project** - Second Year
{{< /alert >}}

>**First Semester of 2024**


A mobile app and web system designed to assist entrepreneurs under the MEI tax regime in managing their revenue and staying within the legal limits. The goal is to create alerts that notify the entrepreneur when they are nearing the category's revenue limit. Also, the system provides a way to manage the entrepreneur's expenses and revenue, generating reports and graphs to help them understand their financial situation.


<div style="display: flex; gap: 10px; align-items: center;">

### MEI

<button onclick="document.getElementById('meiModal').style.display='block'">
  <i class="fas fa-info-circle" title="Click for more information about MEI"></i>
</button>

</div>

Promotional Video (in Portuguese)

{{< youtubeLite id="uXs_BRr0ye4" label="Demo Video" >}}


**Technologies**: C#, .NET, ASP.NET Core, React.js, React Native, MongoDB, MongoDB Atlas, MongoDB Compass, RESTful API, Swagger, Postman, Visual Studio 2022, VSCode, Rider, Figma, Trello, Git, Github, NUnit, XUnit

- [Website Demo](https://meiameipuc.azurewebsites.net/)

- Login: gg@email.com

- Password: 12345

> It is hosted on a free Azure server, so it may take a while to start up.

### Web System 

{{< gallery >}}
  <img src="featured.png"           class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei1.png" class="grid-w500 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei2.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei3.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei4.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei5.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
{{< /gallery >}}

### Mobile App

{{< gallery >}}
  <img src="gallery/Mei01.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei02.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei03.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei04.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei05.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei06.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
{{< /gallery >}}


You can find more information about the project in the `GitHub Repository`.
{{< github repo="ICEI-PUC-Minas-PMV-ADS/pmv-ads-2024-1-e4-proj-dad-t3-mei" >}}


<!-- The Modal -->
<div id="meiModal" class="modal">
  <div class="modal-content">
    <span class="close" onclick="document.getElementById('meiModal').style.display='none'">&times;</span>
    <h2>
      <i class="fas fa-info-circle" ></i>
      What is MEI?
      </h2>
      <p>MEI stands for Microempreendedor Individual (Individual Microentrepreneur). It is a type of business entity in Brazil designed for small business owners who want to formalize their business activities. MEIs benefit from simplified tax obligations and reduced bureaucracy.</p>
  </div>
</div>

