#### Scala Fundamentals - Part 1

---

[cass@metalgear ~]$ `scala`
```
Welcome to Scala version 2.11.7 (Java HotSpot(TM) 64-Bit Server VM, Java 1.8.0_72).
Type in expressions to have them evaluated.
Type :help for more information.
```

---

scala> `println("Welcome to Scala Fundamentals")`
`Welcome to Scala Fundamentals`

scala> `println("Scala can automatically \n declare variables and handle their datatypes ...")`
```
Scala can automatically
 declare variables and handle their datatypes ...
```

---

##### Scala can automatically declare variables and handle their datatypes

scala> `"hello world"`
`res2: String = hello world`

scala> `res2`
`res3: String = hello world`

scala> `10`
`res4: Int = 10`

scala> `10.2`
`res5: Double = 10.2`

scala> `10+20`
`res6: Int = 30`

scala> `10+20.2`
`res7: Double = 30.2`

scala> `"hello " + "world !"`
`res8: String = hello world !`

---

##### Variables & Immutable Values

scala> `var x = "hello world"`
`x: String = hello world`

scala> `x = x + ". we love scala."`
`x: String = hello world. we love scala.`

##### variables (var) can be modified

scala> `val y = "hello world"`
`y: String = hello world`

scala> `y = y + ". we love scala."`
```
<console>:11: error: reassignment to val
       y = y + ". we love scala."
         ^
```

##### immutable values (val) cannot be modified

scala> `y = "hello world" + ". we love scala."`
```
<console>:11: error: reassignment to val
       y = "hello world" + ". we love scala."
         ^
```

scala> `val y = "hello world" + ". we love scala."`
`y: String = hello world. we love scala.`

##### redeclared val y ...

---

##### for loop

scala> `for(i <- 1 to 5) println(i)`
```
1
2
3
4
5
```

##### automatic variable declaration ... automatic increments ...

---

scala> `var numList = for(i <- 1 to 5) yield i`
`numList: scala.collection.immutable.IndexedSeq[Int] = Vector(1, 2, 3, 4, 5)`

scala> `numList.foreach(i => println(i))`
```
1
2
3
4
5
```

scala> `val y = "Hello World"`
`y: String = Hello World`

scala> `y.foreach(c => println(c))`
```
H
e
l
l
o

W
o
r
l
d
```

##### c => println(c) can be changed to println(_)

scala> `y.foreach(println(_))`
```
H
e
l
l
o

W
o
r
l
d
```

##### println(_) can be simplified as println

scala> `y.foreach(println)`
```
H
e
l
l
o

W
o
r
l
d
```

---

scala> `println("thats it for basic Scala introduction ...")`
scala> `println("for more info, please visit http://www.scala-lang.org/ ")`

scala> `:quit`

[cass@metalgear ~]$

---
