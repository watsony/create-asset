# PRISM

## [Prism.js](https://prismjs.com)

> **PRISM**はエディタのようなビジュアルでコードをWeb表示するためのデザインテンプレート。CSSとJSファイルを[ダウンロード](https://prismjs.com/download.html#themes=prism-okaidia&languages=markup+css+clike+javascript)もしくはCDNで利用。


おすすめダウンロード設定
- Compression level: Minified version
- Themes: Okaidia
- Languages: Markup, CSS+C-like, JavaScript, Markup templating, Python, PHP, Git, YAML
- Plugins: Line Highlight, Line Numbers, Command Line, Copy to Clipboard Button, Unescaped Markup, Remove initial line feed, Normalize Whitespace, Treeview

上記設定のダウンロードURL:  
https://prismjs.com/download.html#themes=prism-okaidia&languages=markup+css+clike+javascript+git+markup-templating+php+python+yaml&plugins=line-highlight+line-numbers+remove-initial-line-feed+command-line+unescaped-markup+normalize-whitespace+toolbar+copy-to-clipboard+treeview


## 言語設定:  
```
<pre>
  <code class="language-html">
    PRISMで表示するコード
  </code>
</pre>
```
の```class```に言語を設定

| 言語名 | クラス指定 |
| --- | --- |
| なし | language-none |
| HTML | language-html |
| CSS | language-css |
| JavaScript | language-js |
| PHP | language-php |
| Python | language-python |
| Git | language-git |
| YAML | language-yaml |
| C | language-c |
| C++ | language-cpp |


## エスケープ
「<」は「&lt;」、「>」を「&gt;」に変換する。

## CDNの利用
JsDelivrからCDN利用可能
例：
```
<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">

    <!-- JsDelivr from https://www.jsdelivr.com/package/npm/prismjs -->

    <!-- Select Themes from https://www.jsdelivr.com/package/npm/prismjs?path=themes -->
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/prismjs@1.27.0/themes/prism-okaidia.min.css">
    <script src="https://cdn.jsdelivr.net/npm/prismjs@1.27.0/prism.min.js"></script>

    <!-- Add Components from https://www.jsdelivr.com/package/npm/prismjs?path=components-->
    <script src="https://cdn.jsdelivr.net/npm/prismjs@1.27.0/components/prism-python.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/prismjs@1.27.0/components/prism-git.min.js"></script>

    <!-- Add Plugins ex. line-numbers, command-line, line-highlight, toolbar, clipboard,.. from https://www.jsdelivr.com/package/npm/prismjs?path=plugins -->
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/prismjs@1.27.0/plugins/line-numbers/prism-line-numbers.min.css">
    <script src="https://cdn.jsdelivr.net/npm/prismjs@1.27.0/plugins/line-numbers/prism-line-numbers.min.js"></script>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/prismjs@1.27.0/plugins/command-line/prism-command-line.min.css">
    <script src="https://cdn.jsdelivr.net/npm/prismjs@1.27.0/plugins/command-line/prism-command-line.min.js"></script>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/prismjs@1.27.0/plugins/line-highlight/prism-line-highlight.min.css">
    <script src="https://cdn.jsdelivr.net/npm/prismjs@1.27.0/plugins/line-highlight/prism-line-highlight.min.js"></script>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/prismjs@1.27.0/plugins/toolbar/prism-toolbar.min.css">
    <script src="https://cdn.jsdelivr.net/npm/prismjs@1.27.0/plugins/toolbar/prism-toolbar.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/prismjs@1.27.0/plugins/copy-to-clipboard/prism-copy-to-clipboard.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/prismjs@1.27.0/plugins/normalize-whitespace/prism-normalize-whitespace.min.js"></script>
    
</head>
<body>
    <h1>Prism Template Code</h1>
    <pre class="line-numbers">
        <code class="language-html">
            &lt;h1&gt;Hello PRISM!&lt;/h1&gt;
            &lt;h1&gt;Hello CDN!&lt;/h1&gt;
        </code>
    </pre>

    <pre class="line-numbers">
        <code class="language-python">
            import numpy
            print("Hello World!")
        </code>
    </pre>

</body>
</html>
```

公式ガイド:  
【PRISM】Line Highlight: https://prismjs.com/plugins/line-highlight/  
【PRISM】Line Numbers: https://prismjs.com/plugins/line-numbers/  
【PRISM】Command Line: https://prismjs.com/plugins/command-line/#how-to-use  

参考サイト：  
HTMLエスケープツール: https://webtools.dounokouno.com/htmlescape/  
Qiita Prism.js 使ってみた: https://qiita.com/taqumo/items/825c862517ba9d8567a  
与太郎の備忘録: https://yotarandum.net/prismjs/  

My GitHub Code: https://github.com/watsony/create-asset/tree/main/prism  

My GitHub Pages サンプルサイト：  
https://watsony.github.io/create-asset/prism  
https://watsony.github.io/create-asset/prism/index-simple.html  
https://watsony.github.io/create-asset/prism-cdn.html  