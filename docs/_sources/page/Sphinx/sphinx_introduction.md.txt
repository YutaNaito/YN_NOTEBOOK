# Sphinxの導入

1. sphinxのインストール
    - `pip install sphinx`
2. ディレクトリ作成
    - `m kdir <PROJECT_DIRECTORY> && cd <PROJETCT_DIRECTORY>`
3. 作成したディレクトリでプロジェクト作成
    ```
    $ sphinx-quickstart
    Welcome to the Sphinx 3.1.2 quickstart utility.

    Please enter values for the following settings (just press Enter to
    accept a default value, if one is given in brackets).

    Selected root path: .

    You have two options for placing the build directory for Sphinx output.
    Either, you use a directory "_build" within the root path, or you separate
    "source" and "build" directories within the root path.
    > Separate source and build directories (y/n) [n]: y

    The project name will occur in several places in the built documentation.
    > Project name: プロジェクト名
    > Author name(s): 筆者名
    > Project release []: リリースバージョン

    If the documents are to be written in a language other than English,
    you can select a language here by its language code. Sphinx will then
    translate text that it generates into that language.

    For a list of supported codes, see
    https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-language.
    > Project language [en]: ja

    Creating file C:\Workspace\Python\sample-sphinx\source\conf.py.
    Creating file C:\Workspace\Python\sample-sphinx\source\index.rst.
    Creating file C:\Workspace\Python\sample-sphinx\Makefile.
    Creating file C:\Workspace\Python\sample-sphinx\make.bat.

    Finished: An initial directory structure has been created.

    You should now populate your master file C:\Workspace\Python\sample-sphinx\source\index.rst and create other documentation
    source files. Use the Makefile to build the docs, like so:
        make builder
        where "builder" is one of the supported builders, e.g. html, latex or linkcheck.
    ```
4. HTMLの作成
    - `make html`

    上記のコマンドはWindows標準搭載のコマンドプロンプトで使用できるコマンドであり、Git BashなどのUNIX系コマンドラインでは以下のコマンド
      - `sphinx-build -d docs/.doctrees source docs`
      - `./make.bat html`

#### 参考資料
- [sphinxのインストール](https://www.sphinx-doc.org/ja/1.4/install.html)
- [sphinxでドキュメント作成からWeb公開までをやってみた](https://qiita.com/kinpira/items/505bccacb2fba89c0ff0)
- [4.Sphinxでの文章の書き方(reStructuredText)](https://planset-study-sphinx.readthedocs.io/ja/latest/04.html)
- [ふだんMarkdownを書く技術者のためのreStructuredText文法まとめ](https://gotohayato.com/content/464/)
- [Sphinxによるドキュメント作成と国際化の事始め](https://qiita.com/tatsurou313/items/8bf7b43842b7827760fa)