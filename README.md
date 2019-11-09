PXchfon-extras
==============

LaTeX： pxchfon パッケージ用の追加プリセット定義

### 前提環境

  * フォーマット： LaTeX
  * エンジン： pTeX、upTeX
  * DVIウェア： dvipdfmx
  * 依存パッケージ：
      - pxchfon

### インストール

  - `*.def`      → $TEXMF/tex/platex/pxchfon-extras/

### ライセンス

MITライセンスの下で配布される。

--------------------

使用法
------

インストールしておくだけで、pxchfon を読み込む際に自動的に有効になる。

### 追加プリセット一覧

以下に挙げるプリセットは、[ptex-fontmaps] における同名のマップファイルと
同等の設定を行う。

※macOS 付属のフォントについては、cjk-gs-integrate(-macos) により適切な
リンクが生成されている状態を前提とする。（参照：[cjk-gs-support]）

  * ms-osx
  * bizud
  * canon
  * hiragino-highsierra-pron
  * hiragino-highsierra
  * toppanbunkyu-sierra
  * toppanbunkyu-highsierra

独自のプリセット。

  * yu-highsierra： macOS 10.13 (High Sierra) 以降に付属する游フォント。
    ただし、Windows 上の動作の場合は Windows 10 の游フォントを利用した
    定義に振り替えられる。定義は以下の通り（括弧内は Windows の場合）。

      - 明朝・細：       YuMin-Medium     (YuMincho-Regular)
      - 明朝・中：       YuMin-Medium     (YuMincho-Regular)
      - 明朝・太：       YuMin-Demibold   (YuMincho-Demibold)
      - ゴシック・中：   YuGothic-Medium
      - ゴシック・太：   YuGothic-Bold
      - ゴシック・極太： YuGothic-Bold

    ※macOS・Windows の何れの場合も“AJ1 でない”フォントであるため、この
    プリセットを指定した場合は `unicode` が自動的に有効になる。


[ptex-fontmaps]: https://github.com/texjporg/jfontmaps
[cjk-gs-support]: https://github.com/texjporg/cjk-gs-support


--------------------

更新履歴
--------

  * Version 0.2  〈2019/10/09〉
      - 最初の公開版。

--------------------
Takayuki YATO (aka. "ZR")  
https://github.com/zr-tex8r
