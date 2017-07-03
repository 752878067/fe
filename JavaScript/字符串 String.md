# 字符串 String

JavaScript 通过字符串存储文本。字符串的内部格式是 [UTF-16](https://en.wikipedia.org/wiki/UTF-16)，与文档格式无关。

## 声明字符串
字符串可以用一对双引号 `"` 或者单引号 `'` 括起来。
```javascript
"但愿人长久，千里共婵娟。"

'其实我是一个演员。'

"I'm fine, thank you, and you?"  // 如果文本内容包含单引号，那就用 "" 括起来，反之亦然。

// 如果文本内容既有单引号又有双引号，那你需要在其中一种前面加 \ 进行转义。

"老师说，JavaScript 字符串用单引号 ' 或者双引号 \" 括住都行，那我应该用单引号还是双引号呢？"
'老师说，JavaScript 字符串用单引号 \' 或者双引号 " 括住都行，那我应该用单引号还是双引号呢？'
```

### Backtick 字符串
`ES6`  

字符串还可以用一对反引号 `` 括起来。
```javascript
`老师说，JavaScript 字符串用单引号 ' 或者双引号 " 括住都行，那我应该用单引号还是双引号呢？`
```

Backtick 字符串可以通过 `${}` 内嵌任意表达式。
```javascript
> `7 * 8 = ${ 7 * 8 }`
→ "7 * 8 = 56"
```
💡 Chrome, Safari,  Firefox, Edge 的最新版本都支持这种特性，IE 全系不支持，但是我们可以通过工具转换。

## 拼接字符串
通过 `+` 可拼接字符串，如
```javascript
> "唧唧复唧唧，" + "木兰当户织。"
→ "唧唧复唧唧，木兰当户织。"

> "3 乘以 6 的结果是 " + 3 * 6
→ "3 乘以 6 的结果是 18"

> "1 + 2 的结果是 " + (1 + 2)
→ "1 + 2 的结果是 3"
```

## 对比字符串
通过 `==` 或 `===` 可以确定两个字符串是否**相等**。
```javascript
> "Are you OK?" ==  "Are you OK?"
→ true
> "Are you OK?" === "Are you OK?"
→ true

> "Are you OK?" ==  "Are you ok?"
→ false
> "Are you OK?" === "Are you ok?"
→ false
```

通过 `!=` 或 `!==` 可以确定两个字符串是否**不等**。
```javascript
> "我有一只小毛驴" !=  "我从来也不骑"
→ true
> "我有一只小毛驴" !== "我从来也不骑"
→ true

> "两只老虎" !=  "两只老虎"
→ false
> "两只老虎" !== "两只老虎"
→ false
```

## 字符串长度
通过访问字符串的 `length` 属性可获取字符串长度。
```javascript
> "Are you OK?".length
→ 11
> "举头望明月，低头思故乡。".length
→ 12
> "好好Study，天天Happy。".length
→ 16
> "   ".length
→ 3
```

## 特殊字符



## 参考链接
* https://javascript.info/string
* https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Strings
