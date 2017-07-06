# 数组 Array

## 声明数组

```javascript
var skills = ['卖萌', '碎觉', '瞪眼', '三分球', '各种语言的 Hello World'];

var wishes = [7, '🐶', 'iPhone 8', [180, 210, 280], { message: '恭喜你被录用了！' }];

var matrix = [,
  [, 8, 1, 6],
  [, 3, 5, 7],
  [, 4, 9, 2]
];
```

## 数组元素
### 访问数组元素
通过 `[]` 访问数组元素。💡 数组下标从 `0` 开始。
```javascript
> skills[0]
→ "卖萌"

> wishes[1]
→ "🐶"

> wishes[wishes.length - 1]
→ { message: "恭喜你被录用了！" }

> matrix[2][2]
→ 5
```

### 修改数组元素
通过赋值符 `=` 修改数组元素。
```javascript
> skills
→ ["卖萌", "碎觉", "瞪眼", "三分球", "各种语言的 Hello World"]

> skills[2] = '呵呵'
→ "呵呵"

> skills
→ ["卖萌", "碎觉", "呵呵", "三分球", "各种语言的 Hello World"]
```

## 常用方法
`Array.prototype.push()` 方法将一个或多个元素添加到数组末尾，并返回数组的最新长度。
```javascript
> var sx = ['🐭', '🐮', '🐯', '🐰'];
→ undefined

> sx.push('🐲')
→ 5

> sx
→ ["🐭", "🐮", "🐯", "🐰", "🐲"]

> sx.push('🐍', '🐴', '🐑', '🐵', '🐔', '🐶', '🐷');
→ 12

> sx
→ ["🐭", "🐮", "🐯", "🐰", "🐲", "🐍", "🐴", "🐑", "🐵", "🐔", "🐶", "🐷"]
```

## 参考链接
* https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Arrays
* https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/push
