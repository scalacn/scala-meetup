---
marp: true
theme: uncover
---

# AST Manipulation and Pattern Matching in Scala

---

```
1 + a + 2
-> (1 + a) + 2
-> (a + 1) + 2
-> a + (1 + 2)
-> a + 3
```

---

## Antlr4 in 1 minute
ANTLR (ANother Tool for Language Recognition) is a powerful parser generator for reading, processing, executing, or translating structured text or binary files.

---

## Antlr4: A Parser Generator
```
expression
   :  expression  POW expression
   |  expression  (TIMES | DIV)  expression
   |  expression  (PLUS | MINUS) expression
   |  LPAREN expression RPAREN
   |  (PLUS | MINUS)* atom;

atom
   : scientific
   | variable;

scientific
   : SCIENTIFIC_NUMBER;

variable
   : VARIABLE;
```

---

## Antlr4: Tree of `1 + a + 2`

``` scala
val lazyTree = LazyTree("1 + a + 2")

lazyTree.expression().foreach { node =>
  println(s"${beautifyName(node)} [${extract(node)}]")
}
```

---

## AST Manipulations

---

## Constraints
Only LPAREN/RPAREN/PLUS/atom is allowed.

---

## Parenthesize

```
1 + a + 2
-> (1 + a) + 2
```


---

## Evaluate
```
a + (1 + 2)
-> a + 3
```

---

## Constant Folding

``` sql
select 1 + a + 2 as x from tbl

select a + 3 as x  from tbl
```

---

## DSL
1. Antlr4
2. Pattern Matching
3. Create a DSL

## SQL
### Data Query Language
### Data Manipulation Language

---

## Q&A Notes
### Spark SQL / MySQL

load mysql as mysql_x select * from x;

select * from mysql_x join y

---

## Q&A Notes

text -> AST(antlr4)
-> AST (More Abstraction)

sql -> AST -> LogicalPlan -> PhysicalPlan

---

## Q&A
