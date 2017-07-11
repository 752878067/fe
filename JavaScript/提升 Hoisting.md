# 提升 Hoisting

JavaScript 中的提升(Hoisting)特指使用 `var` 声明的变量和函数声明被提升到所在作用域的顶端。

## 变量提升

⚠️ `let` 不存在变量提升。

## 函数提升
函数声明会被提升到所在作用域的顶端，因此调用语句可以放在函数声明之前。
```javascript
(function() {

  sing();
  
  function sing() {
    console.log('少林功夫好耶 真好耶🎸');
  }
  
})();
```
⚠️ 函数表达式不会被提升，因此调用前要先声明，否则会报错。
```javascript
(function() {
  
  var moon = function() { console.log('床前明月光，疑是地上霜。'); }
  
  moon();  // 正常
  home();  // 报错 Uncaught TypeError: home is not a function
  
  var home = function() { console.log('举头望明月，低头思故乡。'); }

})();
```

## 参考链接
* http://es6.ruanyifeng.com
* https://zhuanlan.zhihu.com/p/27558914
* https://github.com/getify/You-Dont-Know-JS/issues/767
* https://developer.mozilla.org/en-US/docs/Glossary/Hoisting
* http://www.adequatelygood.com/JavaScript-Scoping-and-Hoisting.html
* https://rainsoft.io/variables-lifecycle-and-why-let-is-not-hoisted
* http://adripofjavascript.com/blog/drips/variable-and-function-hoisting
* https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/var
* https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let
* https://stackoverflow.com/questions/31219420/are-variables-declared-with-let-or-const-not-hoisted-in-es6
* https://medium.freecodecamp.org/what-is-variable-hoisting-differentiating-between-var-let-and-const-in-es6-f1a70bb43d

