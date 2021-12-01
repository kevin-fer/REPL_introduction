# REPL_introduction
TP dans le cadre du cours de Ph. D Pierre Boudes (LIPN) https://gitlab.sorbonne-paris-nord.fr/boudes/cours-fondementsprog-m1
Site pour apprendre un langage X en Y minutes : https://learnxinyminutes.com/
Reminder OCAML sympa : http://philippe.skler.free.fr/commandesocaml.pdf
## A. Tester les REPL, évaluer l'expression mathématique 1+2

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
// Node JS 
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

```scala
// Scala / amm
((x:Int, y:Int) => x + y)
res4: (Int, Int) => Int = ammonite.$sess.cmd4$$$$Lambda..... // Adresse, où la fonc est stockée la fonction dans le Byte code
// Application directement 
((x:Int, y:Int) => x + y)(1,2)
res5: Int = 3
// application après
val f = ((x:Int, y:Int) => x + y)
...
f(1,2)
```
```node
// Node JS
// Application directement
((x, y) => x + y) 
[Function (anonymous)]
((x, y) => x + y) (1,2)
3

// Application après
let add = ((x,y) => x + y)
undefined
add(1,2)
// Application directe et appel de add avec valeur résultat retourné directement
let add = ((x,y) => x + y)(1,2)
undefined
add
3
```
```clojure
; Clojure / lein repl (comme LISP)
; Application directeUse Array.make instead.
((fn [x, y] (+ x y)) 1 2)
3
```
```python
# Python 3.10
((lambda x, y: x + y) (1, 2))
>>>
3
>>>
```

## C. Map en C, créer en C une fonction map qui prend en entrée un pointeur de fonction in(*f)(int) 
## D. Map dans les REPL

```ocaml
(* "OCAML / utop " *) 
(* "Tableau " *) 
let tab = Array.create 10 0;;

Alert deprecated: Stdlib.Array.create
Use Array.make instead.
val tab : int array = [|0; 0; 0; 0; 0; 0; 0; 0; 0; 0|]
(* " Pour accéder à la valeur de la case 0 "*)
tab.(0);;
- : int = 0

```
