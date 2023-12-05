# Ferramenta de modelagem de software para ensino de programação com Design Patterns

Este é o trabalho de conclusão de curso de engenharia de computação da Escola Politécnica da USP feito por:

- André Hideki Gashu Nishimura
- William Abe Fukushima

E orientado pelo Prof. Dr. Jorge Luis Risco Becerra.

Os códigos fonte do frontend e do backend da aplicação podem ser acessados nos links a seguir:
- Frontend: https://github.com/AndreHGN/TCC-front
- Backend: https://github.com/williamfukushima/TCC-Backend

A aplicação em si está disponível para ser usada neste endereço:
https://andrehgn.github.io/TCC-front

# Introdução

Em desenvolvimento de software é comum a utilização de Design Patterns durante as fases de programação e refatoração. Alguns desafios associados ao aprendizado e ensino desses conceitos, são a elevada abstração e dificuldade na escolha do padrão adequado para um contexto específico. Uma maneira de melhorar este problema é pela introdução gradual aos estudantes de exemplos e exercícios práticos, desde aplicações mais simples até as mais complexas.

**Objetivo:** Desenvolver uma ferramenta que utiliza diagramas UML para gerar de códigos de design patterns, focando em projetos educativos e de pequeno porte para sistemas web e aproximando o estudo teórico da prática.

# Metodologia

A base teórica do projeto é a metodologia da Ciência do Design. Esta abordagem é frequentemente adotada em disciplinas onde a ação prática e a criação de soluções concretas são centrais para o processo de pesquisa como projetos de engenharia, design e ciência da computação.

![image](https://github.com/AndreHGN/tcc-poliusp-modelagem-design-patterns/assets/80173402/0864d857-b8df-47e6-9513-94490700f21b)

# Arquitetura

A arquitetura elaborada para o projeto segue como base o modelo cliente-servidor. O cliente consiste de um editor de diagramas que possibilita a modelagem em UML e que codifica a informação em JSON para transmissão via Web. Recebendo o dado, o servidor o decodifica para gerar os arquivos de códigos a partir de um gerador de código fonte.

![image](https://github.com/AndreHGN/tcc-poliusp-modelagem-design-patterns/assets/80173402/c0db9cef-967f-417a-9dd4-1e29245a7667)

# Resultados

O software foi desenvolvido com sucesso e abrange os principais requisitos levantados, incluindo: modelagem de diagramas UML, associação a conceitos de design patterns e geração de templates de código. A imagem mostra a tela final da interface com um diagrama modelado, enquanto os trechos de códigos abaixo são algumas das classes geradas.

![image](https://github.com/AndreHGN/tcc-poliusp-modelagem-design-patterns/assets/80173402/d427920f-8b84-423f-8c68-c1bf54a1bad1)

```javascript
export class Subscriber {
    //#region Attributes
    //#endregion

    constructor() {
    }
    
    //#region Methods
    public update(){
      # Implement This Method
    };
    //#endregion
  }
```

```javascript
export class DigitSubscriber {
    //#region Attributes
    //#endregion

    constructor() {
    }
    
    //#region Methods
    public update(changedSubject : Subject) : void{
      # Implement This Method
    };
    //#endregion
  }
```

```javascript
export class Subject {
    //#region Attributes
    //#endregion

    constructor() {
    }
    
    //#region Methods
    public subscribe(subscriber){
      # Implement This Method
    };
    public unsubscribe(subscriber){
      # Implement This Method
    };
    public notify(){
      # Implement This Method
    };
    //#endregion
  }
```

# Conclusões

Como prova de conceito, foi desenvolvido uma pequena aplicação utilizando os códigos gerados pelo sistema através do padrão Strategy, consistindo em um jogo de pedra, papel e tesoura com duas possíveis estratégias. Com isso, pode-se validar o uso desta ferramenta para implementar projetos de software simples a partir dos modelos elaborados com design patterns. Assim, o usuário poderá relacionar mais facilmente a motivação e o uso desses padrões com a implementação prática.

