# fetch_cazy

## fetch_fasta.ipynb
CAZyデータベースからダウンロードできる NCBI ID リストをクエリに配列を取得します。

### 準備
1)  Google drive に解析用のディレクトリを作る。
2) [GitHub](https://github.com/lomon978410/fetch_cazy) > Code > Download zip  からファイルをダウンロードし、解凍した fetch_fasta.ipynb ファイルを自分の Google drive に保存する。
3) 保存したファイルを右クリック、アプリで開く から Google Colaboratory を選択して開く。選択肢にない場合はアプリを接続する。

### 実行
1) ダウンロードした ID の .txt ファイルを解析用のディレクトリにアップロードする。
2) コード中の `Entrez.email = "xxxx@yyyy.zz"` を自分のアドレスに書き換える。
3) `ID_list="/content/drive/MyDrive/xxx/yyy/zzz.txt"` このパスを ID の .txt ファイルのものに書き換える。
4) ランタイム > すべてのセルを実行 をクリックして実行。または、三角のマークをクリックしてセルを一つずつ実行。

# fetch_fasta.ipynb

CAZy のサイトからウェブスクレイピングを行って GenBank ID を取得し、配列をダウンロードする。

準備はfetch_fasta.ipynbと同じ。

### 実行
1) コード中の `Entrez.email = "xxxx@yyyy.zz"` を自分のアドレスに書き換える。
2) `outdir=` の後ろのパスをファイルを出力したいディレクトリに書き換える。
3) `cazy_url=` の後ろのurl を取得したいCAZy のページのものに書き換える。配列が 100 を越える場合は複数のタブがあるので注意。
4) ランタイム > すべてのセルを実行 をクリックして実行。または、三角のマークをクリックしてセルを一つずつ実行。
