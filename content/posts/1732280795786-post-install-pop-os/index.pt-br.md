---
title: "Automatizando a Pós-Instalação no Pop!_OS com Scripts Personalizados"
date: 2024-11-22
draft: false
description: "uma descrição"
---

Configurar um novo sistema operacional pode ser uma tarefa tediosa, especialmente quando se trata de instalar softwares essenciais, configurar o ambiente e configurar aliases para comandos usados com frequência. Para simplificar esse processo, eu criei um conjunto de scripts que automatizam a configuração de pós-instalação do Pop!_OS (22.04 LTS). Neste post, vamos dar uma olhada no projeto e mostrar como usá-lo para configurar seu sistema rapidamente.

[Link para o repositório](https://github.com/geraldohomero/post-install-pop-os)

## Visão Geral do Projeto

O projeto consiste em vários scripts que executam várias tarefas, como instalar pacotes de software, configurar aliases personalizados e configurar o ambiente de desenvolvimento. Os principais scripts são:

- [`run.sh`](run.sh): O ponto de entrada para o processo de pós-instalação.
- [`src/post-install.sh`](src/post-install.sh): Instala pacotes de software e realiza a limpeza do sistema.
- [`src/alias.sh`](src/alias.sh): Configura aliases personalizados.
- [`src/devEnv.sh`](src/devEnv.sh): Instala ferramentas de desenvolvimento como Node.js, .NET SDK e Entity Framework Core.
- [`src/githubClone.sh`](src/githubClone.sh): Clona todos os repositórios de um usuário especificado do GitHub.
- [`src/homeScript.sh`](src/homeScript.sh): Copia scripts utilitários para o diretório home e os torna executáveis.
- [`misc/update.sh`](misc/update.sh): Atualiza e faz upgrade do sistema.
- [`misc/syncthingStatus.sh`](misc/syncthingStatus.sh): Verifica o status do Syncthing.
- [`misc/swapAudio.sh`](misc/swapAudio.sh): Alterna os canais de saída de áudio.

```bash
LICENSE
misc/
    swapAudio.sh
    syncthingStatus.sh
    update.sh
README.md
run.sh
src/
    alias.sh
    devEnv.sh
    githubClone.sh
    homeScript.sh
    post-install.sh
```

## Começando

### Passo 1: Clonar o Repositório

Primeiro, clone o repositório para o local de sua preferência. Neste exemplo, vamos cloná-lo para a pasta `Downloads`:

```bash
git clone https://github.com/geraldohomero/post-install-pop-os.git $HOME/Downloads/post-install-pop-os
```

## Passo 2: Tornar os Scripts Executáveis
Navegue até o repositório clonado e torne os scripts executáveis:
  
  ```bash
  cd $HOME/Downloads/post-install-pop-os
  chmod +x *.sh src/*.sh misc/*.sh
  ```


## Passo 3: Executar o Script de Configuração Pós-Instalação
Execute o script `run.sh` para iniciar o processo de pós-instalação:

O script exibirá mensagens coloridas e informativas à medida que avança pelas etapas de instalação e configuração. Você pode precisar fornecer sua senha para certas operações que exigem privilégios administrativos.

## Passo 4: Siga as Instruções na Tela
O script de configuração irá guiá-lo pelo processo de instalação. Ele irá:

- Executar o script `src/post-install.sh` para instalar pacotes de software e realizar a limpeza do sistema.
- Executar o script `src/alias.sh` para configurar aliases personalizados.
- Copiar scripts utilitários (`update.sh`, `misc/syncthingStatus.sh`, e `misc/swapAudio.sh`) para o diretório home e torná-los executáveis.
- Executar o script `src/devEnv.sh` para instalar ferramentas de desenvolvimento.
- Executar o script `src/githubClone.sh` para clonar todos os repositórios de um usuário especificado do GitHub.

## Passo 5: Personalizar Aliases e Programas Instalados
Você pode modificar ou adicionar seus próprios aliases personalizados no script `src/alias.sh` para se adequar ao seu fluxo de trabalho. Edite o array `CUSTOM_ALIASES` com os aliases desejados e execute o script `src/alias.sh` novamente para atualizar seu arquivo `.bash_aliases`.

## Passo 6: Revisar Software Instalado e Aliases
Após a conclusão da configuração, você pode revisar o software instalado e os aliases no seu sistema. O script `src/post-install.sh` instala pacotes de software listados em sua configuração, enquanto o script `src/alias.sh` configura aliases personalizados.

## Passo 7: Usar Scripts Utilitários
Os scripts utilitários `misc/update.sh`, `misc/syncthingStatus.sh`, e `misc/swapAudio.sh` são copiados para o seu diretório home e tornados executáveis. Você pode usá-los da seguinte forma:

- `update`: Atualiza e faz upgrade do sistema.
- `syncstatus`: Verifica o status do Syncthing.
- `swap`: Alterna os canais de saída de áudio.

## Conclusão
Seguindo esses passos, você pode automatizar a configuração pós-instalação para o Pop!_OS, economizando tempo e garantindo um ambiente consistente em todas as instalações. Sinta-se à vontade para personalizar os scripts para atender às suas necessidades e fluxo de trabalho específicos.