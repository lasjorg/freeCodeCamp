---
id: ab306dbdcc907c7ddfc30830
title: 数组扁平化
challengeType: 5
forumTopicId: 16079
---

# --description--

在这道题目中，我们需要写一个数组扁平化的函数。请注意考虑多层数组嵌套的情景。

# --hints--

`steamrollArray([[["a"]], [["b"]]])` 应返回 `["a", "b"]`。

```js
assert.deepEqual(steamrollArray([[['a']], [['b']]]), ['a', 'b']);
```

`steamrollArray([1, [2], [3, [[4]]]])` 应返回 `[1, 2, 3, 4]`。

```js
assert.deepEqual(steamrollArray([1, [2], [3, [[4]]]]), [1, 2, 3, 4]);
```

`steamrollArray([1, [], [3, [[4]]]])` 应返回 `[1, 3, 4]`。

```js
assert.deepEqual(steamrollArray([1, [], [3, [[4]]]]), [1, 3, 4]);
```

`steamrollArray([1, {}, [3, [[4]]]])` 应返回 `[1, {}, 3, 4]`。

```js
assert.deepEqual(steamrollArray([1, {}, [3, [[4]]]]), [1, {}, 3, 4]);
```

代码中不应使用 `Array.prototype.flat()` 或 `Array.prototype.flatMap()` 方法。

```js
assert(!code.match(/\.\s*flat\s*\(/) && !code.match(/\.\s*flatMap\s*\(/));
```

# --solutions--

