---
type: doc
layout: reference
category: "Syntax"
title: "委譲"
---

<!--original
---
type: doc
layout: reference
category: "Syntax"
title: "Delegation"
---
-->

# 委譲 (Delegation)

<!--original
# Delegation
-->

## クラスの委譲

<!--original
## Class Delegation
-->

[Delegationパターン](https://en.wikipedia.org/wiki/Delegation_pattern)は、実装継承の良い代替手段であることが証明されており、Kotlinはネイティブでそれをサポートし、かつ定型コードを必要としません。
`Derivced` クラスは、 `Base` インターフェイスから継承することができ、指定されたオブジェクトへの public メソッドのすべてを委譲することができます。

<!--original
The [Delegation pattern](https://en.wikipedia.org/wiki/Delegation_pattern) has proven to be a good alternative to implementation inheritance,
and Kotlin supports it natively requiring zero boilerplate code.
A class `Derived` can inherit from an interface `Base` and delegate all of its public methods to a specified object:
-->

``` kotlin
interface Base {
  fun print()
}

class BaseImpl(val x: Int) : Base {
  override fun print() { print(x) }
}

class Derived(b: Base) : Base by b

fun main(args: Array<String>) {
  val b = BaseImpl(10)
  Derived(b).print() // 出力：10
}
```

<!--original
``` kotlin
interface Base {
  fun print()
}

class BaseImpl(val x: Int) : Base {
  override fun print() { print(x) }
}

class Derived(b: Base) : Base by b

fun main(args: Array<String>) {
  val b = BaseImpl(10)
  Derived(b).print() // prints 10
}
```
-->

`Derived` のスーパータイプのリスト中の *by*{:.keyword} 節は、 `b` が `Derived` のオブジェクトに内部的に格納されることを示し、コンパイラは `b` に取り次ぐ `Base` のすべてのメソッドを生成します。

<!--original
The *by*{: .keyword }-clause in the supertype list for `Derived` indicates that `b` will be stored internally in objects of `Derived`
and the compiler will generate all the methods of `Base` that forward to `b`.

-->

<script src="http://code.jquery.com/jquery-1.11.0.min.js"></script>
<script>
$(function() {
  $("*").contents().filter(function() {
    return this.nodeType==8 && this.nodeValue.match(/^original/);
  }).each(function(i, e) {
    var tooltips = e.nodeValue.replace(/^original *[\n\r]|[\n\r]$/g, '');
    $(this).prev().attr('title', tooltips);
  });
});
</script>
