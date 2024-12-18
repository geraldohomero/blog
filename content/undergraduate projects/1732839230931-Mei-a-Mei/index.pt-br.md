---
title: "PUC Minas | Mei a Mei"
date: 2024-11-29
draft: false
description: "uma descrição"
tags: [ "projeto em destaque", "PUC Minas", "software", "desenvolvimento", "javascript", "mongoDB", "React.js", "React Native" ]
---
<head>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</head>
  <script>
    // Script para lidar com a exibição do modal
    window.onclick = function(event) {
      var modal = document.getElementById('meiModal');
      if (event.target == modal) {
        modal.style.display = "none";
      }
    }
    // Script para fechar o modal com a tecla Esc
    document.onkeydown = function(event) {
      var modal = document.getElementById('meiModal');
      if (event.key === "Escape") {
        modal.style.display = "none";
      }
    }
  </script>
{{< alert "star" >}}
**Projeto Destaque** - Segundo Ano
{{< /alert >}}

>**Primeiro Semestre de 2024**


Um aplicativo móvel e sistema web projetado para auxiliar empreendedores sob o regime tributário MEI na gestão de suas receitas e na permanência dentro dos limites legais. O objetivo é criar alertas que notifiquem o empreendedor quando ele estiver se aproximando do limite de receita da categoria. Além disso, o sistema fornece uma maneira de gerenciar as despesas e receitas do empreendedor, gerando relatórios e gráficos para ajudá-lo a entender sua situação financeira.


<div style="display: flex; gap: 10px; align-items: center;">

### MEI

<button onclick="document.getElementById('meiModal').style.display='block'">
  <i class="fas fa-info-circle" title="Clique para mais informações sobre MEI"></i>
</button>

</div>

Vídeo Promocional (em Português)

{{< youtubeLite id="uXs_BRr0ye4" label="Vídeo Demo" >}}


**Tecnologias**: C#, .NET, ASP.NET Core, React.js, React Native, MongoDB, MongoDB Atlas, MongoDB Compass, API RESTful, Swagger, Postman, Visual Studio 2022, VSCode, Rider, Figma, Trello, Git, Github, NUnit, XUnit

- [Demonstração do Site](https://meiameipuc.azurewebsites.net/)

- Login: gg@email.com

- Senha: 12345

> Está hospedado em um servidor gratuito da Azure, então pode demorar um pouco para iniciar.

### Sistema Web 

{{< gallery >}}
  <img src="featured.png"           class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei1.png" class="grid-w500 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei2.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei3.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei4.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei5.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
{{< /gallery >}}

### Aplicativo Móvel

{{< gallery >}}
  <img src="gallery/Mei01.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei02.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei03.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei04.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei05.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
  <img src="gallery/Mei06.png" class="grid-w50 md:grid-w33 xl:grid-w25" />
{{< /gallery >}}


Você pode encontrar mais informações sobre o projeto no `Repositório GitHub`.
{{< github repo="ICEI-PUC-Minas-PMV-ADS/pmv-ads-2024-1-e4-proj-dad-t3-mei" >}}


<!-- O Modal -->
<div id="meiModal" class="modal">
  <div class="modal-content">
    <span class="close" onclick="document.getElementById('meiModal').style.display='none'">&times;</span>
    <h2>
      <i class="fas fa-info-circle" ></i>
      O que é MEI?
      </h2>
      <p>MEI significa Microempreendedor Individual. É um tipo de entidade empresarial no Brasil projetada para pequenos empresários que desejam formalizar suas atividades comerciais. Os MEIs se beneficiam de obrigações fiscais simplificadas e redução da burocracia.</p>
  </div>
</div>
