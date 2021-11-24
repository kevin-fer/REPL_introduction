# REPL_introduction

best site clairement : https://learnxinyminutes.com/

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
(+ 1 2)https://learnxinyminutes.com/
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

```scala
// Scala / amm
((x:Int, y:Int) => x + y)
res4: (Int, Int) => Int = ammonite.$sess.cmd4$$$$Lambda..... // Adresse où est stockée la fonction dans le Byte code
// Application directement 
((x:Int, y:Int) => x + y)(1,2)
res5: Int = 3
// application après
val f = ((x:Int, y:Int) => x + y)
...
f(1,2)
```

