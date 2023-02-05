# Kajitsudo AI proj2

ベビーリーフの収穫日予測プロジェクト2

栽培データと天候データ（気象庁もしくはハウス内のデータ）から収穫日（生育日数）を予測します．気象庁のデータを使った場合とハウス内のデータを使った場合で，どのような違いがあるのか調査する目的で作成しました．

処理の流れとしては，データの前処理 → モデル作成 → モデル評価となっています．

# Installation
1. Google Colaboratory にソースコードをアップロード

    1. Google Colaboratory にアクセス
    
        https://colab.research.google.com
        
    1. ソースコードをアップロード
    
        添付している「果実堂ベビーリーフ収穫日予測.ipynb」をアップロードする．
        
        
1. Google Drive にデータをアップロード

    データを参照できれば問題ないので，この通りにする必要はないです．
    
    1. 先ほどアップロードした「果実堂ベビーリーフ収穫日予測.ipynb」を開く
    
    1. 「果実堂ベビーリーフ収穫日予測.ipynb」の1.1及び1.2を実行する．
    
    1. Google Drive（https://drive.google.com/drive/my-drive ）に移動して，マイドライブ内に「kajitsudo_AI_proj」が作られていることを確認．
    
    1. kajitsudo_AI_projフォルダに移動し，添付しているデータをアップロード．以下のようなファイル構成になる．
        
        ```
        My Drive
        └─kajitsudo_AI_proj
            └─ data
                ├─ weather
                │   ├─ masiki_1209.csv
                │   ├─ kumamoto_1209.csv
                │   ├─ kahoku_1209.csv
                │   ├─ A1-12_日射_20210101_20211231_10min_a.csv
                │   ├─ A1-12_日射_20200101_20201231_10min_a.csv
                │   ├─ A1-12_日射_20190101_20191231_10min_a.csv
                │   ├─ A1-12_日射_20180101_20181231_10min_a.csv
                │   ├─ A1-12_日射_20170101_20171231_10min_a.csv
                │   ├─ A1-12_20210101_20211231_10min_a.csv
                │   ├─ A1-12_20200101_20201231_10min_a.csv
                │   ├─ A1-12_20190101_20191231_10min_a.csv
                │   ├─ A1-12_20180101_20181231_10min_a.csv
                │   └─ A1-12_20170101_20171231_10min_a.csv
                └─ input
                    ├─ seiikukeikaku_general.csv
                    ├─ seiikukeikaku_takasesiki_csv
                    ├─ data_2018192021.csv
                    ├─ data_2021.csv
                    └─ data_2018_2019_2020_checked.csv
        ```
    
以上で「果実堂ベビーリーフ収穫日予測.ipynb」のすべての実行が可能になります．

# Usage

基本的には上から順番に実行していくだけです．
        
2.2の天気データ読み込みに関して，ハウス内のデータを使うか気象庁のデータを使うか選択できます．
        
        2.2.1を実行　→　ハウス内のデータ

        2.2.2を実行　→　気象庁のデータ
        
一定時間経過もしくはパソコンを閉じるとGoogle Colaboratoryのセッションが切れるので，そのときはドライブのマウントから実行してください．（ただし，Google Drive へのデータのアップロードは1回で十分です．）

# Note

Google Chrome 上でのみテストしています．他のブラウザではテストを行っていません．

# Author
熊本高等専門学校

2022創成技術デザイン実習 第6班

代表者連絡先：
ae22niidome@g.kumamoto-nct.ac.jp
