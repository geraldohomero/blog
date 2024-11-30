---
title: "PUC Minas | Mei a Mei"
date: 2024-11-29
draft: false
description: "uma descrição"
tags: [ "featured project", "PUC Minas", "software", "development", "javascript", "mongoDB", "React.js", "React Native" ]
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

Um aplicativo móvel e sistema web projetado para auxiliar empreendedores sob o regime tributário MEI na gestão de suas receitas e na permanência dentro dos limites legais. O objetivo é criar alertas que notifiquem o empreendedor quando estiverem se aproximando do limite de receita da categoria.

<div style="display: flex; gap: 10px; align-items: center;">

### MEI

<button onclick="document.getElementById('meiModal').style.display='block'">
  <i class="fas fa-info-circle" title="Clique para mais informações sobre MEI"></i>
</button>

</div>

{{< alert "star" >}}
**Projeto em Destaque** - Segundo Ano
{{< /alert >}}
>**Primeiro Semestre de 2024**

{{< youtubeLite id="uXs_BRr0ye4" label="Vídeo de Demonstração" >}}


**Tecnologias**: C#, .NET, ASP.NET Core, React.js, React Native, MongoDB, MongoDB Atlas, MongoDB Compass, API RESTful, Swagger, Postman, Visual Studio 2022, VSCode, Rider, Figma, Trello, Git, Github, NUnit, XUnit

- [Demonstração do Website](https://meiameipuc.azurewebsites.net/)

<details style="cursor:pointer" open><summary>Prévia</summary>
  <img src="featured.png" style="border-radius:2%">
</details>

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