# Welcome to MkDocs

For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.

---

## 0. MkDocsの環境構築
> Python環境の起動

venvの場合：例
- 仮想環境 "~/.venv/myenv"の作成
```
$ python -m venv ~/.venv/myenv
```
- 作成した仮想環境の起動
```
$ source ~/.venv/myenv/activate/bin
```

> MkDocsのインストール
```
$ pip install mkdocs
```

---

## 1. MkDocsプロジェクト作成
```
$ mkdocs new .
```

## 2. WebPageファイルの生成
```
$ mkdocs build
``` 
※ mkdocs.yml と同じ階層で実行

## 3. ローカル環境でサイトをホスティング
```
$ mkdocs serve
```
ローカルで確認
[http://127.0.0.1:8000/](http://127.0.0.1:8000/)

---

## ビルド実行後のディレクトリ構造
<pre>
root/
├── docs/
│   └── index.md
├── mkdocs.yml
└── site/
</pre>

## 初期設定の "mkdocs.yml"
```
site_name: My Docs

```

## 初期設定の ["index.md"](https://github.com/watsony/create-asset/tree/main/MkDocs/site-default/index.md)
```
# Welcome to MkDocs

For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.

```


## GitHub Pages URL
[https://watsony.github.io/create-asset/MkDocs/site-default](https://watsony.github.io/create-asset/MkDocs/site-default)

## GitHub Pages にデプロイ（自動で gh-test ブランチ生成）
```
$ mkdocs gh-deploy
```