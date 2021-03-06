# 100 Days Of Code - 学習ログ

### 0、1日目: 2020年6月12日(金)

**今日の進捗**: 個人アプリのトップページ作成。サイドバーに表示させたい項目を整理し、CSSで位置を調整した。また、メインメニューのコンテンツが横２列で表示されるようにした。

**思ったこと**: ページのデザインが完成に近付くと細かい雑さが気になって修正に時間をかけてしまう。要因としては「githubにアップロードするコードをきれいにしたい」のと「今直さないと忘れてしまいそう」だからだと思われる。
手早く進むための改善案として「気になっている部分をコメントしておく。コメントしたら修正は後回しにする」という方法を試しても良いかもしれない。

**課題**: text-align:justifyでブロック要素(li)の中のテキストが均等割り付けにならなかった。検証としてliタグの中にspanタグを入れてその中にテキストを入れたり、親要素にwidthを設定してみたが均等割り付けにならず。

### 2日目: 2020年6月13日(土)

**今日の進捗**: 個人アプリのGithubで出ていた警告を確認。railsバージョンを5.2.4.2→5.2.4.3にしたりactionpack、activesupportのgemを入れて脆弱性への対処を実施。アプリ自体の進捗としてはdevise gemを入れてこれからログイン機能の実装を始める。

**思ったこと**: フロントエンドで躓いたことは一旦後回し。余裕があれば開発の調整期間で手直しをしようと思う。リソースを割く優先順位を大事に。

**リンク**: [永久保存版！？伊藤さん式・Railsアプリのアップグレード手順](https://qiita.com/jnchito/items/0ee47108972a0e302caf)

**課題**: text-align:justifyでブロック要素(li)の中のテキストが均等割り付けにならなかった。検証としてliタグの中にspanタグを入れてその中にテキストを入れたり、親要素にwidthを設定してみたが均等割り付けにならず。

### 3日目: 2020年6月14日(日)

**今日の進捗**: deviseを使用してusersテーブルを作成。アプリの設計を見直して、新規登録時に必須ではない項目を別テーブルに分けるようにした。

**思ったこと**: テーブルのカラムをdate型にする場合には「date」という単語を使用せず「_on」を使用するという命名規則を初めて知りました。「型名を名前にするのは冗長」という説明で納得。

**リンク**:
テーブルのカラム名を作成する際に参考にしたサイト↓
[モデルやメソッドに名前を付けるときは英語の品詞に気をつけよう](https://qiita.com/jnchito/items/459d58ba652bf4763820)
アプリ作成が終わったらしっかりした眼鏡を買おうと思ってブックマークしたサイト↓
[メガネに今の倍額以上を投資してマジ世界が変わった](https://techracho.bpsinc.jp/hachi8833/2016_12_21/27862)

### 4日目: 2020年6月15日(月)

**今日の進捗**: deviseを使用したユーザー新規登録機能の実装続き。新規登録画面のビューを作成(hamlのみ)。deviseでデフォルトのパラメーター以外も保存を許可するためにapplication_controllerにconfigure_permitted_parametersを追記。nicknameとbirth_on等オリジナル要素を追加した。

**思ったこと**: ユーザーの新規作成までならdeviseのコントローラー作成は不要。ここら辺はフリマアプリを作成するときの手順を覚えていたが、カリキュラムの内容を見ずに自分で調べて自身を持って進められるかというと自信がない・・。誤った操作による失敗を恐れすぎている気がシマスネ。

**リンク**: [[*Rails*] deviseの使い方（rails5版）](https://qiita.com/cigalecigales/items/f4274088f20832252374)

### 5日目: 2020年6月16日(火)

**今日の進捗**:

* 個人アプリ作業：ユーザーサインアップ画面にcss(sass)を適用。floatを使用し左右のブロック構成にした。
* 勉強：dockerとKubernetes(K8s)の概要についてYouTube解説動画やネットの記事でサクッと勉強。dockerについてはkindleで環境構築についての書籍をDLして深堀り予定

**思ったこと**: 勉強のリソース管理をもっと真面目にやらないと個人アプリ作成だけで時間がカツカツになってしまう

### 6日目: 2020年6月17日(水)

**今日の進捗**:

* 個人アプリ作業(6h)：ユーザーサインアップ画面にcss(sass)を適用。入力欄の左側に表示させているアイコンをきれいに横並びにできず苦戦。本日は断念。
* 勉強(2h)：dockerの概念をqiitaの記事で学習。「コンテナ技術」が重要なキーワード。共同開発では重要になりそうだが自分一人で開発する際には多用しそうにないので、意識して使用するようにしないと覚える機会を設けられなさそう。あと時間があれば公式ドキュメントと書籍も読みたい。

**リンク**: [【図解】Dockerの全体像を理解する -前編-](https://qiita.com/etaroid/items/b1024c7d200a75b992fc)

### 7日目: 2020年6月18日(木)

**今日の進捗**:

* 個人アプリ作業(3h):ユーザーサインアップ画面のcss(sass)適用。昨日の問題は解消。入力欄はきれいになり、ページはほぼ完成。また、mixinとcolor設定用のscssファイルも作成しリモートリポジトリへプッシュ。ただ全体のクラス設定を少しずつ変更したこともありこれだけの作業で終わってしまった。

### 8日目: 2020年6月19日(金)

**今日の進捗**:

* 個人アプリ作業(2.5h):ユーザーサインアップ画面のcss(sass)適用完成。技術的には特に新しい学びはないものの、着実にフロントエンドの経験値が貯まっていっている。まだレスポンシブ対応をしていないため、サイズの変化に弱い部分は納期に間に合わせたあとで更新予定。

### 9日目: 2020年6月20日(土)

**今日の進捗**:

* 個人アプリ作業(2h):アプリのサインアップ機能のテスト。実際にフォームに入力を行ってみて、期待通りにアカウント作成ができるか、意図しない情報を入力された時にアカウント作成ができないかテストした。結果PW入力フォームの正規表現が希望通りに動作しないことがわかったため、明日は検証と修正を実施予定。

### 10日目: 2020年6月21日(日)

**今日の進捗**:

* 個人アプリ作業(6h):アプリのサインアップ機能のテスト(RSPec)。RSPecの復習も兼ねてバリデーションを記述し、期待通りにアカウント作成ができるか、境界値によってはちゃんとアカウント作成ができなくなるかテストを実施。

**思ったこと**: RSPecでFactoryBotを使う際、createメソッドを使用したらincludeマッチャがexampleしなくなった。buildだとexampleしたことから、テスト用のDBをロールバックしたらエクスペクテーションの段階でマッチャによる検証ができなくなってしまうのかな？と予想。

### 11日目: 2020年6月22日(月)

**今日の進捗**:

* 個人アプリ作業(4h):アプリのサインアップ機能のテスト(RSPec)。サインアップ画面のすべてのカラムに対してバリデーションを実施し、すべて期待通りに動くことを確認した。

**思ったこと**: 今回テストしたパターンは登録可能・不可能パターン計26パターン。初めて自分で必要なテストを考えたため、実務では不要なテストもあったかもしれない。今後のテストはこれを基準にブラッシュアップしていく。

### 12日目: 2020年6月23日(火)

**今日の進捗**:

* 個人アプリ作業(11h):アプリのアカウント作成・ログイン機能の実装。アカウント作成フォームでバリデーション同様の入力制限がかかるようにした。また、deviseの日本語化を行い、テストも日本語のエラーメッセージに対して行われるように修正。ログイン画面も作成(サインアップ画面を踏襲)し、アカウント作成→サインアウト→ログインができるようになった。

### 13日目: 2020年6月24日(水)

**今日の進捗**:

* 個人アプリ作業(3h): ログインページはサインアップページのデザインを踏襲しているため、保守性を上げるために部分テンプレートに共通化。また、ヘッダーを作成しトップページへ戻れるようにした。

### 14日目: 2020年6月25日(木)

**今日の進捗**:

* 個人アプリ作業(2h): ヘッダーの細かい調整を実施。ロゴやリンクはヘッダーに集約し、一旦ここまでを一区切りにしてマスターブランチへマージした。

### 15日目: 2020年6月26日(金)

**今日の進捗**:

* 個人アプリ要件定義(2h): 根幹機能である記事の新規作成機能について、あらためて何をどこまで実装するか要件を精査した(非コーディング)。

### 16日目: 2020年6月27日(土)

**今日の進捗**:

* 個人アプリ要件定義(4h): 記事(問題)の作成について、今回作成する範囲の検討(非コーディング)。e-learningとしては複数パターンの問題を用意したいが、いきなりすべてのパターンを用意すると時間を取られてしまうため、今回は包括的に対応が可能な「正解が複数存在でき、作成した問題数分画面遷移する(セッションを保持)」パターンの記事が作成可能なところまで作成する。

### 17日目: 2020年6月28日(日)

**今日の進捗**:

* 個人アプリ作業(10h): 要件を定義した「問題の作成機能」をDB設計に反映(README)。Githubに問題の作成機能のブランチを作成。前準備として「contents」として作っていた部分が新しい定義では「pages」になるため、既に作成していたコントローラーを削除して「pages」コントローラーを作成しました。

### 18日目: 2020年6月29日(月)

**今日の進捗**:

* 個人アプリ設計(3h): １セッションで１Articleに複数(任意の数)Pagesを作成する設計を検討。理想は１ビューで完結することだが、未経験の課題が多いため現時点では後述の設計を採用。

1. 最初のビューでArticleと最初のPagesのレコードを作成

1. [完了(一般公開)]、[完了(非公開)]、[次のPagesを作成]の3パターンのsubmitボタンを用意する

1. [完了]では入力した項目をテーブルに保存。[次の〜]ではそのArticleのセッションを保ったまま新しいPagesのビューに遷移

1. 続けていき、最後に[完了]をしたタイミングですべてのセッションを保存する

**思ったこと**: 実装した後の方が具体的な実装の質問がしやすいため、まずは最速で実装を終えたい。そのあと改良可能であれば改良する。ここに時間をかけすぎると視野が狭くなるためそこだけ要注意。

### 19日目: 2020年6月30日(火)

**今日の進捗**:

* 個人アプリ開発(4h): 記事作成機能の実装継続。Article_id/Page_idのパスになるようルーティングをネスト。newアクションのビューを表示できるよう関連モデルのテーブル(categories,articles,pages)を作成しました。

### 20日目: 2020年7月1日(水)

**今日の進捗**:

* 個人アプリ開発(3h): テーブル作成時のエラーに躓き、解決できませんでした。エラー内容はreferences型のカラムを追加する際に元テーブルのidがbigint型だから合わせてbigintにしろというもの。マイグレーションファイルのバージョンが5.2なので元々bigint同士で作られるはずなのにそうならず、本日は終了。明日に持ち越し。

### 21日目: 2020年7月3日(金)

**今日の進捗**:

* 個人アプリ開発(6h):首の怪我のため7月2日は作業できず。今日は記事作成機能で最低限必要になるモデル(Category,Article,Page,Option)とテーブルを作成。外部キーカラムについてはreferences型にこだわらずbigint型のカラムにforeign_key :trueをつけることにした。

### 22日目: 2020年7月4日(土)

**今日の進捗**:

* 個人アプリ作業(3h):記事作成機能実装。記事作成画面のマークアップの下準備で完成画面をノートにスケッチした。

### 23日目: 2020年7月5日(日)

**今日の進捗**:

* 個人アプリ開発(6h):記事作成機能実装ブランチに派生ブランチを作成し、記事作成画面のマークアップとCSS適用をした。

### 24日目: 2020年7月6日(月)

**今日の進捗**:

* 個人アプリ開発(2h):記事作成機能のビューにcssを適用。1/3完了。

### 25日目: 2020年7月7日(火)

**今日の進捗**:

* 個人アプリ開発(1h):記事作成機能のビューにcss適用。体調が芳しくなかったため睡眠を優先した。

### 26日目: 2020年7月8日(水)

**今日の進捗**:

* 個人アプリ開発(8h):記事作成機能のビューを作成。html(haml)・css(scss)の作成はほぼ完了。明日調整をしてコミット予定。明日はブランチをマージした後サーバーサイド実装に入る。

### 27日目: 2020年7月9日(木)

**今日の進捗**:

* 個人アプリ開発(3.5h):記事作成画面のサブブランチを記事作成機能のブランチにマージするつもりが誤って記事作成機能のブランチをマスターにマージしてしまったため、git revertで打ち消し。打ち消し前のブランチで再度プルリクエストを作成し、記事作成画面のサブブランチを統合した。本日はアプリケーション完成日までの実装予定を改めてリストに落とし込み、逆算して予定を立て直した。

### 28日目: 2020年7月10日(金)

**今日の進捗**:

* 個人アプリ開発(2h):モデルファイルにdependentオプションの記載が漏れていたため追加。明日実装予定の動的一対多フォームの実装に使用予定のcocoonGemについてqiitaの記事と公式リファレンスを読んで予習し、開発工程のあたりをつけた。

### 29日目: 2020年7月11日(土)

**今日の進捗**:

* 個人アプリ作業(2h):記事新規作成機能の動的一対多フォームの実装の計画を立てた。具体的にはArticle内にpages、page内にoptionsをネストしたフォームをfields_forで作成し、pageはJSで動的に追加(新たなフォームが追加される)ように実装する。動的フォーム実装はcocoonGemを使用し、フォームはsimple_formかFormtasticを使用予定。

**思ったこと**: 記事作成機能についてはpageの作成を(sessionを保ちつつ)画面遷移で回していく方法が技術的には簡単と思われるが、問題作成の度に画面遷移するのは非常に使い勝手が悪いので動的記事作成フォームの実装にはこだわりたい。

**リンク**: [cocoon](https://github.com/nathanvda/cocoon) [箱のプログラミング日記。](https://www.y-hakopro.com/entry/2019/08/03/234126)

### 30日目: 2020年7月12日(日)

**今日の進捗**:

* 個人アプリ作業(8h):Railsで非推奨のaccepts_nested_attributes_forを使用せずにネストフォームを実装する方法を調べた。今回はフォームオブジェクトを使用した実装方法を使用してみる。また、その後に動的一対多フォーム実装が控えているため、テストが済んだらcocoonGemと共存ができそうか検証予定。

* NoCodeの概念をリサーチ(0.5h):NoCodeでWebアプリを作成するメリットとデメリットについて調べた。また、学習するためのプラットフォームやNoCodeが現在活かされている場面について調べ、自分でも活かし方を考えてみた

**思ったこと**:NoCodeは通常開発に比べWeb作成(特にモバイル)の速度の速さが最大の魅力だと思われる。その利点を活かし、NoCodeで簡易サイトを作成→それを元にクライアントに簡易サイト・通常開発の違いを説明し任意の開発手法で案件を獲得するという手法が使えるのではないかと思った(他社との提案競争にも優位になる)。

**リンク**:
[accepts_nested_attributes_forを使わずに複数リソースを同時登録する(クイズアプリを例に)](https://qiita.com/kumackey/items/b469143f1a0c4902cf4e)
[プログラミング不要のNoCode（ノーコード）とは？どうやって学習するの？](https://note.com/nocodeninja/n/n48feac237591)

### 31日目: 2020年7月13日(月)

**今日の進捗**:

* 個人アプリ作業(3h):フォームオブジェクトの実装。まずはフォームのname属性に対応させる予定のattributeをフォームオブジェクトに作成し、バリデーションはコメントアウトした上でレコード保存に成功した時の処理をフォームオブジェクトとコントローラーに記述した。

### 32日目: 2020年7月14日(火)

**今日の進捗**:

* 個人アプリ作業(3h):simple_formGemを使い、フォームをsimple_formに置き換え。NoMethodエラーを解消中。

### 33日目: 2020年7月15日(水)

**今日の進捗**:

* 個人アプリ作業(2h):ビューのフォームに対しNoMethodエラーが出ていた問題を解消。原因はform_with(simple_form_for)が受け取ったフォームオブジェクトのクラス名を対応するコントローラーのパスであると認識してしまったためと思われる。

### 34日目: 2020年7月16日(木)

**今日の進捗**:

* 個人アプリ作業(4h):フォームをsimple_formに置き換える作業続き。simple_formで置き換えたフォームでsubmitボタンにはクラス名があたるものの、selectプルダウンにクラス名があたらずcssが反映されなかった。直接関連したリファレンスはなかったためいくつか総当りで試すも本日は解決せず。

### 35日目: 2020年7月17日(金)

**今日の進捗**:

* 個人アプリ作業(3h):simple_formのselectタグにクラスを当てる方法は偶然enumを日本語化する記事に近い記法が載っていたので試したところうまくいった。
但しinputタグにはまだクラスが当たらないため、まだ試行錯誤が必要。

**リンク**:
[enumを日本語化する](https://qiita.com/sakuraniumarete/items/90d3fbaebcd5fdb31646)

### 36日目: 2020年7月18日(土)

**今日の進捗**:

* 前回の課題に対しての取り組み:simple_formのinputタグにclassを当てる場合f.input_fieldにする必要があった。これで問題は解決。

* 個人アプリ作業(4h):既存のフォームをほぼsimple_formに置き換え。categoryを入れるselectフォームには予めcategoryのseedデータを入れておかなければいけないため、準備をしました。

### 37日目: 2020年7月19日(日)

**今日の進捗**：

* 前回の課題に対しての取り組み：seedデータ作成。ancestryGemを使用した３世代構造のseedデータ作成で、単純作業が多く数も大量のため本日中に終わらず。

* 個人アプリ作業(4h)：categoryのseedデータ作成。入れ込むデータの選定や入れ方を調べ、入れ方はチーム開発時のアプリのやり方(3階層のカテゴリ名をすべて入れる)を踏襲した。理由はe-learningで記事を調べるためにカテゴリ名が仮のものだとアプリのイメージがし辛いため。

* 次の課題：seedデータ作成は本業の休憩時間などにちょこちょこ進めるのが効率が良さそうなので、月曜日に進めておく。

### 38日目: 2020年7月20日(月)

**今日の進捗**：

* 前回の課題に対しての取り組み：seedデータ作成完了。

* 個人アプリ作業(4h)：categoriesテーブルに投入するseedデータを作成。validationをかけても無事にデータ投入できました(エラーもすべて解消済み)。

* 次の課題：記事入力フォームのカテゴリ選択フォームを作成

### 39日目: 2020年7月21日(火)

**今日の進捗**：

* 前回の課題に対しての取り組み：カテゴリ選択フォーム作成・エラーに対してのトラブルシューティング

* 個人アプリ作業(1h)：記事入力フォームのカテゴリ選択フォーム(f.collection_select)にCategoryのレコードを入れたいがエラーが解消できず。

* 次の課題：エラー解消

### 40日目: 2020年7月22日(水)

**今日の進捗**：

* 前回の課題に対しての取り組み：f.collection_selectのエラーを解消

* 個人アプリ作業(1h)：categoryを選択するセレクトボックスに無事テーブルのレコードを表示させられた。

* 次の課題：

1. categoryのセレクトボックスに入れる値のロジックがビューに書かれているので最適化をする
1. ログインしているユーザーが記事を投稿できるかテストをする

### 41日目: 2020年7月23日(木)

**今日の進捗**：

* 前回の課題に対しての取り組み：categoryのセレクトボックスでルートカテゴリを選択できるようにするロジックをモデルに記載した

* 個人アプリ作業(4h)：ビューのセレクトボックス作成、enumの日本語化を実施。ネストされたフォームのレコード保存方法の調査をした。

* 次の課題：

1. フォームオブジェクトを用いたフォームのネスト方法(ビュー、コントローラー)の調査

1. ログインしているユーザーに紐付けて記事が投稿できるかテスト

### 42日目: 2020年7月24日(金)

**今日の進捗**：

* 前回の課題に対しての取り組み：フォームオブジェクトを用いてarticle,page,optionsのインスタンスを作成・テーブルに保存した。

* 個人アプリ作業(8h)：問題作成機能はインスタンスを保存するテストまではできたのであらかた完了。

* 次の課題：

1. カテゴリのセレクトボックスがルート→選択したルートのペアレント→選択したペアレントのチルドレンの順に表示されるようにする

1. 問題の選択肢が動的に追加できるようにする(cocoonGem)

### 43日目: 2020年7月25日(土)

**今日の進捗**：

* 前回の課題に対しての取り組み：カテゴリのセレクトボックスを非同期で出現させるため、jQueryを導入した。

* 個人アプリ作業(3h)：jQueryを導入。セレクトボックスを非同期で出現させる手順を復習した。

* 次の課題：カテゴリのセレクトボックスがルート→選択したルートのペアレント→選択したペアレントのチルドレンの順に表示されるようにする

### 44日目: 2020年7月26日(日)

**今日の進捗**：

* 前回の課題に対しての取り組み：セレクトボックスは未着手

* 個人アプリ作業(8h)：インスタンスの保存に失敗した時に(simple_formの)セレクトボックス(collection_select)起因のエラーが表示されることを発見。一旦セレクトボックス実装前の状態にし、まずはその他のカラムの保存に失敗した時にエラーが適切に出るようエラーメッセージを実装した。同時にエラーメッセージの日本語化を行った。

* 次の課題：エラーメッセージ表示の続き。セレクトボックス以外のフォームで引っかかったバリデーションごとに日本語のエラーメッセージが出るようにする。

### 45日目: 2020年7月27日(月)

**今日の進捗**：

* 前回の課題に対しての取り組み：未着手

* 個人アプリ作業(2h)：categoryを選択するセレクトボックスがある状態でもインスタンスの保存に失敗した時にundefined methodエラーが出ないようにしました(これが出ていると正常にバリデーションエラーが出せない)。

* 次の課題：記事投稿機能に関連するカラムのバリデーションの設計。設定方法を下調べ

**リンク**:
[collection_selectにインスタンス変数を渡すと、undefined method `map' for nil:NilClass が発生するエラー](https://qiita.com/zorori777/items/07cca6b04de125b812a0)

### 46日目: 2020年7月28日(月)

**今日の進捗**：

* 前回の課題に対しての取り組み：バリデーションとDBの制限の違いについて調査。

* 個人アプリ作業(2h)：DBのNOT NULL制約とバリデーションのrequire: trueの違いについて調査。DBでNULLを許可してバリデーションで許可しないパターン(またはその逆)も可能かもしれないが、確たる情報はすぐに出てこなかった。また、dependent: :nullifyを使用した時のみnullを許可する事は可能か調べてみたが、すぐに情報が出てこなかったため実装フェーズでテストすることにする(カテゴリーを削除してもそのカテゴリーに属する記事は消したくない)。

* 次の課題：記事(問題)投稿機能の必要カラムにバリデーションを記載。また、問題の出題形式によって記事のレイアウトが変えやすいよう出題形式のセレクトボックスをフォーム外に設置する(レイアウトを再設計)。

### 47日目: 2020年7月29日(水)

**今日の進捗**：

* 前回の課題に対しての取り組み：記事投稿機能のバリデーション記載完了。問題の出題形式によって問題のレイアウトを変えるレイアウトの設計完了

* 個人アプリ作業(4h)：プルダウンで選択した出題形式によって問題作成時のビューのレイアウトを大きく変えたいが、すべてをJSで実装するとJSタスクの粒度が大きくなりすぎてしまう懸念があるため、問題のレイアウト変更はあくまでも画面遷移で行うことにした。但し、「１ページで問題作成ができる」という表現にはこだわりたいので画面遷移をしても問題作成画面が出題形式のボックスの下に追加されるような見た目にすることにした。問題テーブルの出題形式カラムを別テーブルに分けるかどうかやルーティングは改めて考える。

* 次の課題：問題テーブルの出題形式カラムを別テーブルに分けるかどうか、ルーティングはどうするか(セッションを持たせる必要がある)検討する

### 48日目: 2020年7月30日(木)

**今日の進捗**：

* 前回の課題に対しての取り組み：未完了

* 個人アプリ作業(1h)：出題形式を先に選んでフォームを出現させる方法の選択肢とメリット・デメリットをまとめ、実装手順の想定をした。まだどのように実装するか決めかねている状況。

* 次の課題：設問の出題形式を選択してからフォームが出るようにする。

### 49日目: 2020年7月31日(金)

**今日の進捗**：

* 前回の課題に対しての取り組み：設問の出題形式を選択してからフォームが出るようにする設計完了。

* 個人アプリ作業(6h)：設問機能の設計は完了したので、今回のブランチはカテゴリーのセレクトボックスが３段階動的に追加されるところまで実装する。

* 次の課題：カテゴリーのセレクトボックスをカテゴリー３まで動的に追加する。

### 50日目: 2020年8月1日(土)

**今日の進捗**：

* 前回の課題に対しての取り組み：未達

* 個人アプリ作業(1h)：手の甲を怪我したためキーボードを打てず本日はほぼ療養。以前実装したJSの確認と実装が終わったhaml・scssファイルの(Githubへの)コミットを実施。

### 51日目: 2020年8月6日(木)

**今日の進捗**：

* 前回の課題に対しての取り組み：カテゴリーのセレクトボックスが３世代まで動的に追加される状態まで実装済み。

* 個人アプリ作業(7h)：手がほぼ完治（蜂窩織炎）したため作業再開。カテゴリーのセレクトボックスがjQueryで動的に追加されるよう実装が完了。CSSはまだ当てていないため機能のみ。

* 次の課題：カテゴリのセレクトボックスにCSSを当てて見た目を整える。

### 52日目: 2020年8月7日(金)

**今日の進捗**：

* 前回の課題に対しての取り組み：カテゴリのセレクトボックスにCSS適用

* 個人アプリ作業(1h)：CSSコード記述のみ。

* 次の課題：RSpecでバリデーションのテストを実施する。

### 53日目: 2020年8月8日(土)

**今日の進捗**：

* 前回の課題に対しての取り組み：未達成

* 個人アプリ作業(4h)：前回のセレクトボックスへのCSS適用方法を変更。前回はJSで追加されたセレクトボックスに対してCSSをあてていたが、変更後は既存のセレクトボックスにあてていたCSSがJSで追加したセレクトボックスにもあたるようにしました(CSS共通化リファクタリング)。

* 次の課題：RSpecでバリデーションのテストを実施する(継続)。

### 54日目: 2020年8月9日(日)

**今日の進捗**：

* 前回の課題に対しての取り組み：バリデーションテスト実施中(未完)。

* 個人アプリ作業(7h)：記事投稿機能の単体テスト。通常の１モデルのテストと異なり、フォームオブジェクトの３モデル分のバリデーションチェックを１ファイル(FactoryBotを含めると２ファイル)で実施中。フォームオブジェクトのテスト方法はリンクを参考にし、フォームオブジェクトに予め入れておくデータ作成(FactoryBot)は近い記事がなかったためオリジナルで実装した(現状エラーなし)。

* 次の課題：問題投稿できる場合、できない場合のテストを書く。

**リンク**：
[フォームオブジェクトのテストをRSpecで書く](https://next49.hatenadiary.jp/entry/20150503/p1)

### 55日目: 2020年8月10日(月)

**今日の進捗**：

* 前回の課題に対しての取り組み：バリデーションテスト実施中(未完)。

* 個人アプリ作業(6h)：記事投稿機能の単体テスト実施。numericalityのバリデーションで、値が空欄の際には出ているエラーMSGが文字列の際には出ず(空白のエラーMSGが出る)、現在対処法を調査中。

* 次の課題：単体テスト完了。

### 56日目: 2020年8月11日(火)

**今日の進捗**：

* 前回の課題に対しての取り組み：フォームオブジェクトの単体テスト完了。

* 個人アプリ作業(5h)：フォームオブジェクトの単体テスト終了。エラーMSGなしのバリデーションが出た原因の究明とテストのDRYにできなかった部分(letを使用しようとしたが.errorsメソッドがno methodエラーになってしまった)の原因究明ができなかったが、優先度が低いため時間をかけずそのまま進めた。

* 次の課題：コントローラーのテストを実施。

### 57日目: 2020年8月12日(水)

**今日の進捗**：

* 前回の課題に対しての取り組み：Gem導入。コントローラーテスト用のファイルを作成、RSpec実行動作確認実施。

* 個人アプリ作業(3h)：コントローラーのテストについては準備まで完了。別途テスト前に以下の問題があったため対処。
  * ログインしていない状態で問題作成機能に遷移できてしまう
  * 上記対処後、authenticate_user!メソッドによるログイン画面へのリダイレクトで遷移時のメッセージが出なかった（対応するymlが用意されていなかった）

* 次の課題：コントローラーのテストを完了させる。

### 58日目: 2020年8月13日(木)

**今日の進捗**：

* 前回の課題に対しての取り組み：コントローラーのテストでログインしている場合としていない場合で処理を分ける方法を再確認し、実装した。

* 個人アプリ作業(2.5h)：getメソッドでarticleコントローラーのnewアクションにアクセスした際にnew.html.hamlのテンプレートが呼び出されなかった問題の解消。原因はdeviseGemによってログイン時と非ログイン時で処理を分けたため、非ログイン時にnewアクションのビューが呼び出されなかったこと。対処としてcontroller_macros.rbを作成し、deviseのコントローラーのテスト用のモジュールと一緒にrails_helper.rbで読み込んだ。

* 次の課題：コントローラーのテスト完了。

### 59日目: 2020年8月14日(金)

**今日の進捗**：

* 前回の課題に対しての取り組み：フォームオブジェクトに対してbe_a_newマッチャが使用できない問題の対処。

* 個人アプリ作業(3h)：RSPecを用いたコントローラーの検証継続。articleコントローラーのnewアクションにフォームオブジェクトであるFormArticle.newを渡していることをbe_a_newマッチャで検証したところ「undefined method `new_record?'」エラー。仮説として、フォームオブジェクトはモデルインスタンスではないためbe_a_newマッチャでの検証はできないと思われる。代替案としてbe_an_instance_ofマッチャで同一クラスかどうかを検証した。

* 次の課題：コントローラーのテスト完了。

**リンク**：[Github/rspec](https://github.com/rspec/rspec-rails) ／ [Ruby on Rails、RSpecを使ってコントローラのテストを書いてみる](https://naichilab.hatenablog.com/entry/2016/01/19/011514) ／ [rspecについてまとめてみました](https://qiita.com/ea54595/items/459727ea8c32fed48b50#%E5%90%8C%E4%B8%80%E3%82%AF%E3%83%A9%E3%82%B9%E3%81%8B%E7%A2%BA%E8%AA%8D)

### 60日目: 2020年8月15日(土)

**今日の進捗**：

* 前回の課題に対しての取り組み：createアクションの変数検証についてのエラー解消

* 個人アプリ作業(4h)：createアクションで定義している@form_article(フォームオブジェクトの新規インスタンス)の中身の検証。検証対象にするインスタンス（パラメーター）はシンボル型にしないといけないため、build(:form_article)でFactoryBotをそのまま使用するとエラーが出た。対処法を検証中。

* 次の課題：エラーの回避策を検証、テスト完了。

### 61日目: 2020年8月16日(日)

**今日の進捗**：

* 前回の課題に対しての取り組み：フォームオブジェクトのパラメーター(FactoryBot)をPOSTメソッドで送ろうとした時にエラーが出る問題の解消。

* 個人アプリ作業(3h)：FactoryBotで作成したフォームオブジェクト(form_article)のパラメーターだけをPOSTメソッドで送る場合は「オブジェクト名: attributes_for(:FactoryBotの定義名)」のように指定すればエラーが出ずにパラメーターが送れました。

* 次の課題：コントローラーのテスト完了。

**リンク**：[FactoryBot(FactoryGirl)チートシート](https://qiita.com/morrr/items/f1d3ac46b029ccddd017#%E3%83%95%E3%82%A1%E3%82%AF%E3%83%88%E3%83%AA%E3%81%AE%E7%94%9F%E6%88%90)

### 62日目: 2020年8月17日(月)

**今日の進捗**：

* 前回の課題に対しての取り組み：テスト時のエラー解消。

* 個人アプリ作業(6h)：form_articleの値を保存する際に外部キーのcategoryのidがないことでバリデーションエラー。categoryは本来seedで最初から入っているため、今回検証に使うidのカテゴリーのみcreateしてエラー回避(テストの場合seedのようにテストデータを予め作成するのは好ましくないため)。

* 次の課題：コントローラーのテスト完了。

### 63日目: 2020年8月18日(火)

**今日の進捗**：

* 前回の課題に対しての取り組み：コントローラーのテスト完了。

* 個人アプリ作業(7h)：

1. コントローラー単体テスト：コントローラーでログイン時・非ログイン時の動作テスト完了。ログイン時はform_articleの保存に成功した場合としなかった場合の動作が意図通りかテストし、想定通りになったことを確認。

1. フィーチャスペックのテスト(統合テスト)：capybaraGemを使用し、ログインから記事投稿までをテストする予定。まずは基本的な流れをおさらいした。

* 次の課題：フィーチャスペックでログインから記事投稿完了までをテストする。

### 64日目: 2020年8月19日(水)

**今日の進捗**：

* 前回の課題に対しての取り組み：フィーチャスペック実施

* 個人アプリ作業(2h)：フィーチャスペックの概要(基本の構文)を確認し、テストする項目を洗い出した。

* 次の課題：フィーチャスペックテスト実施。

### 65日目: 2020年8月20日(木)

**今日の進捗**：

* 前回の課題に対しての取り組み：フィーチャスペックテスト内容記述。

* 個人アプリ作業(2h)：フィーチャスペックのテスト内容を一通り記述。非ログイン状態でトップページから記事投稿をする流れをテスト。記事投稿時にカテゴリのプルダウンが選択できない(プルダウン内に指定した値がない)エラーが発生。解消中。

* 次の課題：エラー解消。

### 66日目: 2020年8月21日(金)

**今日の進捗**：

* 前回の課題に対しての取り組み：エラー解消作業

* 個人アプリ作業(4h)：フィーチャスペックでカテゴリのプルダウンが選択できなかった理由はテスト環境のDBにカテゴリの中身が用意されていなかったため。中身を用意するにあたり構築方法が開発環境とは異なるため、FactoryBotでancestryカラムを持ったレコードを用意する際のナレッジを調べた。

* 次の課題：FactoryBotでカテゴリを用意してフィーチャスペック再開。可能であれば単体テスト(モデル・コントローラー)の内容も修正する。

**リンク**：[ancestryカラムを持ったFactoryの作り方](https://qiita.com/ratovia/items/a27ef84b8bb118fe7647)

### 67日目: 2020年8月22日(土)

**今日の進捗**：

* 前回の課題に対しての取り組み：FactoryBotでカテゴリデータ作成

* 個人アプリ作業(4h)：リンク記事通りカテゴリのFactory内にancestryの３世代をcreateできず(createがfactory内でundefined methodになる)。解決策を模索中。

* 次の課題：FactoryBotでカテゴリのテスト用レコードを用意する。

### 68日目: 2020年8月23日(日)

**今日の進捗**：

* 前回の課題に対しての取り組み：RSPecのテストデータの投入方法調査。

* 個人アプリ作業(6h)：RSPecでテストデータを入れる方法を調査。基本テストにおいてseedを使用することは推奨されないようだが、今回のフィーチャスペックのカテゴリデータに限ってはseedを許容することにした。

* 次の課題：testにseedを入れる具体的な操作の確認、seedを入れた上で改めてフィーチャスペックテスト続行。

### 69日目: 2020年8月24日(月)

**今日の進捗**：

* 前回の課題に対しての取り組み：test環境用のseedファイルを作成

* 個人アプリ作業(3h)：テスト用のseedファイルはそれ以外のseedファイルと分け、テスト単体で使用できるようにした。具体的な読み込み方法については参考記事の情報が古いため一次情報も確認しながら実装予定。

* 次の課題：テスト環境にseedを読み込ませてフィーチャスペックでプルダウンが検証できるかテストする。

**リンク**：[RSpecで、ロード時にデータベースをシードする方法は？](https://www.it-swarm.dev/ja/ruby-on-rails/rspec%E3%81%A7%E3%80%81%E3%83%AD%E3%83%BC%E3%83%89%E6%99%82%E3%81%AB%E3%83%87%E3%83%BC%E3%82%BF%E3%83%99%E3%83%BC%E3%82%B9%E3%82%92%E3%82%B7%E3%83%BC%E3%83%89%E3%81%99%E3%82%8B%E6%96%B9%E6%B3%95%E3%81%AF%EF%BC%9F/972754901/)

### 70日目: 2020年8月25日(火)

**今日の進捗**：

* 前回の課題に対しての取り組み：RSPecでテスト用seedの読み込み

* 個人アプリ作業(2h)：テスト用seedファイル(カテゴリデータ)をフィーチャスペックで使用するspecファイルのみで読み込みをすることに成功。レコードの重複もないことを確認。但し、カテゴリのプルダウンリストはルートカテゴリを選択してもペアレントカテゴリが出現しない(IDが存在しない)状態。1〜3秒ほどテストをsleepさせても同じ状況。問題の解決方法を模索中。

* 次の課題：カテゴリのプルダウンを３世代すべて選択可能にする。

### 71日目: 2020年8月26日(水)

**今日の進捗**：

* 前回の課題に対しての取り組み：フィーチャスペックでJSのプルダウンが表示されない問題の調査。

* 個人アプリ作業(3h)：jQueryで出現するプルダウンがフィーチャスペックで認識できない問題の原因を調査。capybaraGemのテスト実行環境(ヘッドレスブラウザ)が標準だとJSに対応していない(Rack::Test)事が原因だった。調査情報を元にJS: trueにしたものの、プルダウンの要素(ID)が検索できないため、さらに追加調査が必要。

* 次の課題：カテゴリプルダウンのセレクトボックスを変更できるようにする。

**リンク**：[【capybara】JavaScriptで生成されたselectタグを選択することができない](https://teratail.com/questions/244610)、[【Rails】JavaScriptが絡むテスト](https://qiita.com/koki_73/items/ffc115ed542203161cef)、[Capybaraチートシート](https://qiita.com/morrr/items/0e24251c049180218db4#%E8%A6%81%E7%B4%A0%E3%82%92%E6%A4%9C%E7%B4%A2%E3%81%99%E3%82%8Bcapybaranodefinder)

### 72日目: 2020年8月27日(木)

**今日の進捗**：

* 前回の課題に対しての取り組み：統合テスト完了

* 個人アプリ作業(5h)：フィーチャスペックのテストが通ることを確認。テストコードがうまく動いているか確認する方法の一つとして、コード内にスクリーンショットを撮るコマンドを入れ込むデバッグ方法を実践。

* 次の課題：プルリクエスト内のコード修正。masterブランチにマージ。

### 73日目: 2020年8月28日(金)

**今日の進捗**：

* 前回の課題に対しての取り組み：コンフリクトの解消

* 個人アプリ作業(2h)：コンフリクトを解消して記事投稿機能のブランチをマスターブランチにマージ。コンフリクト解消時のコミット一覧にコンフリクトしていないように見えるファイルがあり、プッシュすると進行状況がmaster相当のほうになると思ったものの試しにマージしたらやはりmaster相当になってしまった。対処としてgit revertしてからブランチをマージした。

* 次の課題：問題回答機能の実装開始。

### 74日目: 2020年8月29日(土)

**今日の進捗**：

* 前回の課題に対しての取り組み：問題購入機能のブランチ・プルリクエストを作成

* 個人アプリ作業(4h)：問題回答機能を実装するために、問題を購入する機能を先に実装することにした。まずは購入する対象の設問をトップページに表示させるために設問のseedデータを作成(rake db:seedは未実施)。

* 次の課題：db:seedコマンドでエラー無くseedデータがDBに保存されるようにする。登録された設問がトップページに一覧表示されるようにする。

### 75日目: 2020年8月30日(日)

**今日の進捗**：

* 前回の課題に対しての取り組み：設問seedデータ作成

* 個人アプリ作業(3h)：設問のseedデータ作成。seedファイル全体もseedデータが重複作成されないよう改良した。また日本語化したfakerを使用し、日本語でダミーデータが作成されるようにした。

* 次の課題：seedの設問がトップページに表示されるようにする。

### 76日目: 2020年8月31日(月)

**今日の進捗**：

* 前回の課題に対しての取り組み：トップページのデザイン再考

* 個人アプリ作業(4h)：トップページに設問のカテゴリを表示させるデザインを再考。以下を検討予定

1. ログイン時・非ログイン時のデザイン(html)
1. カテゴリの３世代は１ページで一覧から選べるようにするか画面遷移させるか

* 次の課題：トップページのhaml実装

### 77日目: 2020年9月1日(火)

**今日の進捗**：

* 前回の課題に対しての取り組み：トップページのデザイン検討

* 個人アプリ作業(1h)：ルートカテゴリを選択したら配下のカテゴリの一覧が出る動きを画面遷移無しで実現できないか見た目のアイデア出し。一旦シンプル指向にしていくことにした。

* 技術調査(1h)：Reactについて概要を調査。Railsアプリのフロントエンドで使用することを想定し、webpackerというGemがあることがわかった。また、webpackerはRails6.0以降は標準搭載されているため、Rails学習と並行して進めていけそう。

* 次の課題：トップページのhaml変更、scss置き換え

### 78日目: 2020年9月2日(水)

**今日の進捗**：

* 前回の課題に対しての取り組み：トップページのから設問購入までのルーティング設計。トップページ変更用のブランチ作成。

* 個人アプリ作業(2h)：トップページデザインの検討の結果、ルーティングから見直すことにした。トップページはカテゴリコントローラーのindexアクションにし、ログインなしでも設問一覧が見られるように工夫。ログイン後は使用頻度が高いと思われる機能(購入した問題)のビューへ遷移するように設計した。

* 次の課題：トップページのビュー変更を完成させる。

### 79日目: 2020年9月3日(木)

**今日の進捗**：

* 前回の課題に対しての取り組み：トップページのビュー再構成（途中）

* 個人アプリ作業(5h)：トップページのビューを再構成するにあたり、構成要素のヘッダーとサイドメニューを別ファイルに切り出し(hamlは部分テンプレート、scssファイルは機能を切り分けてインポート)。scssファイルのディレクトリ構成もコントローラーごとに分別し、baseファイルでimportさせた。また、categoriesコントローラーを作成し、indexビューがrootパスになるようにした。

* 次の課題：非ログイン時のトップページのフロント部分を作成。可能であればログイン時のトップページも作成。

### 80日目: 2020年9月4日(金)

**今日の進捗**：

* 前回の課題に対しての取り組み：haml・scssファイルファイル整理

* 個人アプリ作業(3h)：トップページのサイドメニューをログイン時メニューではなく(非ログイン時も使える)ルートカテゴリの一覧に変更。サイドバーが２種類になるため、サイドバーのscssを１つのscssファイルにまとめ、中身をmixinで共通化した。

* 次の課題：メイン画面のhamlを今回の変更に合うように変更する。

### 81日目: 2020年9月5日(土)

**今日の進捗**：

* 前回の課題に対しての取り組み：トップページに表示するデータの取得方法を調査、トップページの横並び要素の仕様変更方法の調査。

* 個人アプリ作業(5h)：非ログイン時のトップページのメイン画面を作成(途中)。メイン作業は以下の２つ

1. メイン画面で使用するカテゴリの２世代目だけをDBから取り出す方法はないか調査
1. サイドバーとメイン画面の位置関係をfloat以外の方法で再現する方法の調査

調査結果

1. カテゴリのancestryカラムで「整数」という条件でレコードを抽出する方法はHITせず
1. 定番だがflexboxが良さそう

* 次の課題：調査結果をもとに以下のように実装予定

1. メイン画面にはカテゴリの２世代目をすべて表示させず、代わりの画面を実装する(未定)
1. flexboxにサイドバーとメイン画面を入れて横並びにする

### 82日目: 2020年9月6日(日)

**今日の進捗**：

* 前回の課題に対しての取り組み：トップページのビューに何を表示させるか検討。サイドバー・メイン画面をflexbox内に配置。

* 個人アプリ作業(4h)：やることが決まっているflexbox化はすぐに実施。トップページの内容については時間がかかってしまい今日中には決まらず。個人開発の一番の難所。

* 次の課題：トップページ作成。ユーザーログイン→カテゴリ一覧ページまでの動線を作成。

### 83日目: 2020年9月7日(月)

**今日の進捗**：

* 前回の課題に対しての取り組み：トップページ作成(仮置)。カテゴリ一覧表示作成(途中)

* 個人アプリ作業(4h)：トップページは暫定で仮置。新着の問題と多く解かれている問題を設置予定。サイドバーでルートカテゴリを選択したらshowアクションが呼ばれてメイン画面にparentカテゴリとchildrenカテゴリが表示されるようにした。

* 次の課題：childrenカテゴリを選択したらchildrenカテゴリの設問一覧が表示されるようjQueryを作成する。

### 84日目: 2020年9月8日(火)

**今日の進捗**：

* 前回の課題に対しての取り組み：時間が足りずjQueryは作成できず。すぐできることとして以下を実施。

1. 9/7までのコミットをリモートリポジトリにプッシュした際にsiderから指摘があったコードの修正
1. categoryモデルのロジックリファクタリング

* 個人アプリ作業(2h)実施：

1. siderの指摘でルーティングでrootに指定したアクションは重複してroutes.rbに再定義しなくても良いことに気付いた。また、siderでもアクティブレコードはコントローラーに書くよう指摘があったためそのように修正。
1. categoryモデルにancestryがrootのレコードを抽出するロジックを作っていたが、最初からrootsというメソッドが用意されていたためロジックを削除して置き換えた。

* 次の課題：jQueryで選択したカテゴリの設問一覧が表示されるようにする。

### 85日目: 2020年9月9日(水)

**今日の進捗**：

* 前回の課題に対しての取り組み：categories#showのビューをhamlで作成。

* 個人アプリ作業(4h)：jQueryで非同期にする予定のhtmlを一旦hamlファイルで作成。明日それを元にjsファイルを作成予定。

* 次の課題：jQueryで選択したカテゴリの設問一覧が表示されるようにする。

### 86日目: 2020年9月10日(木)

**今日の進捗**：

* 前回の課題に対しての取り組み：haml再修正

* 個人アプリ作業(4h)：jQuery作成中、設問の問題文にはタイトルが無いことに気付き、haml修正（一覧ページで問題文１つあたりのタイトルを表示させるようなビューにしていたため）。

* 次の課題：修正したhamlに対応するようなjQueryの作成。

### 87日目: 2020年9月11日(金)

**今日の進捗**：

* 前回の課題に対しての取り組み：アコーディオンメニューの実装(途中)。

* 個人アプリ作業(3h)：子カテゴリをクリックするとそれに属する設問が表示されるアコーディオンメニューを実装。現在は同じクラス名の要素がすべて展開されてしまうため、指定の仕方を工夫する必要がある。

* 次の課題：アコーディオン修正完了。親カテゴリクリックで子カテゴリとそれに属する設問一覧が表示されるjQuery実装。

### 88日目: 2020年9月12日(土)

**今日の進捗**：

* 前回の課題に対しての取り組み：アコーディオンメニュー完成。親カテゴリクリックで子カテゴリとそれに属する設問一覧が表示されるjQuery実装。

* 個人アプリ作業(5h)：アコーディオンメニューの問題修正。「this」で取得した要素の.next要素をslideToggleで表示させたいので、.clickの対象要素をそれに合うクラスに変更したところ問題なくアコーディオン表示ができた。設問一覧表示までのjQueryは大まかに分けると「クリックした親カテゴリ名がメインページ下半分に表示され」「その親に属する子カテゴリバーが表示され」「子カテゴリに属する設問一覧が表示される」動きになる。一旦フリーハンドですべてコードを作成したが実行するとfailしたため、明日はエラー解消がメインになる。

* 次の課題：jQueryエラー解消。

### 89日目: 2020年9月13日(日)

**今日の進捗**：

* 前回の課題に対しての取り組み：jQueryエラー解消

* 個人アプリ作業(7h)：jQuery(jsファイル)からコントローラーに送られたdivタグ内のテキストの前後に改行が入る問題は「$(this).text().trim()」のようにtrimを入れることで解消。次はコントローラーで定義されたインスタンス変数が適切にjbuilderでJSON形式に変換できない問題の解消。インスタンス変数を２つ使用したかったので、それぞれをjbuilderで入れ子にすることで問題を解消。jQueryのdoneで引数になっているデータレコードのhas_many関係にあるレコードをcategory.articlesとして取り出そうとしたが取り出せず。次回はこちらの問題の解消予定。

* 次の課題：jQueryでクエリメソッドが使用できない問題の解消。

**リンク**：[【Rails】jbuilderの使い方辞典〜メソッドの文法と使い方がすぐわかる](https://pikawaka.com/rails/jbuilder)

### 90日目: 2020年9月14日(月)

**今日の進捗**：

* 前回の課題に対しての取り組み：親カテゴリのリンククリック後の動作をhamlで実装。

* 個人アプリ作業(6h)：親カテゴリをクリックした後に画面下に子カテゴリ一覧が表示される動きは、子カテゴリに属している設問一覧の表示がjQueryで実装困難であることから画面遷移するように仕様変更した。ルーティング、haml作成、コントローラーで変数定義、scss適用まで完了。

* 次の課題：アコーディオンメニュー(article)の中身をDBから呼び出して表示できるようにする。

### 91日目: 2020年9月15日(火)

**今日の進捗**：

* 前回の課題に対しての取り組み：UX向上、showアクションにもアコーディオンメニュー(article)を追加。

* 個人アプリ作業(2h)：本来はroot→parent→childrenの順番にカテゴリを選択する必要があるところを、rootカテゴリを選択しただけで最初のparentカテゴリのchildrenがアコーディオンメニューに表示されるようにした。これにより、無意識に感じる「article選択までには３回カテゴリをクリックしなければいけない」という心理的抵抗を軽減させた。

* 次の課題：article購入機能の実装or仮置トップページのビューを変更。

### 92日目: 2020年9月16日(水)

**今日の進捗**：

* 前回の課題に対しての取り組み：仮置のトップページを作成

* 個人アプリ作業(2h)：新着articles一覧が表示されるだけのトップページを作成しフロントエンドのブランチを終了。

* 次の課題：article購入機能の実装。

### 93日目: 2020年9月17日(木)

**今日の進捗**：

* 前回の課題に対しての取り組み：開発アプリ変更

* 要件定義・設計(8h)：開発中アプリの機能が多すぎてまだ期間が大幅にかかりそうなので、機能を限定した新アプリの開発に着手。SNS(Twitterを予定)上の情報の信頼性を上げるためのツールを開発予定。類似サービスは今のところ見当たらないことと、機能要件はあらかた定義できたので明日から設計に入る予定。

* 次の課題：アプリ設計。使用技術の選定からDB設計、タスクへの落とし込み。

### 94日目: 2020年月18日(金)

**今日の進捗**：

* 前回の課題に対しての取り組み：技術選定、タスクの落とし込み

* 個人アプリ作業(7h)：サービス名は暫定で「evi-source」。まずはRailsを使用したWebアプリとして作成予定。Twitterの発言の根拠を示す際に「evi-source」で作ったURLをつぶやきに含める使い方をする。示せる根拠は「情報源(URL・画像・文章)」「何次情報なのか」「いつの情報か」等７種。

* 次の課題：DB設計

### 95日目: 2020年9月19日(土)

**今日の進捗**：

* 前回の課題に対しての取り組み：アプリ新規作成。ER図作成。DB設計。

* 個人アプリ作業(8h)：アプリをrails newで作成。テスト関連の初期設定とコードレビュー設定(sider/rubocop)、プルリクエストテンプレート作成、ER図をdraw.ioで描画、READ MEにDB設計を記載。

* 次の課題：エビデンス入力フォーム、表示画面作成

### 96日目: 2020年9月20日(日)

**今日の進捗**：

* 前回の課題に対しての取り組み：アプリの日本語化。モデル・DB作成。

* 個人アプリ作業(4h)：日本語のlocalesファイルを用意し、アプリを日本語化。メイン機能(Post・Evidence)モデル・DBを作成。

* 次の課題：トップページのビュー作成。プルリクエストマージ。

### 97日目: 2020年9月21日(月)

**今日の進捗**：

* 前回の課題に対しての取り組み：トップページのビュー作成

* 個人アプリ作業(4h)：トップページ(evidences#new)のhamlファイル・scssを作成。今後cocoonGemを使うためにsimple_formを使用しているため、仮置のhamlでもDBを作成し、カラムに紐付いた入力フォームを作成した。また、cocoonを使用する関係であえてネストしたフォームにフォームオブジェクトは使わずにaccepts_nested_attributes_forを使用した。

* 次の課題：実際に入力フォームに入力したデータがDBに保存できるかテスト。

### 98日目: 2020年9月22日(火)

**今日の進捗**：

* 前回の課題に対しての取り組み：フォームの動作テスト、プルリクエストマージ、公開用READ ME作成

* 個人アプリ作業(4h)：フォームはエラーを解消して無事にデータが保存できたことを確認。ブランチは終了しマスターブランチにマージ。

* 次の課題：エビデンス表示画面(evidences#show)を仮置から本番に変更

### 99日目: 2020年9月23日(水)

**今日の進捗**：

* 前回の課題に対しての取り組み：Twitter埋め込み方法の検討

* 個人アプリ関連作業(3h)：Twitterに投稿したつぶやきを埋め込み表示で表示させる技術をパターンごとに下調べ。今回はTwitterのoEmbed APIでツイートURLから埋め込み用フォーマットを取得する方法を調べた。

* 次の課題：evidences#showのビュー作成

### 100日目: 2020年9月24日(木)

**今日の進捗**：

* 前回の課題に対しての取り組み：evidences#showのビュー作成

* 個人アプリ作業(5h)：showアクションのビューを作成。Twitterの投稿内容１つに対し、エビデンスがテーブル形式で表示されるレイアウトにした。

* 次の課題：ビュー作成のブランチをマスターにマージ

### 101日目: 2020年9月25日(金)

**今日の進捗**：

* 前回の課題に対しての取り組み：evidences#showのビュー調整

* 個人アプリ作業(4h)：enumでDB保存されているデータをビューに表示させる時の表示を日本語化(「_i18n」を最後につける)。localesファイルのフォーマットで日付表示を変更、URLが入るブロック要素を折り返すようにcssでword-breakを設定した。

* 次の課題：ビューを最終調整し、ブランチをマスターにマージ。デプロイ作業。

### 102日目: 2020年9月26日(土)

**今日の進捗**：

* 前回の課題に対しての取り組み：ブランチのマージ、アプリケーションのデプロイ準備

* 個人アプリ作業(8h)：showアクションのビューを作成したブランチをmasterにマージ。ec2インスタンスの環境設定を初めから実施したものの、アプリケーションサーバーのunicornの起動でエラーが出たため作業が一旦中断。

* 次の課題：環境構築＆デプロイ

### 103日目: 2020年9月27日(日)

**今日の進捗**：

* 前回の課題に対しての取り組み：unicornエラー解消、webサーバー(Nginx)設定。

* 個人アプリ作業(3h)：unicornが起動できないエラー解消。起動できなかった原因はunicorn.rbをおいていた場所がconfig直下ではなくassets/config直下だったため。その後webサーバーのNginx経由でRailsにアクセスできるよう導入と環境設定を実施。

* 次の課題：アプリが自動デプロイされるようcapistranoを導入する。

### 104日目: 2020年9月28日(月)

**今日の進捗**：

* 前回の課題に対しての取り組み：Capistranoを使用した自動デプロイ

* 個人アプリ作業(2h)：自動デプロイツールのCapistranoを導入。設定は２回目なので特に問題なく設定は完了、自動デプロイが可能になった。

* 次の課題：本番環境の動作確認。問題があれば修正。

### 105日目: 2020年9月29日(火)

**今日の進捗**：

* 前回の課題に対しての取り組み：本番環境での投稿テスト、表示崩れ解消。

* 個人アプリ作業(2h)：本番環境の目立つ問題としてヘッダーの画像が表示されない問題があったため参照方法を変更(asset_pathメソッドを使用)。また、本番環境でエビデンスの投稿が問題なくできることをテストした。

* 次の課題：エビデンス投稿にバリデーションを設定。

### 106日目: 2020年9月30日(水)

**今日の進捗**：

* 前回の課題に対しての取り組み：バリデーション設定

* 個人アプリ作業(3h)：evidenceモデルにバリデーション記載。情報ソースにpresence: true設定をした以外は特にバリデーションをかけず。アプリの特性上自由記載をさせたい項目が多いため、こちらについては文字数などは改めて考える。enumについてはバリデーションをかけなくても不正な値に対してはエラーが出てくれるようだがinclusionをかけることもできるためここはテストで挙動を確認する。

* 次の課題：モデルテスト・統合テスト実施。状況によってはバリデーション内容を変更する。

### 107日目: 2020年10月1日(木)

**今日の進捗**：

* 前回の課題に対しての取り組み：単体テスト(モデル)ファイル記載。

* 個人アプリ作業(2h)：エビデンス最終更新日が未来だとおかしいので、未来だった場合はバリデーションで弾くためのロジックを考えた。逆パターンでオリジナルのバリデーションを作成している記事を見つけたため参考にする。

* 次の課題：日付のバリデーション設定、単体テスト、コントローラーのテスト、統合テスト実施

**リンク**: [Railsで過去の日付(date)に対するバリデーション（日付の比較）](https://qiita.com/Kiichiro-T/items/8334e4e187d5ab236624)

### 108日目: 2020年10月2日(金)

**今日の進捗**：

* 前回の課題に対しての取り組み：日付のバリデーション記述、バリデーションエラーメッセージ表示

* 個人アプリ作業(3h)：記事を参考にオリジナルのバリデーションを作成。テストを実施。presence: trueのカラムで値がnilの時にバリデーションのエラーメッセージが出なかったため原因究明。エラーメッセージを表示させるためのhamlファイルを作成し、実際のフォームでエラーが出た時にどのようにエラーが出るか確認した。まだ原因の究明には至らず。

* 次の課題：バリデーションエラー解決。

### 109日目: 2020年10月3日(土)

**今日の進捗**：

* 前回の課題に対しての取り組み：モデルの単体テスト終了

* 個人アプリ作業(3h)：テスト時にバリデーションのエラーメッセージが出なかった理由はエラーメッセージを表示させるカラムをエラーが出ていないカラムに指定していたためだった。原因がわかり適切にモデルの単体テスト終了。

* 次の課題：コントローラーのテスト、統合テスト

### 110日目: 2020年10月4日(日)

**今日の進捗**：

* 前回の課題に対しての取り組み：コミットをリモートリポジトリへプッシュ、i18nのymlファイルの整理

* 個人アプリ作業(4h)：単体テストのコミットをリモートリポジトリにもプッシュ。日本語化で使用しているymlファイルが１つだけだと可読性が悪いため、モデルに関連するymlファイルとsimple_formに関連するymlファイルを大元のja.ymlから分けて管理するようにした。

* 次の課題：バリデーションメッセージのビューへの表示(CSS適用)。コントローラーのテスト・統合テスト

### 111日目: 2020年10月5日(月)

**今日の進捗**：

* 前回の課題に対しての取り組み：コントローラーのテスト開始

* 個人アプリ作業(3h)：RSpecでコントローラーのテスト。newアクションでPostモデルにaccepts_nested_attributes_forでネストされたevidenceモデルをbuildしているのでその動きをテストする書き方を参考記事を元に学習予定。

* 次の課題：コントローラーのテスト完了。統合テスト開始。

**リンク**: [[Rails]accepts_nested_attributes_forの使い方](https://qiita.com/seimiyajun/items/dff057b3eb40434d5c27#rspec)

### 112日目: 2020年10月6日(火)

**今日の進捗**：

* 前回の課題に対しての取り組み：コントローラーのテスト(RSpec)

* 個人アプリ作業(6h)：RSpecでevidencesコントローラーのアクションをテスト。newアクションでインスタンス変数と画面遷移のテストが完了。createアクションではaccepts_nested_attributes_forでネストしたフォーム(Post→Evidence)の子モデル(Evidence)だけ保存されない現象が発生。対応中。

* 次の課題：子モデルが保存されない現象のトラブルシューティング

### 113日目: 2020年10月7日(水)

**今日の進捗**：

* 前回の課題に対しての取り組み：コントローラーのテスト(RSpec続き)

* 個人アプリ作業(5h)：accepts_nested_attributes_forのフォームの子モデルが保存されない問題はテストの記述方法を大きく変え、既に保存ができているやり方(参考リンク)を踏襲することで保存ができた。但し、インスタンスにenumの値が入っているとArgumentErrorが出るため、こちらにも対処が必要。

* 次の課題：enumのカラムが保存できない現象の対処。

**リンク**:[fields_forで子テーブルのデータを一気に作成する（テストも書いてます）[Rails][Rspec]](https://qiita.com/tanutanu/items/c82c1ed2f5fa78a58366)

### 114日目: 2020年10月8日(木)

**今日の進捗**：

* 前回の課題に対しての取り組み：コントローラーのテスト完了

* 個人アプリ作業(4h)：createアクション成功時のリダイレクト先をshowに設定。単純に「:show」だとリダイレクトしないため、「evidence_path(assigns(:post).id)」のようにした。enumのカラムにFactoryBotで数字を入れているとエラーが出た問題の原因はenumが「モデルで対応する番号に変換する」ため。FactoryBotではフォーム入力時と同じ表記を踏襲する必要があるため、enumに対応した文字列の方をFactoryBotのデータにした。

* 次の課題：フィーチャスペック（統合テスト）

### 115日目: 2020年10月9日(金)

**今日の進捗**：

* 前回の課題に対しての取り組み：フィーチャスペックテスト実施。

* 個人アプリ作業(3h)：フィーチャスペックテストでフォームの投稿とPost・Evidenceテーブルの保存がうまくできているかテスト実施。ほぼエラーなく完了。

* 次の課題：開発環境の投稿フォームの表示崩れ解消。

### 116日目: 2020年10月10日(土)

**今日の進捗**：

* 前回の課題に対しての取り組み：simple_formの表示崩れの原因究明。

* 個人アプリ作業(4h)：simple_formで入力必須にしたフィールドの表示が崩れた原因を究明。simple_formは入力必須にするとタグ構成が変化する可能性があるため、この部分に対する対処が必要。

* 次の課題：simple_formのタグ構成が変わっても表示が崩れないようcssを調整。

### 117日目: 2020年10月11日(日)

**今日の進捗**：

* 前回の課題に対しての取り組み：simple_formの表示崩れの解消。プルリク終了。

* 個人アプリ作業(3h)：simple_formで必須カラムに出ていたabbrタグをsassのdisplay: noneで非表示化。必須でも必須じゃなくても同じsassがあたるようにクラス名指定を外してタグのみでsassがあたるように変更した。これでバリデーションとテストのブランチ完了。

転職活動に入るため100DaysOfCodeは終了。
