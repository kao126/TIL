## 3-1 基数変換 ☆
- 進数
  - 2進数：0と1
  - 8進数：0-7
  - 10進数：0-9
  - 16進数：0-9, A-F
- 基数：各桁の重み付けの基本となる数

[N進数の重み対応表]
|・・・| N² | N¹ | N⁰ | 小数点（.） | N<sup>-1</sup> | N<sup>-2</sup> |・・・| 
|---|---|---|---|---|---|---|---|

> 「N進数の重み」とくれば「小数点を基準に左へ、N⁰, N¹, N², …」「小数点を基準に右へ、N<sup>-1</sup>, N<sup>-2</sup>, …」

- 基数変換：別の進数で表現し直すこと

> 「N進数→10進数」とくれば「各桁にN進数の重みを掛けて足す」
> 
> 「10進数→N進数」とくれば「整数部は、Nで割って下から余りを並べる」「小数部は、Nで掛けて順に整数部を並べる」

>「2進数→8進数」とくれば「小数点を基準に、3桁ずつ区切って、8進数に変換する」
>
>「2進数→16進数」とくれば「小数点を基準に、4桁ずつ区切って、16進数に変換する」


## 3-2 補数と固定小数点
- 補数：「ある数」を「決められた数」にするために、「補う数」のこと
> 「1の補数」とくれば「ビットを反転する」
> 
> 「2の補数」とくれば「1の補数に1を加える」

- 固定小数点：小数点の位置を決められた場所に固定して表現するもの


## 3-3 浮動小数点
- 浮動小数点：実数（小数点の付いた数）を扱う場合に使用する形式
- 正規化：桁移動


## 3-4 誤差
- 誤差：真の値と表現する値との間に差が発生すること
- **桁あふれ誤差**：演算結果がコンピュータの表現できる範囲を超えること（オーバーフロー/アンダフロー）で発生する誤差
> 「桁あふれ誤差」とくれば「表現できる範囲を超えることで発生する誤差」
> 
> 「丸め誤差」とくれば「切捨て・切上げ・四捨五入することで発生する誤差」

- **桁落ち誤差**：絶対値がほぼ等しい数値の間で、同符号の減算や異符号の加算をしたときに、有効桁数が減ることで発生する誤差
> 「桁落ち誤差」とくれば「有効桁数が減少することで発生する誤差」

- **情報落ち誤差**：絶対値の差が非常に大きい数値の間で加減算を行ったときに、絶対値の小さい数値が計算結果に反映されないことで発生する誤差
> 「情報落ち誤差」とくれば「小さな数値が計算結果に反映されないことで発生する誤差」
> 
> 「打切り誤差」とくれば「計算処理を打ち切ることで発生する誤差」


## 3-5 シフト演算 ◎
- シフト演算：左右にビットをずらして（シフトして）、乗算や除算の演算をすること
> 「シフト演算」とくれば「nビット左にシフト→2ⁿ倍」「nビット右にシフト→1/2ⁿ倍」

- 論理シフト：符号を考慮しないシフト演算
> 「論理シフト」とくれば「あふれたビットは捨てる」「空いたビットには0を入れる」

- 算術シフト：符号を考慮するシフト演算
> 「算術左シフト」とくれば「符号ビットはそのまま」「あふれたビットは捨てる」「空いたビットには0を入れる」
> 「算術右シフト」とくれば「符号ビットはそのまま」「あふれたビットは捨てる」「空いたビットには符号ビットと同じビットを入れる」


## 3-6 論理演算 ☆
- 論理演算：「1と0」または「真と偽」のように、2値のうちいずれか一方の値を持つデータ間で行われる演算
  - 論理和（OR）
  - 論理積（AND）
  - 否定（NOT）

> 「論理和」とくれば「入力が少なくとも一方が1ならば、出力が1」
> 
> 「論理積」とくれば「入力の両方が1ならば、出力が1」
> 
> 「否定」とくれば「入力が1ならば、出力が0。入力が0ならば、出力が1」

- 論理演算の組み合わせ
  - 排他的論理和（EOR/XOR）
  - 否定論理和（NOR）
  - 否定論理積（NAND）

> 「排他的論理和」とくれば「入力が異なれば、出力が1」
> 
> 「否定論理和」とくれば「論理和の否定」
> 
> 「否定論理積」とくれば「論理積の否定」

- ビット演算
> 「ある特定のビットを取り出す」とくれば「取り出したいビットと1で論理積（AND）」
> 
> 「ある特定のビットを反転させる」とくれば「反転させたいビットと1で排他的論理和（EOR）」


## 3-7 半加算器と全加算器
- 加算器：2進数の加算を行う回路
  - 半加算器：2つの2進数を加算して、同桁の値（S）と桁上がり（C）を出力する加算器
  - 全加算器：上位桁への桁上がり（C）だけでなく、下位桁からの桁上がり（C'）も考慮した加算器

> 「半加算器」とくれば「上位桁への桁上がりのみ考慮した加算器」
> 
> 「全加算器」とくれば「下位桁からの桁上がりと上位桁への桁上がりを考慮した加算器」


## 3-8 計測と制御 ☆
- アナログとディジタル
  - アナログデータ：連続的に変化する情報
  - ディジタルデータ：アナログデータを「0」と「1」に区切って置き換えた不連続な情報
  - A/D変換：アナログ→デジタルに変換すること
  - D/A変換：デジタル→アナログに変換すること
- **PCM伝送方式（Pulse Code Modulation）**：アナログの音声信号をディジタル符号に変換する方式
  - 標本化：アナログ信号を一定の時間間隔で測定すること（別称：サンプリング/Hz）
  - 量子化：決められた一定の間隔に区切り数値化すること
  - 符号化：量子化された値を2進数のディジタル符号に変換すること
- 制御技術
  - フィードバック制御：外部の作用（外乱）の影響をセンサで検知して、コンピュータが判断し、修正動作を行う制御
    - フィードフォワード制御：あらかじめ外乱を予測できる場合に、前もって必要な修正動作を行う
    - シーケンス制御：あらかじめ定められた順序や条件に従って、制御の各段階を逐次進めていく
  - PWM制御（Pulse Width Modulation）：モータの回転速度やLEDの明るさなどをディジタル信号で制御する方式
  - 電力量
    - アンペア（A）：電流。電気の流れ
    - ボルト（V）：電圧。電気を流そうとする力の強さ
    - ワット（W）：消費電力。消費される電力


## 3-9 オートマトン ◎
- オートマトン：現在の状態と入力によって、出力が決定される機械をモデル化したもの（例：自販機）
  - 有限オートマトン：最終的に受理状態（終了状態）になるもの
  - **状態遷移図**：オートマトンの状態の遷移を図にしたもの
  - 状態遷移表：オートマトンの状態の遷移を表にしたもの


## 3-10 AI ☆
- **AI(Artificial Intelligence)**：人が行うような学習・認識・予測・判断などの知的な活動を、コンピュータにさせる取組みやその技術のこと（人工知能）
- **機械学習**：大量のデータ（ビッグデータ）をコンピュータに解析させ、コンピュータ自らが予測や判断などができるように学習させること
  - **教師あり学習**：あらかじめ問題（データ）と正解をコンピュータに提示し、誤りを指摘したりすることで、コンピュータ自らがそれらの特徴を学習すること
  - 教師なし学習：コンピュータ自らが、統計的性質やある種の条件に従い、データのグループ分け（クラスタリング）や、情報の集約を行うこと
  - 強化学習：試行錯誤を通して、報酬（評価）が最も多く得られるような方策を学習すること
- **ディープラーニング**：人の脳神経回路を模倣したモデル（**ニューラルネットワーク**）で解析し、AI自らがデータを判別するための特徴を探し出すこと（深層学習）


## 3-11 線形代数 ◎
- スカラー：大きさを表す数値のこと
- ベクトル：数値、つまりスカラーを一列に並べたもの
> 「行列」とくれば「横方向のまとまりが行、縦方向のまとまりが列」
- 行列
  - 正方行列：行と列が同じ数になっている行列
  - 単位行列（*E*）：左上からの対角線上の成分が1、それ以外の成分が0である正方行列
  - 逆行列（A<sup>-1</sup>）：行列Aに行列Bを掛けて単位行列が得られる場合、行列Bは行列Aの逆行列


# 3-12 確率・統計 ☆
- 確率：ある事象の起こる可能性の度合いのこと</br>
`確率 = ある事象の起こる場合の数 / 起こりうる事象のすべての場合の数`

- 順列：n個の中からr個取り出して並べたもの</br>
`n個の中からr個を取り出す順列の数は、nPr = n!/(n-r)! (n≧r)`

- 組合せ：n個の中から並び順を考慮せずにr個取り出したもの
`n個の中からr個を取り出す組合せの数は、nCr = n!/r!(n-r)! (n≧r)`

- 統計
  - 平均値：各データの合計をデータの個数で割って求めた値
  - メジアン（中央値）：データを順番に並べて中央に位置する値
  - モード（最頻値）：出現頻度の最も高い値
  - レンジ（範囲）：データの最大値と最小値の差
  - 分散：平均値からのばらつきを表し、偏差（平均値との差）の2乗の総和の平均値
  - 標準偏差：分散の平方根（√）

> 「メジアン」とくれば「中央値（真ん中の値）」
> 
> 「モード」とくれば「最頻値（最も頻繁に現れる値）」
> 
> 「レンジ」とくれば「範囲（最大値 - 最小値）」

- 正規分布：平均値を中心とした左右対称の釣り鐘型の分布
> 「正規分布」とくれば「釣り鐘型に分布する」
