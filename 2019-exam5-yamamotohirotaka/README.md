# 問題5

## 学籍番号: AE0033040
## 名前: 山本広高
## e-mail: hirotaka.yamamoto@thincess.com

1. git clone 後，適宜ブランチを設定する(例えば WorkInProg のように)

2. ``README.md`` ファイルの 受講生番号，氏名, e-mail を適宜書き換えること

3. jupyter notebook で記述された問題を解く

    - `ml-1.ipynb`: 行列の QR 分解．scipy の線形代数機能を用いて
      行列のQR分解を行う．QR分解自体は，最小二乗法を行うときに用いられる分解で，
      行列を直交行列 Q と上三角行列 R とに分解する手法である．
      scipyのチュートリアル

      https://docs.scipy.org/doc/scipy/reference/tutorial/linalg.html

      などを参考に QR 分解を行うこと．
      これらのコードを実行し，終了してからノートブックを保存する．

    - `ml-2.ipynb`: 簡単な機械学習による判別を行う．
      例題では，以下の手順で実験を行っている．
      `load_breast_cancer()` 関数をじっこうすると，データが読み込まれるので，
      `X` に乳がんの特徴値，`y` に乳がんかどうかのラベルを取り出す．
      
      次に，機械学習のモジュールである `sklearn` （scikit-learn）から
      ロジスティック回帰関数を用いて判別関数を求めている．
      
      sklearn の使い方に関しては，
      http://scikit-learn.org/stable/index.html
      の Classfication を参考のこと．
      基本的には 識別器 (`cls`という変数名) を作ったら，
      データをフィット(`cls.fit()`)させ，
      データからラベルを予測する（`cls.predit()`) ことで判別を行う．

      さらに，accuracy_score() 関数を用いて，真のラベル値 `y` と
      予測ラベル値 `y_pred` を計算し，性能を `accuracy_score()` で評価している
      
      ここまでを実行した上で，別の識別器を構築することを考えなさい．
      識別機械としては サポートベクターマシンやk-means 法などが考えられる．
      これらの使い方に関しても
      http://scikit-learn.org/stable/index.html
      を参照のこと．

      これらのコードを実行し，終了してからノートブックを保存する．


4. 以上の操作を行い，保持したファイルを ``git add``, ``git commit`` を用いて
   更新し，バックアップを取る場合には ``git push -u ブランチ名`` といった操作を行う．
   
5. 最終的に課題を提出する場合は，`github` のウェブインターフェースにある 
   `pull request` リンクを押して，必要な場合はコメントなどを残し 
   `Create pull request` ボタンを押してを送り課題終了

