- 下はプロジェクトの指示を作成するための指示。
- 八つの各プロジェクトは項目「全プロジェクト共通」と各プロジェクトを示す項目に従うこと。

# 全プロジェクト共通

指示内容は次のコードブロック内。

``` markdown
# 基本

## 作品 <work root>

- ユーザーは <work root> をフォルダパスで設定する。
- <work root> は作品に関するルートフォルダとする。
- 作品は一つまたは複数の章を持つ。

## 章 <chapter>

- ユーザーは <chapter> を自然数で設定する。
- <chapter> は物語全体を分割する最大の単位「章」の番号とする。
- 同一 <work root> 内に連番で設定される <chapter> の章同士は <chapter> に沿って続きものとする。
- 以前の <chapter> がある場合にはその章の内容を参照する。

## エピソード <episode>

- <episode> は章を分割する単位「エピソード」の番号とする。
- 同一作品内の同一章内のエピソードは <episode> に沿って続きものとする。ただしプロットに従って時間や場所に連続性がない場合もある。
- 以前の <episode> がある場合はそのエピソードの内容を参照する。

## その他

- 文字数を扱うとき改行記号やスペースを数えない。

# フォルダ構造・ファイルの役割

- `<work root>\settings\config.md`:                           作品全体のテーマ、コンセプト、ログライン
- `<work root>\settings\characters.md`:                       キャラクター設定
- `<work root>\settings\world-building.md`:                   世界設定
- `<work root>\settings\things.md`:                           物事全般の設定
- `<work root>\settings\place.md`:                            地域、土地の設定
- `<work root>\settings\location.md`:                         空間、部屋の設定
- `<work root>\plot\<chapter>\plot-a-<chapter>.md`:           プロット a。
- `<work root>\plot\<chapter>\plot-b-<chapter>.md`:           プロット b。
- `<work root>\plot\<chapter>\plot-c-<chapter>-<episode>.md`: プロット c。
- `<work root>\text\<chapter>\text-<chapter>-<episode>.txt`:  本文。
- `<work root>\text\<chapter>\cover.md`:                      タイトル、キャッチコピー、あらすじ。
```

- - - -

# プロジェクト 1

- コンフィグ
- プロンプトに入力する内容
  - <work root>
  - <chapter>
  - 元になるアイデア
  - ジャンル
  - 全体の文字数
  - エピソードの数量
  - 本文の改行方式
- 指示内容は次のコードブロック内。

``` markdown
# ユーザーによる設定

今回の章について次を設定する。

- 元になるアイデア
- ジャンル
- 全体の文字数
- エピソードの数量
- 本文の改行方式

# ChatGPTによる設定

- 各エピソードの文字数についておおよその数を、 `章全体の文字数` を `エピソードの数量` で除して求める。
- ユーザーのアイデアを実現するのに最適なテーマ、コンセプト、ログラインを創作する。

# 設定の記録

`<work root>\settings\config.md` にユーザーおよびChatGPTによる設定の内容と、その他の特筆すべき事柄を記録する。
```

- - - -

# プロジェクト 2

- 世界設定
- プロンプトに入力する内容
  - <work root>
  - <chapter>
- 指示内容は次のコードブロック内。

``` markdown
次のファイルを参照し、記述内容を実現するのに必要十分な世界観を創作して設定する。

- `<work root>\settings\config.md`

# 設定の記録

- `<work root>\settings\world-building.md` に世界設定を記録する。
- `<work root>\settings\things.md` に物事全般の設定を記録する。
- `<work root>\settings\place.md` に地域、土地の設定を記録する。
- `<work root>\settings\location.md` に空間、部屋の設定を記録する。
```

- - - -

# プロジェクト 3

- キャラクター
- プロンプトに入力する内容
  - <work root>
  - <chapter>
- 指示内容は次のコードブロック内。

``` markdown
次のファイルを参照し、記述内容を実現するのに必要十分なキャラクターを創作して設定する。

- `<work root>\settings\config.md`
- `<work root>\settings\world-building.md`
- `<work root>\settings\things.md`
- `<work root>\settings\place.md`
- `<work root>\settings\location.md`

# 設定内容

- 呼称
  - 対象：全キャラクター
- 役割
  - 対象：全キャラクター
  - メモ：役割名は主人公、ヒロイン、敵、モブなど
- フルネーム
  - 対象：メインキャラクター、サブキャラクター
- 魅力
  - 対象：メインキャラクター、サブキャラクター
- 欠点
  - 対象：メインキャラクター、サブキャラクター
- 一言で言い表せる性格の概要
  - 対象：メインキャラクター、サブキャラクター
- 性格要素
  - 対象：メインキャラクター、必要ならサブキャラクター
- 外見
  - 対象：全キャラクター
  - メモ：必要十分な量
- その他の有用な性質
  - 対象：全キャラクター

# 設定の記録

- `<work root>\settings\characters.md` にキャラクター設定を記録する。
- 世界設定に追加・変更が必要な場合には `<work root>\settings\world-building.md` を更新する。
- 物事全般の設定に追加・変更が必要な場合には `<work root>\settings\things.md` を更新する。
- 地域、土地の設定に追加・変更が必要な場合には `<work root>\settings\place.md` を更新する。
- 空間、部屋の設定に追加・変更が必要な場合には `<work root>\settings\location.md` を更新する。
```

- - - -

# プロジェクト 4

- 基礎プロット（plot-a）
- プロンプトに入力する内容
  - <work root>
  - <chapter>
- 指示内容は次のコードブロック内。

``` markdown
目的：全体の概要、最重要ポイントの設計。

次のファイルを参照し、記述内容を実現するのに必要十分な基礎プロットを創作して設定する。

- `<work root>\settings\config.md`
- `<work root>\settings\world-building.md`
- `<work root>\settings\characters.md`
- `<work root>\settings\things.md`
- `<work root>\settings\place.md`
- `<work root>\settings\location.md`

# 設定内容

- 始まりの状態
- 終わりの状態
- 中盤に主人公が絶望する状況
- 絶望を振り払った主人公が逆転の猛攻によってクライマックスを制する状況

# 設定の記録

- `<work root>\plot\<chapter>\plot-a-<chapter>.md` に設定内容を記録する。
- 世界設定に追加・変更が必要な場合には `<work root>\settings\world-building.md` を更新する。
- キャラクター設定に追加・変更が必要な場合には `<work root>\settings\characters.md` を更新する。
- 物事全般の設定に追加・変更が必要な場合には `<work root>\settings\things.md` を更新する。
- 地域、土地の設定に追加・変更が必要な場合には `<work root>\settings\place.md` を更新する。
- 空間、部屋の設定に追加・変更が必要な場合には `<work root>\settings\location.md` を更新する。
```

- - - -

# プロジェクト 5

_ChatGPTへの問い合わせ：一つのプロジェクトでコードブロック内の設定内容を設定するより分けたほうがいいか。_

- 中間プロット（plot-b）
- プロンプトに入力する内容
  - <work root>
  - <chapter>
- 指示内容は次のコードブロック内。

``` markdown
目的：全体の詳細、重要ポイント　1つのプロジェクトに収めていいかChatGPTにたずねる。

次のファイルを参照し、記述内容を実現するのに必要十分な中間プロットを創作して設定する。

- `<work root>\settings\config.md`
- `<work root>\settings\world-building.md`
- `<work root>\settings\characters.md`
- `<work root>\settings\things.md`
- `<work root>\settings\place.md`
- `<work root>\settings\location.md`
- `<work root>\plot\<chapter>\plot-a-<chapter>.md`

# 設定内容

- なにがしかの形での中程度のピンチに2回陥るが事前に得た知識・技術・アイテム・その他の何かによって切り抜ける。ただしピンチは多くなってもいい。
- なにがしかの形での軽程度のピンチに2回陥るが事前に得た知識・技術・アイテム・その他の何かによって切り抜ける。ただしピンチは多くなってもいい。
- クライマックスでは新事実によってピンチに陥るが中盤に得た知識・技術・アイテム・その他の何かによって切り抜ける。
- クライマックスの新事実には物語全体に3回以上のヒントを配置する。
- 新事実には同一エピソード内またはエピソードを越えて伏線を張っておく。
- 発生する中程度以上の問題には同一エピソード内またはエピソードを越えて伏線を張っておく。
- エピソード内のクライマックスを設置し、メインプロットについて主人公の目的や欲求によって戦闘・交渉・売買・会話・その他の広い意味での交渉を持たせ、ランダムに次のような結果にする。
  - 4割のケースでは思惑どおり目的や欲求が達せられ、話が展開して次の目的や欲求に繋がる。
  - 4割のケースでは思惑と少しだけズレて達せられ、ズレていることで次の目的や欲求につながる。
  - 2割のケースでは思惑どおりいかず失敗するが別のヒントを得、そのことで次の目的や欲求につながる。

# 設定の記録

- `<work root>\plot\<chapter>\plot-b-<chapter>.md` に設定内容を記録する。
- 世界設定に追加・変更が必要な場合には `<work root>\settings\world-building.md` を更新する。
- キャラクター設定に追加・変更が必要な場合には `<work root>\settings\characters.md` を更新する。
- 物事全般の設定に追加・変更が必要な場合には `<work root>\settings\things.md` を更新する。
- 地域、土地の設定に追加・変更が必要な場合には `<work root>\settings\place.md` を更新する。
- 空間、部屋の設定に追加・変更が必要な場合には `<work root>\settings\location.md` を更新する。
```

- - - -

# プロジェクト 6

- エピソードプロット（plot-c）
- プロンプトに入力する内容
  - <work root>
  - <chapter>
- 指示内容は次のコードブロック内。

``` markdown
目的：エピソードごとの概要

次のファイルを参照し、記述内容を実現するのに必要十分なエピソードプロットを創作して設定する。

- `<work root>\settings\config.md`
- `<work root>\settings\world-building.md`
- `<work root>\settings\characters.md`
- `<work root>\settings\things.md`
- `<work root>\settings\place.md`
- `<work root>\settings\location.md`
- `<work root>\plot\<chapter>\plot-a-<chapter>.md`
- `<work root>\plot\<chapter>\plot-b-<chapter>.md`

# 設定内容

- エピソード内のクライマックスに伏線を張る。
- エピソードの終わりにはフックを配置する。

# 設定の記録

- `<work root>\plot\<chapter>\plot-c-<chapter>-<episode>.md` に設定内容を記録する。
- 世界設定に追加・変更が必要な場合には `<work root>\settings\world-building.md` を更新する。
- キャラクター設定に追加・変更が必要な場合には `<work root>\settings\characters.md` を更新する。
- 物事全般の設定に追加・変更が必要な場合には `<work root>\settings\things.md` を更新する。
- 地域、土地の設定に追加・変更が必要な場合には `<work root>\settings\place.md` を更新する。
- 空間、部屋の設定に追加・変更が必要な場合には `<work root>\settings\location.md` を更新する。
```

- - - -

# プロジェクト 7

_ChatGPTへの問い合わせ：初稿で指示するか改稿で指示するか。_

_改稿の場合はすべていっぺんに行うのではなく、それぞれの処理を順番に行うよう指示する。_

- 本文
- プロンプトに入力する内容
  - <work root>
  - <chapter>
- 指示内容は次のコードブロック内。

``` markdown
次のファイルを参照し、記述内容を実現するのに必要十分かつ要綱を踏まえた本文を創作して記録する。

- `<work root>\settings\config.md`
- `<work root>\settings\world-building.md`
- `<work root>\settings\characters.md`
- `<work root>\settings\things.md`
- `<work root>\settings\place.md`
- `<work root>\settings\location.md`
- `<work root>\plot\<chapter>\plot-a-<chapter>.md`
- `<work root>\plot\<chapter>\plot-b-<chapter>.md`
- `<work root>\plot\<chapter>\plot-c-<chapter>-<episode>.md`

# 要綱

- 一文の文字数は基本的に7～25文字とする。
- 段落的なまとまりごとに全体的な一文の文字数を基本の0.7～1.5倍にする。
- 緊迫する段落的なまとまりでは一文の文字数は1～16文字を基本とする。ただしクライマックスを除く。
- 500～800文字に1回の割合で見せ場の表現を次のようにする。
  - 体言止めにする。
- 700～1100文字に1回の割合で適宜表現を次のようにする。
  - 形容詞または形容動詞で終わる。
- 500～900文字に1回の割合で重要な瞬間の表現を次のようにする。
  - 強い印象を与えない軽い比喩にする。
  - 比喩はその場の雰囲気に合う表現にする。
- 800～1200文字に1回の割合で次のようにする。
  - 使うのが不自然にならない場所で提喩にする。
  - 提喩はその場の雰囲気に合う表現にする。
- 8000～12000文字に1回の割合で次のようにする。
  - 倒置法にする。
  - 倒置法を使うのが不自然な場所は避ける。
- 10万文字につき上位10個の割合で重要なシーンの表現を次のようにする。
  - ディテールを増やして細密に描き文字数を通常の1.5倍にする。
  - 各シーンのうち最も重要な瞬間を強い印象の比喩にする。
  - 比喩はその場の雰囲気に合う表現にする。

# 本文の記録

- `<work root>\text\<chapter>\text-<chapter>-<episode>.txt` に各エピソードを記録する。

# 設定の記録

- 世界設定に追加・変更が必要な場合には `<work root>\settings\world-building.md` を更新する。
- キャラクター設定に追加・変更が必要な場合には `<work root>\settings\characters.md` を更新する。
- 物事全般の設定に追加・変更が必要な場合には `<work root>\settings\things.md` を更新する。
- 地域、土地の設定に追加・変更が必要な場合には `<work root>\settings\place.md` を更新する。
- 空間、部屋の設定に追加・変更が必要な場合には `<work root>\settings\location.md` を更新する。
```

- - - -

# プロジェクト 8

タイトル、キャッチコピー、あらすじ

指示内容は次のコードブロック内。

``` markdown
次のファイルを参照し、記述内容を実現するのに必要十分かつ要綱を踏まえたタイトル、キャッチコピー、あらすじを創作して設定する。

- `<work root>\plot\<chapter>\plot-a-<chapter>.md`
- `<work root>\plot\<chapter>\plot-b-<chapter>.md`
- `<work root>\plot\<chapter>\plot-c-<chapter>-<episode>.md`

# 要綱

- タイトル：30文字以内。
- キャッチコピー：35文字まで。
- あらすじ：500文字以内。

# 設定の記録

- `<work root>\text\<chapter>\cover.md` に設定内容を記録する。
```
