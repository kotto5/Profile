問1-2) 問1-1で該当する選択肢がない場合、こちらにご記入ください。利用経験度合いについても上記選択肢を参考にご記入ください。（200文字以内）

C (利用するだけでなくライブラリ構築等ができる. 仕様書 (ABI) を読みながら開発した経験がある。リファレンスやアセンブリを読みながら、パフォーマンスを意識した書き方が出来る)　2022年~現在
C++ 42Tokyoでの開発. 2023年~現在 現時点で一番自分の中で実装力のある言語です。
x86_64 アセンブリ (リファレンスがあれば利用可能 libc の関数などを, 呼出規約に準拠して実装した.) 2024/5~2024/7
Haskell (リファレンスがあれば利用可能 学習中) 2024/5~現在
TypeScript, Next.js, React, Nest.js, PostgreSQL: 利用経験: 42Tokyoの課題でPongゲームアプリケーションを開発, 期間: 2022年9月 ~ 2022年12月
Java: 利用経験: ドリーム・アーツのインターンシップでサーバサイド開発, 期間: 2024年2月 ~ 2024年5月
Linux, macOS 個人開発 42Tokyo 2022年~現在. OSの開発等では無く、シェルからの操作やシステムコールの利用が出来る。

C: 42Tokyo, 個人開発。利用するだけでなくライブラリ構築等ができる。仕様書 (ABI) を読みながら開発した経験がある。リファレンスやアセンブリを読みながら、パフォーマンスを意識した書き方ができる。期間: 2022年 ~ 現在
C++: 42Tokyo, 個人開発。自分の中で一番大きなプロジェクト(Http Server)をC++で経験し、現時点で一番実装力のある言語になっている。期間: 2023年 ~ 現在
x86_64 アセンブリ: 42Tokyo, 個人開発。リファレンスがあれば利用可能。libcの関数などを呼出規約に準拠して実装した。期間: 2024年5月 ~ 2024年7月
Haskell: 42Tokyo, 個人開発。リファレンスがあれば利用可能。学習中。期間: 2024年5月 ~ 現在
TypeScript, Next.js, React, Nest.js, PostgreSQL: 42Tokyoの課題でPongゲームアプリケーションを開発。期間: 2022年9月 ~ 2022年12月
Java: ドリーム・アーツのインターンシップでサーバサイド開発を担当。期間: 2024年2月 ~ 2024年5月
Linux, macOS: 42Tokyo, 個人開発。シェルからの操作やシステムコールの利用ができる。期間: 2022年 ~ 現在
Docker: 42Tokyo 期間: 2023年 ~ 現在


----

問2) MIXIのインターンシップで挑戦してみたいことや目的、目標を教えてください（500文字以内）*

- バックエンド, インフラの開発
見た目やデザインを考えるフロントエンドよりも、システム側の開発に関心があります。

- 多ユーザープロダクトの運用
個人で学習する中では多くのユーザーを抱えた開発が出来ないので、そういった経験を期待しています。

- Elixir や Rust での開発経験
これらの言語に興味があり、開発できる環境に魅力を感じています。

技術力（設計、パフォーマンス改善等）を伸ばし、より活躍していきたいです。

----

問3-1) これまでに開発を経験した場面を教えてください（複数回答可

学校の授業
独学
アルバイト


----

問3-2) 問3-1で回答した開発経験について、「技術的にアピールしたい」1つ目の経験について、詳細を教えてください。　記載例：＜概要：シフト管理ソフトウェア＞【開発背景】インターンシップ【利用技術】Go,PostgreSQL【開発環境】AWS,Docker,github actions　【チーム構成】3人(PM1、バックエンド1, フロント1)【担当領域】プログラミング領域全て【頑張ったところ/工夫したところ】~~~挙動を~~~できるようにしました【プレイ動画や作品URL】http://~~ （1000文字以内）*

概要: Nginxライク(IO多重化、シングルプロセスシングルスレッド)なHttpServerの実装(https://github.com/kotto5/webserv.git)
背景: 42Tokyoでの課題
技術スタック: C++,Googletest
チーム構成: 人数: 3人→2人
分担: 設定ファイルパーサー (1), Http・CGI通信 (2)
担当領域: Http通信およびCGI通信周りの実装
<成果
 Http通信の理解の深化: HttpプロトコルおよびCGI通信に関する理解を得ました。
 RFCドキュメントの読解力向上: 複雑な技術仕様を正確に理解し、実装に反映する能力が向上しました。
>
<工夫と努力
 <シンプルさの追求
  背景: 例外を用いて関数のエラー処理をしたところ、コード量が増えるにつれて呼び出し側で考えることが多くなってしまった。(ex:どの例外を処理すべきか どの例外が来るか）
  アプローチ: 「A Philosophy of Software Design」という書籍や Google C++ Style Guideで 例外が批判されていることを知る。解決策として戻り値を唯一のインターフェースとする設計を採用。これにより、プログラムの複雑性を低減。
  反省点: エラーの情報を引数の変数の状態を利用してしまった。RustにあるResult型を利用することでコードが理解しやすくなると反省>
 <テスト駆動開発 (TDD)
  背景: RFCの要件が大量だった為、品質を維持するための手段が必要。
  導入: テストツールのGoogle Testを導入し、要件をテストで定義。
  成果: テストにより修正の影響範囲が把握でき、チーム内のコミュニケーションコストを削減。効率的な開発が可能に>
 <チーム内コミュニケーション
  背景: プロジェクト開発中、あるメンバーのモチベーションが低下し、コミット量が激減してしまった。
  アプローチ: 率直に意見交換し、チームを解消しました。対話は時間や勇気が必要でしたが、お互い満足の行く選択を出来ました。この経験から、メンバーが伸び伸びと活動するために 1.日頃からのコミュニケーション 2.不満を小さいうちからチームで向き合うような雰囲気作りやシステム が切に必要だと感じました。>
>



---

問3-3) 問3-1で回答した開発経験について、「技術的にアピールしたい」2つ目の経験について、詳細を教えてください（1000文字以内）

概要: Pong Web アプリケーション (https://github.com/usatie/pong)
背景: 42Tokyoでの課題
開発環境: Github Actions, Docker
概要: Pongゲームアプリケーションの開発
技術スタック: TypeScript, Next.js, React, Nest.js, PostgreSQL
チーム構成: 4人. 機能ごとに分担し、メンバーそれぞれがフロントエンドとバックエンドの両方を担当
担当領域: チャット機能、OAuth、オンラインステータス管理を担当
<成果
 ウェブアプリ開発能力の向上: 基本的なウェブアプリの開発能力を向上させることができました。
 パフォーマンス問題への挑戦意欲: ユーザーが少なかったためパフォーマンス問題は発生しませんでしたが、今後取り組みたい課題として認識しました。>
<工夫と努力
 <迅速なキャッチアップ
 背景: チームメンバーのうち2人が現役または元Webアプリエンジニアで、自分は未経験だったため迅速なキャッチアップが求められました。
 アプローチ: 作業単位を細かく報告しフィードバックを受けることで、学習効率を高め、大幅な修正を避けるよう心がけました。この習慣はインターンでも役立ちました。>
 <リアルタイムオンラインステータス管理
 背景: ページ閲覧中にリアルタイムでユーザーのオンラインステータスを取得する必要がありました。
 アプローチ: socket.ioライブラリを利用し、通信回数を増やさないためにポーリングではなく、ステータスに変化があったユーザー起点で他のユーザーに通知する方式を採用しました。>
 <データベース設計の工夫
 背景: 入力値が限定的なカラム (ユーザーのRoleなど) の設計で、文字列型のカラムにするとデータを取り出すたびにバリデーションが必要になる
 アプローチ: Enumを利用し、データのバリデーションを不要にしました。型で保証し、複数人数で開発してもエラーチェックの抜け漏れが起きにくいように工夫しました。>
 <APIの命名規則
 背景: REST APIの命名規則を統一する必要がありました。
 アプローチ: LINEやXなどの有名なSNSを参考にし、REST APIの命名規則を遵守しました。>
>

---

問4) これまでの開発経験の中で、自分で定めた目標と、それを達成するために努力したこと、困難な課題をどのようにして乗り越えたかについて教えて下さい（500文字以内）*

私は開発プロジェクトでの意思決定に積極的に参加することを目標としました。過去には、他のメンバーの意見に頼りすぎて自分の理解が浅くなり、作業効率や創造力に悪影響が出ていました。この課題を克服するため、インターン中に客観的に評価できる具体的な目標を設定しました。

毎週少なくとも1度、設計レビュー(*1)で意見や提案を発表する。
インターン中に少なくとも一度、設計レビューで提案を行う。

初めはレビューの時間に質問をすることから始めましたが、殆どが知らない機能に関するPRの話題であり理解が追いつかないことが多々ありました。レビュー内容を事前に確認し、分からない点をまとめるようにしました。また、日頃からプロダクトに関する疑問をメンターに相談し、キーワードをまとめて知識を積み上げました。

この積み重ねにより、インターンの後半には準備にかかる時間が減り、理解力は向上しました。目標をメンターと共有し、定期的にフィードバックを受けることで、適宜改善を加えました。レビューでは意見の対立で悩むこともありましたが、プロダクトの品質向上のために意見を述べることの重要性を学びました。

*1 比較的大きいPRを承認する会議

---

問5) GitHub, Qiitaなどの公開アカウントや開発ブログ、公開しているWebアプリケーションやゲーム等の制作物がありましたら、URLを教えてください（800文字以内）*

github: https://github.com/kotto5

---

問6) 技術系イベント、インターンシップ、アルバイト等の参加経験がございましたら、イベント名/参加企業を教えてください ※インターンシップやアルバイトの場合、時期や期間、目的、利用言語など添えてください 記載例：MIXI(2023年10月〜2024年2月、サーバサイド開発、Ruby）（800文字以内）) *


インターンシップ
株式会社ドリーム・アーツ
期間: 2024年2月〜2024年5月
目的 内容: サーバサイド開発、プロダクトの保守運用
利用言語: Java

---

問7) 現在興味を持っている技術について、興味を持っている理由と、その技術において新しく挑戦していることや学習していることがあれば教えてください（500文字以内）*
現在の文字数 0

- 低レイヤ

最近はlibc の関数をアセンブリで書きました。新しいことを学習するのが好きなのですが、低レイヤの学習は点と点(今までの知識)が線で繋がる(関係性が分かる)ことが多く、学ぶのが面白いです。(ex: 引数とは何か, スタックバッファオーバーフローによる攻撃 と espレジスタ などは アセンブリの学習を通して解像度が上がり京楽を得ました. 低レイヤの知識をハブの点になり色々な知識が繋がります)

- Haskell (関数型プログラミング)

自分が今まで書いていた手続き型、オブジェクト指向のプログラミングとは異なり、プログラムがシンプルになる魅力を感じています。
以前に大規模なプロダクトで開発した際、スコープの広い変数の状態を駆使して動いている部分がありました。これが、一見依存関係のない関数同士に依存関係を作り、可読性が落ち開発効率が著しく低下しました。こういった課題を解決する、保守性、可変性の高いプログラム設計のアイデアを得るために学習しています。


---

問8) 希望の開始時期、参加期間、週何回出勤可能か教えてください(例)12/1(水)～、3週間～4週間希望、週5日勤務可能　※合格後、入社手続きに3週間ほどお時間をいただきます*
希望開始時期	
参加期間	
週間の出勤可能日数

---

問10-2) MIXIに興味を持ったきっかけを教えてください（500文字以内）*

- MIXIでインターンをしている知人などから、社員の方の技術力の高さ、またMIXIでのチーム開発のやりやすさを伺った
- インフラの分野で技術的な挑戦をしていると聞いた

---

問10-3) 問10-1で「その他」をお選びいただいた場合、詳細を教えてください。または、「友人・知人からの紹介」をお選びいただいた方は、紹介者名を教えてください

