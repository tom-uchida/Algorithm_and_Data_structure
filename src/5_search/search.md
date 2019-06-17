## 探索

### 線形探索
- 線形探索は，配列の先頭から各要素が目的の値を等しいかどうかを順番に調べる．
- 等しいものが見つかった時点でその位置を返し，探索を終了する．
- 末尾まで調べて目的の値が存在しなかった場合は，その事を示す特別な値を返す．
- アルゴリズムの効率は悪いが，線形探索はデータの並び方に関係なく適用することができる．

### 二分探索
- 二分探索は，データの大小関係を利用した探索アルゴリズム
- キーの昇順に並んだデータが配列に格納されているとすると，二分探索のアルゴリズムは次のようになる．

```
二分探索のアルゴリズム
1. 配列全体を探索の範囲とする．
2. 探索の範囲内の中央の要素を調べる．
3. 目的のキーと中央の要素のキーが一致すれば探索を終了する．
4. 目的のキーが中央の要素のキーよりも小さければ前半部分を，大きければ後半部分を探索の範囲として 2. へ戻る．
```

- 各計算ステップが終わるごとに，調べる範囲が半分になっていくので，高速に探索を行うことができる．

### ハッシュ法
- ハッシュ法では，ハッシュ関数と呼ばれる関数値によって，要素の格納場所を決定する．
- これは，データ構造の一種でもあり，ハッシュテーブルと呼ばれる表を用いるアルゴリズム．
- 要素のキー(値)を引数とした関数を呼び出すだけで，その位置を特定することができるので，データの種類によっては，より高速なデータの検索が可能になる．