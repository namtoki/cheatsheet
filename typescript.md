
Union Types
===========



型安全 (Guards)
===============

typeof type guards
------------------

```TypeScript
if (typeof value === 'number') {
    return 0
}
```

in type guards
--------------

```TypeScript
type Hoge = { foo: string }
type HogeA = Hoge & { bar: string }
type HogeB = Hoge & { aaaa: number; bbbb: string }

function fc(hoge: HogeA | HogeB) {
  if ('foo' in hoge) {
    // hoge: HogeA | HogeB
  }
  if ('bar' in hoge) {
    // hoge: HogeA
    return
  }
  // hoge: HogeB
}
```

instanceof type guards
----------------------

```TypeScript
class A {
    // ...
}
class B extends A {
    // ...
}
class C extends A {
    // ...
}

function fc(alph: A | B | C) {
  if (alph instanceof B) {
    // alph: B
  }
  // alph: A | C
  if (alph instanceof C) {
    // alph: C
  }
  // alph: A
}
```

Tagged union
------------

```TypeScript
type A = { name: 'A'; a: string }
type B = { name: 'B'; b: number }
type C = { name: 'C'; c: string }

function fc(alph: A | B | C) {
  switch(alph.name) {
    case 'A':
      // alph: A
      return
    case 'B':
      // alph: B
      return
    case 'C':
      // alph: C
      return
    default:
      // alph: never
      return
  }
}
```
