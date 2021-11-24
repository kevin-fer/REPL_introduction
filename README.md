# REPL_introduction

## A. Tester les REPL, évaluer l'expression mathémrique 1+2

```ocaml
(* "OCAML / utop " *) 
1 + 2;;
- : int = 3
```
```scala
// Scala / amm
1 + 2
res1 : Int = 3
```
```node
// Clojure 
1 + 2
>
3
>
```
```clojure
; Clojure / lein repl 
(+ 1 2)
3
```
```python
# Python 3.10
1 + 2 
>>>
3
>>>
```
## B. Lambda-expressions 


```ocaml
(* "OCAML / utop " *) 
(* "Déclaration puis appel de la fonction" *) 
let my_lambda_expression = fun (x,y) -> x + y;;
my_lambda_expression(1,2);;
- : int = 3

(* "Application directement" *) 
(fun (x,y) -> x + y) (1,2);;
- int = 3
```

