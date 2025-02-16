---
title: <xsl:variable>
slug: Web/XSLT/Element/variable
tags:
  - XSLT
  - variable
  - リファレンス
  - 要素
translation_of: Web/XSLT/Element/variable
---
{{ XsltRef() }}

`<xsl:variable>` 要素はスタイルシートにグローバル変数またはローカル変数を宣言し、値を与えます。XSLT は副作用を許さないため、変数の値が設定されると、変数がスコープから外れるまでは変わりません

### 構文

```
<xsl:variable name=NAME select=EXPRESSION >
  TEMPLATE
</xsl:variable>
```

### 必須属性

- `name`
  - : 変数に名前を付けます。

### 任意属性

- `select`
  - : XPath 式を使用して変数の値を定義します。要素にテンプレートが含まれている場合、この属性は無視されます。

### タイプ

トップレベルまたは指示。トップレベル要素として発生するとその変数は範囲がグローバルであり、ドキュメント全体からアクセスできます。テンプレート内で発生する場合、変数はスコープ内でローカルであり、変数が現れるテンプレート内でのみアクセスできます。

### 定義

XSLT, section 11.

### Gecko のサポート

サポート済み
