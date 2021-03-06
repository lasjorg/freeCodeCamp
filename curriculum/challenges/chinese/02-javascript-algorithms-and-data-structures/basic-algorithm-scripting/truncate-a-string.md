---
id: ac6993d51946422351508a41
title: 截断字符串
challengeType: 5
forumTopicId: 16089
---

# --description--

如果传入的字符串（第一个参数）的长度大于传入的值（第二个参数），请在这个位置截断它并在后面加上 `...`，然后返回结果。

# --hints--

`truncateString("A-tisket a-tasket A green and yellow basket", 8)` 应返回 "A-tisket..."。

```js
assert(
  truncateString('A-tisket a-tasket A green and yellow basket', 8) ===
    'A-tisket...'
);
```

`truncateString("Peter Piper picked a peck of pickled peppers", 11)` 应返回 "Peter Piper..."。

```js
assert(
  truncateString('Peter Piper picked a peck of pickled peppers', 11) ===
    'Peter Piper...'
);
```

`truncateString("A-tisket a-tasket A green and yellow basket", "A-tisket a-tasket A green and yellow basket".length)` 应返回 "A-tisket a-tasket A green and yellow basket"。

```js
assert(
  truncateString(
    'A-tisket a-tasket A green and yellow basket',
    'A-tisket a-tasket A green and yellow basket'.length
  ) === 'A-tisket a-tasket A green and yellow basket'
);
```

`truncateString("A-tisket a-tasket A green and yellow basket", "A-tisket a-tasket A green and yellow basket".length + 2)` 应返回 "A-tisket a-tasket A green and yellow basket"。

```js
assert(
  truncateString(
    'A-tisket a-tasket A green and yellow basket',
    'A-tisket a-tasket A green and yellow basket'.length + 2
  ) === 'A-tisket a-tasket A green and yellow basket'
);
```

`truncateString("A-", 1)` 应返回 "A..."。

```js
assert(truncateString('A-', 1) === 'A...');
```

`truncateString("Absolutely Longer", 2)` 应返回 "Ab..."。

```js
assert(truncateString('Absolutely Longer', 2) === 'Ab...');
```

# --solutions--

