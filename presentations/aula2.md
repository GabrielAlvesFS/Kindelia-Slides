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
 
Kindelia University 


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

# O que irá aprender nesta aula

<Toc columns="1" />

---

# Objetivo com o Kind
A linguagem Kind deve ser extremamente:

* ##  **Eficiente**. 

 Ou seja, **rápida** e com baixo custo de **processamento**.

* ## **Confiável**. 

Não deve haver falhas de segurança.

---


# Por que programação funcional?
A propriedade da **imutabilidade** nas **funções puras**.

Cada entrada de função resulta sempre numa mesma saída. E evita-se ao máximo guardar estados.

Tornando-a em relação a programação **imperativa**, mais:
* **Eficiente**: Pois facilita o **processamento em paralelo** e a **reutilização de funções** sem reprocessamento. 
* **Confiável**: Pode-se usar de **provas formais**, onde prova-se matematicamente que um código comporta-se como esperado. O código final costuma ser  mais simples e legível.

---

# O que é programação funcional?
É um **paradigma de programação** que se baseia na **composição de funções**.

Utiliza-se da **recursão**.

Possui 2 características muito úteis:
* **Lazy Evaluation**: Permite criar listas infinitas, o compilador se encarrega de calcular apenas o que será utilizado.
* Função de alta ordem (**lambdas**): Recebe ou retorna outras funções.

---

# Exemplo: A função fatorial
Definição matemática do fatorial.

Definição pelo **produto**:

$$ n! = \prod_{k=1}^{n} k $$

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
Linguagem de programação **imperativa**.

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
Linguagem de programação **funcional**.

```haskell
fact 0 = 1
fact n = n *fact (n-1)
```

---

# Lista de linguagens de programação funcional

* [Haskell](https://www.haskell.org/).
* [Lua](https://www.lua.org/).
* [Rust](https://www.rust-lang.org/).
* [Elixir](https://elixir-lang.org/).
* [Javascript](https://developer.mozilla.org/en-US/docs/Web/JavaScript) (*dependendo do uso*).

---

# Por que o Kind?
O que falta nas linguagens de programação funcionais atuais?

* ### **Lazy evaluation** em funções.
Tornando o paralelismo extremamente mais **eficiente**.

* ### **Provas formais** nativa.
Tornando o sistema ultra seguro sem aumentar o custo de processamento.
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
Na [teoria dos tipos](https://en.wikipedia.org/wiki/Type_theory) tudo possui um "tipo" (***type*** em ingês)

* ***1*** é do tipo ***nat***; ***True*** é do tipo ***bool***.
* ***Nat*** e ***bool*** são do tipo [**type**](https://en.wikipedia.org/wiki/Type_constructor).
* ***Type*** é do tipo [***kind***](https://en.wikipedia.org/wiki/Kind_(type_theory)).

***Kind*** é o tipo de mais alta ordem, dele que surge a palavra **Kindelia**.
---

# Exercício

* ### Instalar o kind.

