---
---


## 基本的なルール

* インデント:
  soft 4

* 文字数:
  79

## 命名規則

### Interface
  
先頭に `I` を付ける

```
ILogger
Module.ILogger
```

## public, private宣言

かならず付ける

### プロパティ宣言

コンストラクタの引数でプロパティを宣言できるが、明確な使い分けは不明

```
class Hoge {
    constructor(public a: string, public b: number, private c: string) {
    
    }
}

```

### コロン

一貫して左とスペースを開けずに、右とスペースを一つとる。
```
public errorReporter: ErrorReporter = null;
```

### var時の型宣言

基本的に必要ないが、以下のようなケースでは書いた方がよさそう

any[]から取得したオブジェクト。

```
var name: string = names[i];
var description: string = description[name];
```

### 即時関数

JavaScriptにあわせてかく？

```
(function(){})();
```

### enum

アッパーキャメル

```
export enum TokenID {
    Any,
    Bool,
    Break,
    Case,
    Catch,
    //....
    Comment,
    Lim,
    LimFixed = EqualsGreaterThan,
    LimKeyword = Yield,
}
```


## 関数の返り値の型

voidの時は明示しない

```
public voidFunction() {
  
}
```

void以外のときは明示する

```
public stringFunction(): string {
    return "aaaa";
}
```

## キャスト

そのままメソッドチェインとかするときには `()`　つける

```
(any>hoge).fuga()
```

## 関数

```
var hoge = (fuga: Fuga) => {
  // hoge
}
```

## 定数

大文字のスネークケース
