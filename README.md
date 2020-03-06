# GAMSマニュアル
最終更新日: 2020/03/05
本ファイルは、GAMS(General Algebraic Modeling System)の使用方法についてまとめている。  
GAMSは松橋研究室でよく使用されている、最適化計算用のソフトウェア。

## インストールの仕方
#### ライセンスファイルの使用
## プログラムの書き方
#### キーワード
#### モデル化時の注意点
- 最適化問題の種類について  

    <br/>
- ソルバーの選択に関して
    基本的によく使われるソルバーを以下に示す
    - MILP (Mixed Integer Linear Programming)の場合: gurobi, cplex
    - MINLP (Mixed Integer Non-Linear Programming)の場合: antigone

    <br/>
    基本的に中身を知らなくても最適化計算は行ってくれるが、個人的な考えでは具体的にどうやって解を探索していってるかのイメージは持っておいてほしい。

    混合整数計画においてよく使われるのはBranch-and-BoundやBranch-and-cutと呼ばれる手法で、YouTubeなどで検索すればたくさんヒットするし、最適化ゼミでもやったことがあるのでその資料とかを参考に。


    <br/>
        
- データの入力方法に関して 
    データの入力方法として.xlsxや.csvを使うことがあると思うが、.xlsxの方がデータの読み取り時間が長かったような気がする。
    
    一回のシミュレーションにおいては、実行時間のみ気にすればいいと思うが、モンテカルロシミュレーションなどにより繰り返し最適化計算を実行する場合には、入力データを読み取る時間も無視できなくなってくる。

    ただ、csvファイルでデータを入力すると、多くのcsvファイルが必要になるので、User-friendlyではなくなっていくかもしれない。


## プログラムの実行と結果の確認