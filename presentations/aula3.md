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
---

# Booleans

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

# Tipos

    Tipos são como agrupamos uma série de valores, todos os valores contidos naquele grupo pertencem àquela categoria, ou seja, são do mesmo tipo.

---

# Construtores

   Construtores são feitos para guardar algum valor e ao mesmo tempo podem não guardar nenhum valor.

---

# Nessa primeira aula será apresentado o tipo Bool

```ts {all|1|1-3|}
Type Bool {

    true

    false

}
```

True e False são os contrutores do tipo Bool.

Construtores como true e false do tipo Bool por si só não possuem nenhum significado, é apenas um nome, somente quando você escreve funções para atribuir esses valores do que é "true" e o que é "falso" para eles, é quando eles irão trabalhar da maneira que queremos que funcione.

---

# Functions

Funções dão vida aos tipos e construtores que criamos.

## Sintaxe e estrutura de uma função em Kind:

 funçao identidade
 f(x) = x  
 identity (a: Bool): Bool


---

# Functions na prática

```ts {all|1|1-3|}
id(a:Bool): Bool

    case a{

        true: Bool.true

        false: Bool.false

    }

```

##### obs: utilizamos a sintaxe da seguinte forma:
 Tipo.construtor -> Bool.true 

---

# Type Checker

#### para realizar o type check de um arquivo Kind basta rodar o comando no terminal: 

```ts {}

kind "nome_do_arquivo".kind

```

 retornando -> all therms checks
 significa que a sintaxe e os types estão corretos.

#### Logo após você pode rodar o arquivo com: 

```ts {}

kind "nome_do_arquivo" --run

```

---

# Função que recebe dois parâmetros

 Aqui vemos um exemplo: 

```ts {all|2-9|3-8|3-6|4-5|8|all}
or(a: Bool, b: Bool): Bool
    case a{ 
        false: case b {
                true: Bool.true
                false: Bool.false
            }

        true: Bool.true
    }

```

 Essa função tem o intuito de retornar ‘true’ caso alguma das entradas seja ‘true’.
