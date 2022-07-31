修士論文・卒業論文用LaTeXテンプレート
=====================================

慶應義塾大学湘南藤沢キャンパス(SFC)政策・メディア研究科の修士論文用のテンプレートです。
[@ymrl](https://github.com/ymrl/)氏の[修士論文テンプレート](https://github.com/ymrl/thesis-template)(2012)を参考に、最新の大学院ガイドの形式に従って作り直しました。

また、同氏の説明によれば原典は[@kurokobo](http://twitter.com/kurokobo) による[卒業論文用テンプレート](http://wiki.kurokobo.com/index.php?LaTeX) (2010)だそうです。

主な変更点
---------

主な変更点は下記になります。

* SFCの修士論文最新フォーマット(2022)に準拠。  
* 氏名等、共通する記述をmain.texを参照して全て一つの変数で扱えるように変更。
* vscodeのの「Latex Workshop」プラグインを利用する前提の構成に変更。

使いかた
---------

基本は[修士論文テンプレート](https://github.com/ymrl/thesis-template)と同様ですので、そちらの使い方が詳細かつ丁寧です。  
そもそもLatexがわからない？これを機に勉強しましょう😌

画像等の挿入に関して
---------

PDF、画像の挿入を手軽に行えるよう、パッケージを先に記載してます。

大前提、画像は「resources」内部に配置します。

PDFの挿入
```
\includegraphics[width=\textwidth]{title.pdf}
```

画像の挿入
```
\begin{figure}[H]
  \begin{center}
    \includegraphics[width=\textwidth]{title.png}
    \caption{画像のタイトル}
  \end{center}
  \label{fig:title}
\end{figure}

```

参考文献の記載に関して
---------

「RefWorks」などの文献管理ソフトから.bib形式でファイルをエクスポートしてもらい、「main.bib」として保存すれば良いです。  
引用した順に参考文献リストに並ぶように設定しています。  
※余談ですが慶應でRefWorksのライセンスを使えるのは[SFC生だけ](https://libguides.lib.keio.ac.jp/refworks_new)らしいので、もっとフル活用しましょう。

ライセンス
---------
オリジナルのテンプレートについては（おそらく） [@kurokobo](http://twitter.com/kurokobo) 氏
に著作権があります。
また、全体の構成、設計は[@ymrl](https://github.com/ymrl/)氏のものがかなり強く反映されています。
元々自分が修士論文書くために作ったものですし、大した変更はしていないので、権利関係は[@ymrl](https://github.com/ymrl/)氏に倣い全て放棄します。ご自由にご利用ください。

その他
---------

デモや記載例はそのうち追加します。何かご質問等あれば[twitter](https://twitter.com/atomsphere5)へ