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

# Tipo Maybe

```ts {all|1|1-3|}
type Maybe{

    none

    some(value: type)      → O construtor some guarda um valor de algum tipo.

}
```

None e Some são os contrutores do tipo Bool. 

```ts {all|1|1-3|}
                 case algo
               /           \
           none           some(value)
            |                |
           xxx              algo.value  
```

---

# Tipo MaybeBool

```ts {all|1|1-3|}
type MaybeBool{

    none

    some(value: Bool)      → O contrutor SOME guarda um valor, que nesse caso é do tipo Bool.

}

Obs: tipo.construtor → MaybeBool.some(Bool.false)
```

# Exemplo:
```ts {all|3|4-6|5-6|1-9}
//Returns true if Maybe is none

is_none(a: MaybeBool): Bool
	 case a {
		 none: Bool.true
		 some: Bool.false
}
//is_none(MaybeBool.none)
//return: true
```

---

# Tipo Pair

```ts {all|1|3|1-5 }
type Pair{

	new (pair.fst , pair.snd)
   
}
```

O tipo Pair possui apenas um construtor.
Esse construtor recebe dois valores. Um par de algum tipo.


---

# Tipo PairBool

```ts {all|1|3|1-5 }
type PairBool{

	new (fst: Bool, snd: Bool)
   
}
```
O contrutor NEW guarda um par de valores, que nesse caso são do tipo Bool.

# Exemplo:

```ts {all|2|3|3-4|5-6|7-8|2-9|all}
// Returns true if both elements of a PairBool are identical
eql_elements(a: PairBool): Bool 
  case a{
    new: case a.fst{
		      true: a.snd
		      false: case a.snd{
		              true: Bool.false
		              false: Bool.true
      }}}

//eql_elements(PairBool.new(Bool.true , Bool.true))
//return: true
```