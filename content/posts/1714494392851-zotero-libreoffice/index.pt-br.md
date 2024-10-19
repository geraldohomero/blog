---
title: "Integração Zotero + LibreOffice (Linux/Ubuntu)"
date: 2022-04-13
draft: false
type: "tech"
description: "uma descrição"
tags: ["foss", "zotero", "libreoffice", "linux", "ubuntu", "solução de problemas", "plugin"]
---


Zotero + LibreOffice (distribuições baseadas em Linux/Ubuntu) - Créditos para: [Kameid](https://www.reddit.com/r/linux4noobs/comments/i6skza/installing_zotero_and_using_it_with_libreoffice/)

Tentando resolver o problema em que o plugin Zotero não funciona corretamente no LibreOffice Writer do Linux:

## Guia:

### **1. Desinstale o Zotero**

### **2. Verifique se você tem um Ambiente de Execução Java instalado**. 

No LibreOffice, vá em **Ferramentas>Opções>Avançado**. Verifique se a caixa "Usar um JRE" está marcada e se há um JRE instalado. **Se não houver**, abra o terminal e **instale o JRE mais recente**: 

`sudo apt install openjdk-8-jre`

![image](https://user-images.githubusercontent.com/70844369/175447639-41eaf455-1615-4306-9fc3-a8a9300403fa.png#vitrinedev)

### **3. Verifique se a instalação funcionou. Execute o comando:**

`java -version` 

Saída:

![image](https://user-images.githubusercontent.com/70844369/175448591-d2b9d844-aa40-4bb2-a8a8-e4ed587b08a9.png)

### **4. Reinicie o LibreOffice**

### **5. Instale o pacote libreoffice-java-common:**

`sudo apt install libreoffice-java-common`

### **6. Instale o Zotero**

>Agora deve funcionar corretamente

![image](https://user-images.githubusercontent.com/70844369/175447878-09b925d0-8e78-493c-8878-3da98fe551af.png)

Créditos para [Kameid](https://www.reddit.com/r/linux4noobs/comments/i6skza/installing_zotero_and_using_it_with_libreoffice/)

[Post do Zotero](https://www.zotero.org/support/word_processor_plugin_troubleshooting) sobre o processo de solução de problemas do plugin do LibreOffice.

***

## **Bônus caso não tenha funcionado**

1. Navegue até os arquivos do aplicativo Zotero:
   - Vá para o diretório onde o Zotero está instalado e abra `extensions/zoteroOpenOfficeIntegration@zotero.org/install` (Zotero 6) ou `integration/libreoffice` (Zotero 7)
       - Caso use Flatpak: `~/.local/share/flatpak/app/org.zotero.Zotero/x86_64/stable/.../files/share/zotero/extensions/zoteroOpenOfficeIntegration@zotero.org/install`

  - Ou procure por `Zotero_OpenOffice_Integration.oxt` no seu gerenciador de arquivos (Nautilus, Dolphin...)
  
   ![image](https://github.com/geraldohomero/Zotero-LibreOffice-Linux/assets/70844369/e962db11-271d-4091-ba88-81692de66710)

2. Dê um duplo clique no arquivo Zotero_OpenOffice_Integration.oxt para instalá-lo. Ou, vá em Ferramentas → Gerenciador de Extensões no LibreOffice, clique em Adicionar e selecione o .oxt da pasta acima.

[Post no site do Zotero](https://www.zotero.org/support/word_processor_plugin_manual_installation)