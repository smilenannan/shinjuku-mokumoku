# <name_or_handle>

## 会社や業務で普段やっていること

BIや機械学習のモデル作成などやってます。

## 今日取り組むこと

fastText（Facebookの自然言語処理API）を触って、教師ありテキストをラベリング
（前回は教師twitterだったので別のもので正解率など見てみる）

## (option) 相談するかもしれないこと

今日はローカルですが、最近、業務ではGCPのVMに環境構築して使ってるので、
そこらへん詳しい人がいたらいろいろ聞きたいです。。。（GCP初心者なので）

## (option) 得意とすること・教えられること

データ分析、統計、機械学習まわりなど多少は

## やったこと

- 各著者に対するファイル作成（1〜3繰返し）。コーパス数：30〜100万
	1.テキストファイル読み込み
	2.前処理（整形,わかちがき,label情報付与）
	3.ファイル作成
- モデル作成
- 各著者に対するテストデータ生成と予測値追加（1〜4繰返し）。サンプル数：1000件
	1.テキストファイル読み込み
	2.前処理（整形,label情報付与）
	3.データ生成
	4.予測値生成しデータに追加
- 各著者の正解率を算出

## 結果

- 正解率は著者によってかなりばらつきがある（全体の正解率は57%程度）
	- そもそも分類が難しい著者がいるらしい（だれだか忘れてしまった）
	- ハッカソンの1位は70%くらいだった（気がする）ので、著者の取捨選択を適切に行えば、同じくらいの正解率は出せるかも
- 今回はコーパス数が大きいが、モデル生成自体は数十秒で完了した
- fastText単体で使用するのではなくfasttextベースの文書ベクトル作成＋DL or MLなどで速度を担保しつつ精度を上げることができそう（な気がする）

