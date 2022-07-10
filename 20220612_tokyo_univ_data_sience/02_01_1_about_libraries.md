# データ分析で使うライブラリ

## 本書で使用するライブラリ：

* [NumPy（ナンパイ）](https://numpy.org/)
* [Scipy（サイパイ）](https://scipy.org/) NumPyの拡張
* [Pandas（パンダス）](https://pandas.pydata.org/)
* [Matplotlib（マトプロットリブ）](https://matplotlib.org/)

## 読み込み方法

下記の2通りがある。

* `import モジュール名[.機能名] as 識別子`
  * 識別子として任意の名前を指定可能（例：`import numpy as np`）
  * 同時に複数インポートできない（複数行書く必要がある）
* `from モジュール名 import 機能名`
  * 同時に複数インポート可能

## マジックコマンド

* マジックコマンドとは
  * IPythonの拡張機能
  * IPythonとは
    * Pythonの対話型インタプリタを拡張したもの（[参考](https://www.magata.net/memo/index.php?IPython%A4%CE%BB%C8%A4%A4%CA%FD%A5%E1%A5%E2)）
    * 入力補完、変数操作、デバッグ等の便利機能あり
    * Jupyter NotbookはもともとIPython Notebookという名前だった（[参考](https://office54.net/python/basic/ipython-install-jupyter)）
    * つまり、Jupyter Notebookはブラウザ版IPython
* lineマジックとcellマジックがある（[参考](https://www.magata.net/memo/index.php?IPython%A4%CE%BB%C8%A4%A4%CA%FD%A5%E1%A5%E2)）
  * lineマジックは1行分のコマンド
    * コマンドの頭に`%`が付く
  * cellマジックは複数行に渡るコマンド
    * コマンドの頭に`%%`が付く
* `%quickref`でリファレンス閲覧
* `%lsmagic`でマジックコマンド一覧表示

```
import numpy as np
import numpy.random as random
import scipy as sp
import pandas as pd
from pandas import Series, DataFrame

# 可視化ライブラリ
import matplotlib.pyplot as plt
import matplotlib as mpl
import seaborn as sns
%matplotlib

# 小数点3位まで表示
%presicion 3
```