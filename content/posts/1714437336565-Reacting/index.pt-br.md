---
title: "Reacting - Reajamento - Reação - Reagiabilidade"
date: 2024-04-30
draft: false
description: "uma descrição"
tags: [reaja, estudo, javascript]
---
**Minha jornada com React.js e outras tecnologias relacionadas**

{{< github repo="geraldohomero/reacting" >}}

## Reação
Primeiramente, comecei a aprender React.js, uma biblioteca JavaScript para construir interfaces de usuário. Segui a documentação oficial, alguns tutoriais no YouTube e o curso da O'Reilly. Aprendi sobre componentes, props, estado e hooks. Também aprendi sobre o React Router, uma biblioteca para roteamento em aplicações React. 

>Vem comigo que o bagulho vai ser doido!

## Reajamento

Como funcionam os componentes em React? 

### Componentes Funcionais
Os componentes funcionais são funções JavaScript que aceitam props e retornam elementos React. Eles são mais simples de escrever e mais fáceis de entender do que os componentes de classe. 

```jsx
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}
```
>Esse componente aceita uma propriedade `name` e exibe "Hello, [name]".

### Componentes de Classe

Os componentes de classe são uma maneira de definir componentes usando classes JavaScript. Eles têm um estado e um ciclo de vida. 

```jsx
class Welcome extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}</h1>;
  }
}
```
>Esse componente também aceita uma propriedade `name` e exibe "Hello, [name]", mas é definido como uma `classe`.


