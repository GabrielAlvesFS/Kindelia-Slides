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
title: Kindelia Foundation 
---

# Sobre as aulas

Kindelia Foundation 

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Pressione Espaço para passar<carbon:arrow-right class="inline"/>
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

# Índice 

<Toc columns="2" />

---

# O [Kindelia](http://kindelia.org/)
 

 É uma máquina virtual descentralizada equipada com tecnologia blockchain.
 

 Seu objetivo é resolver o [trilema do triângulo de Zooko](https://en.wikipedia.org/wiki/Zooko%27s_triangle): 

![](https://raw.githubusercontent.com/Kindelia/slides/main/img/zooko-dark.png)

- **Eficiente** (Barato e Rápido)  → [HVM](https://github.com/kindelia/hvm): Máquina virtual funcional, paralela e ótima.
- **Segurança**  → [Kind](https://github.com/Kindelia/Kind): Linguagem de programação com provas formais.
- **Descentralizado** → [Kindelia](https://github.com/Kindelia/Kindelia): Computador funcional descentralizado.

<style>
img {
  width: 57%;
  position: relative;
  float: right; 
}
</style>
---


# O que o Kindelia precisa para prevalecer?

- Kindelia: Sob controle nas mãos do Taelin;
- HVM: Newcomers e Turma;
- Kind: Newcomers e Turma;
- Marketing: Grupo primo e comunidade.

Criação de ecossistema:
* Defi: KindCoin, Carteiras, NFTS, Corretoras etc. 
* Jogos diversos.

---

# Objetivo  das aulas

#### Objetivo Geral:
* Que a turma e interessados aprendam a desenvolver em Kind e HVM para contribuir com o ecossistema.

O desafio será aprender sobre linguagens funcionais ao mesmo tempo em que são criadas.

#### Objetivos específicos para a turma:
* Resolver as listas de exercícios.
* Dar feedbacks sobre as aulas para que façamos o melhor conteúdo possível.
* Contribuir com os repositórios [Kind](https://github.com/Kindelia/Kind), 
[Kind2](https://github.com/Kindelia/Kind2), [HVM](https://github.com/kindelia/hvm),
[prelude](https://github.com/Kindelia/prelude),
com a  [Wiki](https://app.gitbook.com/o/f5pmVKXE0zdcMOu6WXHf/s/MAbwOd8IAba3qXSYTi00/)
e com os demais projetos.


---

# Abordagem das aulas
Cada assunto será dividido em duas partes:

### Aula teórica pré-gravada com o conteúdo:

Onde vocês poderão acelerar, pausar, voltar e assistir no momento que preferirem. 

As aulas serão inicialmente direcionadas para a turma, contudo o objetivo é que sirva para qualquer um interessado em aprender por conta própria.

Ao final da aula será passado exercícios.

### Aula síncrona:

Para tirar dúvidas e discutir exercícios.

---

# A equipe

A equipe é formada por: 

* Gabriel
* Humberto
* Jogario
* Corgan
* Rafael

Estaremos nos organizando para entrar em contato com a turma, acompanharmos o desenvolvimento e tirarmos as dúvidas de todos.

--- 

# Objetivo dos Monitores 

* Facilitar o aprendizado da turma (reuniões, links);
* Validar o aprendizado da turma (testes, projetos);
* Criação de conteúdo que facilite o aprendizado de qualquer um interessado (Wiki, youtube);
* Estruturação das informações sobre o Kindelia (Github, redes sociais, site).

---

# Habilidades e conhecimentos pressupostos

* Lógica de programação e Matemática básica;
* Uso de terminal: Comandos básicos, sudo e [WSL](https://docs.microsoft.com/pt-br/windows/wsl/install) se precisar;
* Editor de texto: [VSCode](https://code.visualstudio.com/download), [NeoVim](https://neovim.io/), [Kakoune](http://kakoune.org/) etc.
* Instalação de pacotes: yarn, npm, apt, pacman, brew etc.
* Git e [ssh](https://docs.github.com/en/authentication/connecting-to-github-with-ssh);
* O que é e como funciona o bitcoin e o ethereum.

---

# Cronograma de Aulas (1/3)

## Módulo: Programação Funcional
* Semana 1: Bool, Pair, Maybe, Nat;
* Semana 2: Int, Bits;
* Semana 3: List, Char, string;
* Semana 4: ListMap, BitsMap, PriorityQueue, function;
* Semana 5: Recursion;
* Semana 6: Parsing, TypeClass;
* Semana 7: Monad;
* Semana 8 IO -> projeto final: app;

---

# Cronograma de Aulas (2/3)

## Módulo: Verificação Formal
* Semana 9: Análise de Casos (Bool, Maybe, Pair, Equal);
* Semana 10: Indução Nat;
* Semana 11: Indução Int;
* Semana 12: Indução Bits;
* Semana 13: Tipos dependents;
* Semana 14: Tipos indexados;
* Semana 15: Sigma;
* Semana 16: Prova -> projeto final (1 teorema difícil);

---

# Cronograma de Aulas (3/3)

## Módulo: Lambda Encoding (HVM)
* Semana 17: Lambda Hacks;
* Semana 18: Scott Encoding;
* Semana 19: Church Encoding;
* Semana 20: Self Encoding;

[Lista com mais detalhes](https://gist.githubusercontent.com/VictorTaelin/9470ee286280e5638107fbcfaf7cdc26/raw/4138a5e504e06a557ce212ce29a5491f56640e3a/gistfile1.txt)

---

# Materiais

As aulas ficarão gravadas no [youtube](https://www.youtube.com/c/Kindelia).

Os slides estão disponíveis no repositório [slides](https://github.com/Kindelia/slides).

Os exercícios no repositório [class](https://github.com/Kindelia/class).

Onde é possível acessar o slide online para revisão, e acessar o código fonte dos slides.

Para quem quiser se aprofundar, no repositório do [prelude](https://github.com/Kindelia/prelude) há uma lista com link para referências, incluindo o livro do Okasaki. 

---
layout: center
---

# Exercício

Dar um olhada em:

* [Wiki](https://app.gitbook.com/o/f5pmVKXE0zdcMOu6WXHf/s/MAbwOd8IAba3qXSYTi00/);
* [Class](https://github.com/Kindelia/class);
* [Slides](https://github.com/Kindelia/slides);
* [Youtube](https://www.youtube.com/c/Kindelia).

Se inscrever no canal do youtube, curtir o vídeo, comentar e dar sugestões.
