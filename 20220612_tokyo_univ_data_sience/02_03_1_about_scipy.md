# Scipyの基礎

## ライブラリ
* ルート：`scipy`
* 線形代数：`scipy.linalg`
* 最適化計算（最小値）用の関数：`scipy.optimize`

## 線形代数
* 行列式計算：`linalg.det`
* 逆行列計算：`linalg.inv`
* 固有値、固有ベクトル：`linalg.eig`
  * 固有値と固有ベクトルが同時に求められる：`eig_value, eig_vector = linalg.elg(matrix)`
* 

## 最適化計算
* ニュートン法
  * ニュートン法とは：https://ja.wikipedia.org/wiki/ニュートン法
    * `scipy.optimize.newton`
    * 第一引数：関数
    * 第二引数：解の探索を開始する点
* 最小値
  * `scipy.optimize.minimize_scalar`
  * 第一引数：関数
  * オプションで`method`を指定可能
    * 例：`method = 'Brent'`
    * ブレント法：https://ja.wikipedia.org/wiki/ブレント法
