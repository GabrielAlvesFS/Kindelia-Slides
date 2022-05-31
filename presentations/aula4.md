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

# Exercícios de Booleans

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

# Função negação
Inverte o valor recebido

```ts {all}
id(a: Bool): Bool
case a {
  true: Bool.false
  false: Bool.true
  }
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


