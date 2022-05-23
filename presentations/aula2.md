---
theme: seriph
background: https://source.unsplash.com/collection/94734566/1920x1080
class: text-center
highlighter: shiki
lineNumbers: false
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
drawings:
  persist: false
title: Kindelia University
hideInToc: true
---


# Introdução ao Kind
 
Kindelia Foundation 


<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Pressione Espaço para passar
     <carbon:arrow-right class="inline"/>
  </span>
</div>

<div class="abs-br m-6 flex gap-2">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:edit />
  </button>
  <a href="https://github.com/Kindelia/slides" target="_blank" alt="GitHub"
    class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div>

---
hideInToc: true
---

# O que será ensinado nesta aula

<Toc columns="1" />

---

# Objetivo do Kind
A linguagem Kind deve possuir:

* ## **Provas formais** nativas 

Com baixo custo de processamento

* ## **Sintaxe Simples**
Que facilite o entendimento e criação de aplicações

* ## **Código fonte enxuto**
Para clara legibilidade e manutenção do código


---

# Por que programação funcional?
A propriedade da **imutabilidade** nas **funções puras**

Cada entrada de função resulta sempre numa mesma saída, assim, evita-se ao máximo guardar estados.

Tornando-a em relação a programação **imperativa**, mais:
* **Eficiente** em grandes projetos: Pois facilita o **processamento em paralelo** e a **reutilização de funções** sem reprocessamento;
* **Confiável**: Pode-se usar de **provas formais**, onde prova-se matematicamente que um código comporta-se como esperado. O código final também costuma ser  mais simples e legível.

---

# O que é programação funcional?
É um **paradigma de programação** que se baseia na **composição de funções**

Possui 3 características muito úteis:
* **Recursão**;
* **Lazy Evaluation**: Atrasa a computação até que seja realmente necessário;
* Função de alta ordem (**lambdas**): Recebe ou retorna outras funções.

---

# Exemplo: A função fatorial
Definição matemática do fatorial

Definição pelo **produto**:

$$ n! = 1\cdot 2\cdot 3\cdot ... \cdot(n-2)\cdot(n-1) \cdot n = \prod_{k=1}^{n} k $$


Definição por **recorrência**:

$$ 
  n!=\begin{cases}
    1, & \text{if $n=0$},\\
    (n-1)! \cdot n, & \text{if $n \gt 0$}.
  \end{cases}
$$



---
layout: two-cols
hideInToc: true
---

# C
Linguagem de programação **imperativa**

```c
int factorial (int n){
  int i, r;
  i=1;
  r=1;
  while (i<=n){
    r=r*i;
    i=i+1;
  }
  return r
}
```

::right::

# Haskell
<!-- colocar em kind -->
Linguagem de programação **funcional**

```haskell
fact 0 = 1
fact n = n *fact (n-1)
```

---

# Exemplos de linguagens de programação funcional


### Puras:
* [Haskell](https://www.haskell.org/)
* [PureScript](https://www.purescript.org/)
* [Elm](https://elm-lang.org/)
* [Kind](https://github.com/Kindelia/Kind)

Não-puras (orientadas a PF): 
[MLs](https://en.wikipedia.org/wiki/ML_(programming_language)), 
[Lisps](https://lisp-lang.org/), 
[Elixir](https://elixir-lang.org/), 
[Scala](https://www.scala-lang.org/) etc.

Outras (multiparadigmas): 
[Javascript](https://developer.mozilla.org/en-US/docs/Web/JavaScript), 
[Python](https://www.python.org/), [Lua](https://www.lua.org/) etc.

---

# O que falta nas linguagens de programação funcionais atuais?
Por que criar o kind?

Não há nenhuma nenhuma linguagem de programação funcional atualmente que possua todos os requisitos do **kind**,
e todos são indispensáveis, pois:

* **Provas formais** nativas: 
Permitirá que seja provado que o código criado esteja correto, porém não pode aumentar muito o custo de processamento da aplicação;

* **Sintaxe Simples**: 
A linguagem precisa ser acessível, para que não fique restrita a meios acadêmicos;

*  **Código fonte enxuto**:
É necessário para a confiabilidade do código, e permite que seja estendido de acordo com a necessidade.

---

# Como instalar o Kind

```bash
sudo npm i -g kind-lang
```

ou

```bash
sudo yarn global add kind-lang
```


---

# Origem do nome Kindelia
<!-- talvez tirar slide -->
Curiosidade

Na [teoria dos tipos](https://en.wikipedia.org/wiki/Type_theory) tudo possui um "tipo" (***type*** em ingês):

* ***1*** é do tipo ***nat***; ***True*** é do tipo ***bool***;
* ***Nat*** e ***bool*** são do tipo [**type**](https://en.wikipedia.org/wiki/Type_constructor);
* ***Type*** é do tipo [***kind***](https://en.wikipedia.org/wiki/Kind_(type_theory)).

***Kind*** é o tipo de mais alta ordem, dele que surge a palavra **Kindelia**.
---

# Exercício

* ### Instalar o kind.

