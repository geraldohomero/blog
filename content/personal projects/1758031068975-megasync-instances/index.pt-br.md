---
title: "Gerenciador de Múltiplas Instâncias do MEGASync"
date: 2025-09-16
draft: false
description: "Um script independente de distribuição para gerenciar múltiplas instâncias do MEGASync para diferentes contas MEGA."
tags: ["megasync", "linux", "bash", "script", "projetos pessoais"]
---

Um script independente de distribuição para gerenciar múltiplas instâncias do MEGASync para diferentes contas MEGA.

![Gerenciador de Múltiplas Instâncias do MEGASync](featured.png)

## Funcionalidades
- Funciona no Debian, Ubuntu, Fedora e Arch Linux
- Interface gráfica com Zenity
- Instâncias isoladas com diretórios de configuração separados
- Adição dinâmica de instâncias
- Armazenamento persistente das instâncias

{{< github repo="geraldohomero/megasync-multiple-instances" >}}

## Instalação

Execute este comando para instalar:

```bash
wget -O - https://raw.githubusercontent.com/geraldohomero/megasync-multiple-instances/refs/heads/main/megasync-manager.sh | bash -s install
```

Depois use:

```bash
mega
```

O script detecta sua distribuição e instala as dependências (`megasync`, `zenity`).

## Uso

- Execute `mega` para abrir o gerenciador.
- Selecione instâncias para iniciar ou adicione novas.
- Configure a inicialização automática das instâncias.