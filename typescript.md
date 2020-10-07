

型安全
======

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
```
