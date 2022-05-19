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

# Kindelia University

Booleans

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

<h1 style="text-align: center; margin-bottom: 3rem;">Tipos</h1>


<p style="text-align: center;">
    Tipos são como agrupamos uma série de valores, todos os valores contidos naquele grupo pertencem àquela categoria, ou seja, são do mesmo tipo.
</p>

---

<h1 style="text-align: center; margin-bottom: 3rem;">Construtores</h1>

<p style="text-align: center;">
   Construtores são feitos para guardar algum valor e ao mesmo tempo podem não guardar nenhum valor.
</p>

---

<h1 style="text-align: center; margin-bottom: 3rem;">Nessa primeira aula será apresentado o tipo Bool</h1>

```ts {all|1|1-3|}
                                                            Type Bool {

                                                                true

                                                                false

                                                            }
```

<p style="text-align: center;">True e False são os contrutores do tipo Bool.</p>

<p style="text-align: center;">Construtores como true e false do tipo Bool por si só não possuem nenhum significado, é apenas um nome, somente quando você escreve funções para atribuir esses valores do que é "true" e o que é "falso" para eles, é quando eles irão trabalhar da maneira que queremos que funcione. </p>

---

<h1 style="text-align: center; margin-bottom: 3rem;">Functions</h1>

<p style="text-align: center;">Funções dão vida aos tipos e construtores que criamos.</p>

<h2 style="text-align: center; margin-bottom: 3rem;">Sintaxe e estrutura de uma função em Kind:</h2>

<p style="text-align: center;"> funçao identidade </p>
<p style="text-align: center;"> f(x) = x  </p>
<p style="text-align: center;"> identity (a: Bool): Bool </p>


---

<h1 style="text-align: center; margin-bottom: 3rem;">Functions na prática</h1>

```ts {all|1|1-3|}
                                                        id(a:Bool): Bool

                                                            case a{

                                                                true: Bool.true

                                                                false: Bool.false

                                                            }

```

<h5 style="text-align: center;">obs: utilizamos a sintaxe da seguinte forma:</h5>
<p style="text-align: center;"> Tipo.construtor -> Bool.true </p>

---

<h1 style="text-align: center; margin-bottom: 3rem;">Type Checker</h1>

<h4 style="text-align: center;"> para realizar o type check de um arquivo Kind basta rodar o comando no terminal: </h4>

```ts {}

                                                       kind "nome_do_arquivo".kind

```

<p style="text-align: center; font-size: 13px;"> retornando -> all therms checks</p>
<p style="text-align: center; font-size: 13px;"> significa que a sintaxe e os types estão corretos.</p>

<h4 style="text-align: center;"> Logo após você pode rodar o arquivo com: </h4>

```ts {}

                                                       kind "nome_do_arquivo" --run

```

---

<h1 style="text-align: center; margin-bottom: 3rem;">Função que recebe dois parâmetros</h1>

<p style="text-align: center;"> Aqui vemos um exemplo: </p>

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

<p style="text-align: center;"> Essa função tem o intuito de retornar ‘true’ caso alguma das entradas seja ‘true’. </p>