+++
title = "Skycoin AMA Log (held at ark.io)"
tags = [
    "Ask the Developers",
]
date = "2017-08-01"
categories = [
    "Ask the Developers",
    "Statement",
]
bounty = 12
description = "Log of AMA with Skycoin held at ark.io/slack/ (from 2017-07-02)"
+++

*この対談は2017年2月に[ark.io slack](https://ark.io/slack/)で行われたものです。*

*synth氏はSkycoinの代表としてAMAに参加しました。*

**boldninja**
Skycoin.netのsynthさん、ようこそ。本日はAMAのお時間をいただき、ありがとうございます。

**synth**
どうも、こんにちは。

**mike**
こんにちは、synthさん。

**jakethepanda**
やあ、synthさん。

**thrice.pi**
どうも、synthさん。

**dr10**
こんにちは。

**boldninja**
さて、いつもどおりにはじめましょうか。1度にする質問は２〜３個までにとどめるようにしてください。

**dr10**
Skycoinの良いところを簡潔に説明してくれますか？例えば、雑誌や暗号通貨に詳しくない人を想定して。

**mgaruccio**
メッシュネットについて説明をお願いします。単なるノード間のMPLSネットワークですか？それとも何か大きな構想があるのでしょうか？ 

**michaelthecryptoguy**
やあやあ、synthさん。

**tranzer**
synthさん、流通していないコインは、コールドウォレットに保管してあるのでしょうか？coinmarketcap.comによると全供給量の部分的にしか現在は流通していません。あと、Skycoinの特異的な機能はなんでしょうか？

**synth**
Skycoinを簡潔に説明するのは難しいですね。６年間も開発が続けられてきた大きなプロジェクトですから、各部分がそれぞれの目的を持っています。 
暗号通貨、コインの部分は、既に存在している合意形成アルゴリズムの問題を解決するために作られました。１秒あたりに300という送金の処理速度を誇ります。分単位ではなく、秒単位の話です。マイナーを必要とせず、インフレ防止のためにブロック報酬もありません。51%攻撃や他のマイニングに関する問題を既に解決しています。 
そして、他にも多数のプロジェクトや実験段階のアイデアがあります (https://github.com/skycoin)。メッシュネットと分散型VPNのプロトタイプがあり、ネットワーク参加者はトラフィックを転送するために帯域幅を共有することで報酬を得られます。また、分散型ソーシャルメディアのアプリケーション、P2Pのデータ複製・収容のためのアプリ、その他の実験的なプロジェクトがあります。変更不可なデータ構造に関するリサーチを重ね、次世代のインターネットの構想を着々と実現に近づけています。いくつかは非常に革命的なプロジェクトです。

**dr10**
ネットワーク合意形成アルゴリズムの「Obelisk」はどのような仕組みで、よく知られている他のアルゴリズム（Proof of Work, Proof of Stake）とはどう違うのですか？

**mgaruccio**
実際にどのくらい実用化されていますか?例えば、現時点でSkycoinのブロックチェーン上にアプリを作ることはできますか?

**mike**
進捗状況に関して、プロジェクト発展の最大の障壁になっている要因はなんでしょうか？例えば、資金、人手、技術的な限界点などですか？ 

**synth**

> メッシュネットについて説明をお願いします。単なるノード間のMPLSネットワークですか？それとも何か大きな構想があるのでしょうか？ 

これは単なるメッシュネットのプロジェクトではなく、強力なソフトウェア・ディファインド・ネットワーキングです。全く新しいプロトコルとネームスペースを用いた次世代のネットワーキングのプロジェクトになり、既存のインターネットに頼ることなく成り立つものです。
インターネットがホットポテト・ルーティングを使用している一方、私たちはソース・ルーティングを用いるので、最適化されたレイテンシーが実現されます。
IPv6では不可能な、マルチホーミングにも対応しています。ギガバイトやテラバイトのネットワーキングとマルチ冗長化された帯域幅のパスを確保するのに欠かせない要素です。 
リンク層とE2Eの両方で日和見暗号化がデフォルトとなっています。既存のインターネット異なり、全ての通信はデフォルトで暗号化されています。 
ストアアンドフォワード・ネットワーキングになりますので、レイテンシーが分や時間単位、そしてパケットの損失が大きいアフリカのような地域でも、問題なく動作します。既存のプロトコルでは動作しないような環境でも、私たちのネットワークには影響なしでしょう。IPv4/IPv6やTCP/ipより、さらに安定した確固なネットワークとなります。
プライバシーの問題にも取り組んでいます。パケットが１０の中継地点を通って転送されるとしたら、それぞれの中継地点は直前と直後のノードの情報しか得られません。IPv4のように各パケットが出発と到着地点の情報を持つようなことはありません。このプライバシーのレベルは、現在のインターネットでは不可能です。
IPアドレスは公開鍵に置き換えられ、目的地へのトラフィックは誰にもわからなくなります。それを知るのは、目的地を定めるための公開鍵の秘密鍵を持つ者のみです。このシステムは第三者や認証のための組織を必要としません。革命的なデザインといえるでしょう。

> 流通していないコインは、コールドウォレットに保管してあるのでしょうか？coinmarketcap.comによると、全供給量の部分的にしか現在は流通していないことになっています。

100の異なるアドレスに、１００万個のコインがそれぞれ保管されています。定期的にロックアップが解かれ、段階的に流通量が増えることになっています。
複雑なロックアップと解除の手順があり、これにはデベロッパー全員からのコンセンサスが必要になります。 このグループにいるデベロッパーなら誰でもが、流通量の増加を止める権限を持っています(暗号通貨のNXTはこの対策に失敗しました)。元々の設計により、コインの流通量を増やすのは難しくなっており、決定には事前承認された正当な理由が求められます。

**mike**
ワイヤレスのSkywire(上記のプロトコルの名前)のノードとなるためには、どのようなハードウェアが必要ですか？

**arc-over-water**
nxtは問題なくやっていると私は思いますが。

**synth**

> ネットワーク合意形成アルゴリズムの「Obelisk」はどのような仕組みで、よく知られている他のアルゴリズム（Proof of Work, Proof of Stake）とはどう違うのですか？

PoSとPoWにはマイナーが必要であり、ブロック生成の報酬にマイナーは新しいコインを受取ります。マイナーはたくさんのお金を得ており、自分たちの利益となるようにネットワークを操作しようとするでしょう。新たなコインが生まれるたびにインフレが悪化し、コインのユーザーが被害を被るのです。
Skycoinはマイニングとインフレの問題を解決するように設計されました。ブロック報酬はなく、新たなコインも生まれません。このためには新たな合意形成アルゴリズムが必要で、制約をクリアするには限られた方法しかありませんでした。Michael Ben-Orが考案した、分散化されたシステムで合意形成をとるためのランダム化の手順を改良し、合意形成を邪魔する悪意あるノードを検知する仕組みを加え、「Obelisk」が完成しました。
skycoin.netに詳細が記されたホワイトペーパーがあります。これは「ネットワークコンセンサス」 と呼ばれるべきものです。信頼の環の仕組みを用いて、ブロック生成をする人びとが悪意ある行動をしたときに、その人をネットワークから追放できる仕組みを作りました。同時に、ネットワークをコントロールする人びとも、ネットワークを攻撃する力はありません。できることといえば、処理速度を遅くして邪魔をするくらいなので、悪意ある行動をするノードは追放され、新たな参加者に置き換えられるだけです。

**mike**
Skywireが公開され、ハードウェア上のノードとして機能するのはいつですか (テストネットとメインネットの公開予定日)?

**mgaruccio**
もしブロック報酬がないとすれば、ノードになるインセンティブは何なのでしょうか？

**vega**
Skycoinの実際の機能はなんですか?説明されていた様々なプロジェクトを統合して、価値を保存、交換するために使われるのですか?それとも、もう少し限定的な機能ですか？

**michaelthecryptoguy**
ノードとなるためのハードウェアのスペックはなんですか?初期段階においては?ユーザー数が10000人の段階では?

**synth**

> nxtは問題なくやっていると私は思いますが。

nxtでは3人の人間がそれぞれ供給量の30%のコインを所有していました。このうちの１人がプロジェクトを途中で脱退することを決め、コインを投げ売りしました。NXTは当時1億５千万ドルを超える市場規模でしたが、彼が投げ売りをはじめたせいで、NXTの価格は地に落ちました。 
創始者や早期の参加者が投げ売りをするのを防ぐように、Skycoinの分配計画が作られています。
Skycoinの流通量が供給量の30%になったとき、 残りのコインには計画的なロックアップがされる予定です。毎年最大で5%のコインが解除、分配されることになります。つまり、残りの70% が分配されるまでに最短で14年かかることになります。
残りのコインを今売ることはできません。なぜなら、全体の10%を5ドルの価格で売ると、５千万ドルの資金が手に入ることになり、現時点の私たちにその資金は必要ありません。現段階においては使い道のないお金です。 
Ethereumは3千万ドルから7千万ドルの資金を最初の数年に使い切り、危うく破産するところでした。シリコンバレー並の給料を支払い、綺麗なオフィスを借りたり、といったような使い道です。Skycoinでは保守的な資金の使い方をしており、これまでコストの削減を意識してきました。現在の市場においては、何もプロダクトを発表していない状態で１00億ドルもの資金を調達しようとするEOSのようなプロジェクトもあります。彼らが何にお金を使う予定なのかまるで不明です。マーケティングとPRを目的としたパーティーをタイムズ・スクエアで開催するために350,000ドルものお金を浪費しているという話を聞きました。 

**arc-over-water**
なぜさっさとコインを売ってしまわないのですか?5千万ドルくらいだったら小さい資金額でしょう?
nxtはskyよりも新しいプラットフォームですが、 nxtの時価総額は2億2千万ドルでskyは1億6千万ドルです。あなたの言い分は理解できますが、証拠がないでしょう。nxtのコミュニティは非常に大きく、活動的です。全く崩壊などしていないと思いますが、どうでしょうか？

**synth**

> Skycoinの実際の機能はなんですか?説明されていた様々なプロジェクトを統合して、価値を保存、交換するために使われるのですか?それとも、もう少し限定的な機能ですか？

前者になります。Bitcoinには特に使用価値はありませんでした。アルトコインには２つの機能があります。残高を確認して、他の人にお金を送ること。
コインが価値を持つためには、特定のサービスを利用するために購入される必要があります。実際にコインが使われ、需要が生まれるための価値の源泉がないといけません。
こうして考えると、Bitcoinは完全に投機的な資産です。キャッシュフローはなく、人びとの主観や社会の常識が価値を決めます。
アイデアとしてのSkycoinは「Bitcoinの改良版」としてスタートしました。より速く、安全で、シンプルに、新たなアルゴリズムで。しかし、時間が経つと共に、私たちは1つのエコシステムを作り上げるに至りました。そこにはコインの価値の裏付けとなる使用価値とネットワーク価値が生まれます。
例えば、メッシュネット (skywire) は良い例です。ユーザーは使用するためにコインを手に入れる必要があり、サービスの利用でコインが消費されます。Skywire上のVPNを通してインターネットを利用するとして、おそらく使用料金は驚くほど安いものになりますが、それでも実際の経済活動が生まれていることに意味があります。使用価値に裏付けされたコインと、それを使うコミュニティがあるからです。 そこに投機家はいません。
開発後期になってくれば、プロジェクトの射程はさらに広くなるでしょう。

**arc-over-water**
インターネットの使用時に、SkycoinのウォレットがVPNとして使えるということですか?

**synth**

> nxtはskyよりも新しいプラットフォームですが、 nxtの時価総額は2億2千万ドルでskyは1億6千万ドルです。あなたの言い分は理解できますが、証拠がないでしょう。nxtのコミュニティは非常に大きく、活動的です。全く崩壊などしていないと思いますが、どうでしょうか？

あの出来事がなければNXTは今よりも進んだ状態に発展していたでしょう。Ethereumと比較しても劣らない地点にいたかもしれない。あの分配計画のミスと価格崩壊のせいで、数年の遅れが出たと言っても過言ではない。長期的に見て、大量保有者が価格に与え得る影響を甘く見ていたのです。 

**arc-over-water**
IOTAでも同じようなことがありましたね。リードのデベロッパーで、あれは１００億ドル近くでしたか。
コインを完全に分配し、市場に価格を決定させていました。

**synth**

> インターネットの使用時に、SkycoinのウォレットがVPNとして使えるということですか?

Skywireを経由して帯域幅を使うアプリケーションの1つがVPNです。他にもいくつかのプロジェクトが進められています。
例えば、4chanをモデルとして、CXOによって分散化されたBBSがあります。 https://github.com/skycoin/bbs
Skywire上で機能する、新たなインターネットを私たちは作っているのです。開発されるアプリはプライバシーを重点に置いた、専門的なものです。GitHub上のskycoin/bbsを見てください。BBSの開発に興味がある方は是非協力ください。 

**mike**
Skycoinの価値はProof of Resource、つまり、何かしらのサービスに裏付けされているんですね。この場合はプライバシー保護がされた、安全なネットワークということでしょうか？分散化ストレージ、分散化されたコンピュータ処理能力の提供などのサービスを展開していく予定はありますか？

**arc-over-water**
さっき言っていた、100万個のコインが保管してある100個のアカウントから、どのようにコインを分配していくのですか？100回のICOをやるのか、それとも既に配分プランがコーディングされているのか、デベロッパー次第で決められるのか。どれでしょうか？

**rockyj**
それは計算すればわかりますよ！

**slackbot Custom Response**
https://docs.google.com/spreadsheets/d/1FGo3FkC3uSWXGHatPQyny2brMWjAIJsHFCR-Lhkl_m0/edit#gid=0

**synth**

> もしブロック報酬がないとすれば、ノードになるインセンティブは何なのでしょうか？

合意形成のノードを稼働するのにコストはかかりません。Raspberry Pi上でも動作確認済みです.
重要なのは、もしノードを稼働している人びとが悪意をもった行為をすれば、コミュニティにより追放され、代わりのノードが代替するということです。他に重要な点は、ノードがプロトコルに沿って動作しているかどうか、自動的に監査ができることです。
Skycoinのノードはネットワークを操作する力を持たず、できることは処理速度を遅くすることくらいです。他の人のコインを使うことは秘密鍵がなければ不可能ですから、合意形成のノードがネットワークにもたらす脅威は限りなく小さいものです。Bitcoinの場合はマイナーがネットワークを人質にとり、利己的な行動をとることができます。例えば、自分たちの利益追求のために送金手数料を釣り上げたり、全体にとって有益になり得るbitcoinのアップデートを邪魔したり、ということをマイナーがしています。

> Skycoinの価値はProof of Resource、つまり、何かしらのサービスに裏付けされているんですね。この場合はプライバシー保護がされた、安全なネットワークということでしょうか？分散化ストレージ、分散化されたコンピュータ処理能力の提供などのサービスを展開していく予定はありますか？

私たちは既に分散化されたストレージ、CXOを開発しました。しかし、帯域幅のみがSkywireによってマネタイズされています。それぞれのAPIの動作のために手数料をとるようなことは私たちはやりません。無料のものは無料であるべきです。これが私たち独自の哲学なのです。 
CXO上で動作するソーシャルメディアも開発を進めています (Steemitに類似したもの)。
CXOはIFPSに似ていますが、よりシンプルで私たちの開発環境に合うようにデザインされています。暗号技術に特化した設計です。

**mike**
遅くて働きの悪いノードを避けて、最も速いルートにトラフィックを最適化することはできますか？それはSkycoinの合意形成の安定化につながると思います。

**tranzer**
Skycoinの毎秒のトランザクション数はいくつですか?ブロック生成時間は?

**thrice.pi**
300でしょう? ^

**arc-over-water**
非チューリング完全なLISPのプログラミング言語を使っているとウェブサイトにありましたが？

**synth**

>さっき言っていた、100万個のコインが保管してある100個のアカウントから、どのようにコインを分配していくのですか？100回のICOをやるのか、それとも既に配分プランがコーディングされているのか、デベロッパー次第で決められるのか。どれでしょうか？

分配計画を近いうちにウェブサイトに掲載します。これは複雑で説明が難しいのです。
市場に出回っているコインはSkywireの使用にかかる租税によって回収されていきます。ネットワークの資源を使うために支払う租税により、実質的には自動的にコインが回収される仕組みです。ここで流通量はピークとなり、それから下降曲線をたどっていきます。しかし、ロックアップされたコインが唯一の分配源として残っています。定期的に解除、分配され、流通してから、また供給源に戻ることでしょう。 
ここには２重の経済構造があります。コインを流通から外すための買上げと、ユーザーがコインを保持するインセンティブを与える分配金の配布です。 

**arc-over-water**

つまり、２種類の通貨が存在するということですか。片方を所有することで、他方が付与される。

**synth**

> 遅くて働きの悪いノードを避けて、最も速いルートにトラフィックを最適化することはできますか？

はい、可能です。これはとても重要なことです。
Skywireに接続をしようとする個人が、接続先へのパスを決められるのです。
例えば、ビデオゲームやSkypeの会話には、レイテンシーの低いパスを選ぶことができます。ビデオのダウンロードには最もスループットの高いパスを選びます。もしくは、特定のノードや機能、国を通るパスを選ぶことができます。これはセキュリティ上の懸念のため、また経由地点の数を最小化するのも選択肢にあります。

**mike**
元々計画にあったように、Skywireのノード参加を促すための報酬を与える予定ですか？

**dr10**
あなたの構想している技術とサービスを消費者に提供するのはいつごろですか？あなたの実現しようとしているものを、いつになったら使えるようになるのですか？

**synth**

> 非チューリング完全なLISPのプログラミング言語を使っているとウェブサイトにありましたが？

それは何かの間違いでしょうね。そのうちに新しいウェブサイトが公開される予定です。
Skycoinのブロックチェーンにスクリプト言語はありません。効率性と安全性を確保しながら、最も速い処理速度とシンプルな設計を可能とするために、各トランザクションは定数時間となっています。
ただ、現在開発中のCXというプログラミング言語があります。Ethereumのスマートコントラクトなる遊びを超えた、次世代のプログラミング言語です。変更不可能なデータ構造を用いており、これは全く新しいものです。Skycoinのスマートコントラクトはオフチェーンまたはプライベートブロックチェーン上で処理され、メインチェーンに全てのデータを突っ込むようなことにはなりません。全員が他の人びとのコントラクトの内容をダウンロードして、ブロックチェーンを混雑させるような状況をわざわざ作るのか？他にもっと良いやり方があるでしょう。 

> 元々計画にあったように、SkycoinはSkywireのノード参加を促すための報酬を与える予定ですか？

はい、そうです。 全体の20%〜30%のコインをネットワークの参加して、Skywireのノードを維持するためのインセンティブとして使いたいと考えています。 
これは大きなマーケティング効果をもたらすでしょう。コインをユーザーに分配するのに最も効果的な方法であり、数人の大量保有者を生むよりも良いことです。

**samuelvihollandia**
SkycoinがVPN接続のために使われると話されていましたが、これが最も大きなSkycoinの存在理由でしょうか？

**arc-over-water**
Maidsafeはインターネットの再構築のために約１０年間を費やしてきました。Skycoinとの共通点や相違点はどこにあるのでしょうか？

**synth**

> SkycoinがVPN接続のために使われると話されていましたが、これが最も大きなSkycoinの存在理由でしょうか？

いいえ、既に動作している、簡単な実用化の例に過ぎません。最もスケールの大きいアプリケーションではありません。
現在インターネットのトラフィックの80%はbitorrentが占めていますが、bitorrentのウェブサイトは次々と閉鎖され、インターネットから追放されていっています。しかし、それらのウェブサイトは完全に消えることはなく、公から見えない場所に姿を隠すだけなのです。 What.cd (最も大きなマルチトラックレコーダーサイト、80万人のユーザー数)は閉鎖され、bakabt (最も大きなアニメトラックレコーダーサイト)は新規登録を締め切り、Nyantorrent、その他も...
何百万人ものユーザーを抱えるコミュニティが、企業によって作られている現在のインターネットから、新たなインターネットへと移動してくるのです。これかが何百万人の単位でユーザーが移動をはじめるのを私たちは目撃することでしょう。

**arc-over-water**
Skycoinは企業ですか？それとも財団、または慈善団体ですか?登録はされていますか?Skycoinについて書かれた文章をまだ見たことがないのですが?デベロッパーのチームの規模はどれくらいですか?バックグラウンドは?Maidsafeはオープンで、情報も透明性があります。IOTAやStellarも同じです。あなたのチームに誰がいるかを教えてもらえますか?15年にもまたがる計画をあなたは話されているのですから、ユーザーが信頼できるチームでなければならないでしょう..

**techbytes**
Skywireのノードを稼働させるには、Skycoinを持っている必要がありますか？これはマスターノードのような仕組みなのでしょうか?

**synth**

> Maidsafeはインターネットの再構築のために約１０年間を費やしてきました。Skycoinとの共通点や相違点はどこにあるのでしょうか？

Maidsafeは現在バージョン2かバージョン3になります。Maidsafeがまともなコインを作るようになるのは、バージョン9になってからです。それぞれのバージョンの開発に数年がかかっています。 このペースでいけば、Maidsafeの構想の実現には少なくとも18年がかかるでしょう。
それに対して、Skycoinは6年の開発期間、メッシュネットは4年間で、数ヶ月以内には完成する見通しです。そのときには、人びとが使える段階まで持っていけるようになるでしょう。
Skycoinの目的はmaidsafeと似ていますが、アプローチ、設計、成り立ちからして異なります。全てをやろうとするのではなく、小規模なコアの部分に集中して、これまで実績を積み重ねてきました。
様々な暗号通貨のプロジェクトが乱立していますが、実現可能なタイムラインで実際に新たなインターネットを作り、これだけ大きなシステムの構成部分をデザインして、それぞれの開発段階で役に立つものをリリースしているチームは数少ないのです。 そして、この計画は１０年単位のものなのです。

**mike**
ArkとSkycoinが互いの上にシステムを作り、シナジー効果を生み出すことは可能でしょうか? 重力を無にしてしまうようなSkycoinのプロジェクトを前にして、車輪を新たに開発しようとするのは無駄な試みですから。 
SkycoinはTCP/IPの構造を置き換え、ハードウェアの次元でメッシュネットの機能を実現するものでしょう。Arkはその上のアプリケーション層として機能できるのではないでしょうか？ 

**arc-over-water**
Maidsafeの最新情報にもとづいて話されているのでしょうか？アルファ段階を終えて、プロジェクトは来年にはリリースされるのでは?Maidsafeによれば、公開されれば、ウイルスかAIのように人類にとて驚異的な存在となるだろうとのことです。Tau Chain、HunterMinerCrafterによるAutonomicも同じカテゴリでしょう。Maid、Sky、Tau、Autonomicは私たちをAIの世界に連れていこうとしているのでしょうか?

**dr10**
今はsmartbridgeでしょう!

**mike**
Skycoinは分散化された、グローバルなクラウドサーバーとなろうしているということでしょう。そして、その上にアプリケーションの開発がされるという。コミュニケーションの形としては、メッセージを送ったり特定のサーバーにサイトをホストするのではなく、暗号化されたファイルを特定の受信者に共有するといったものになるのですね。

**synth**

>Skycoinは企業ですか？それとも財団、または慈善団体ですか?登録はされていますか?Skycoinについて書かれた文章をまだ見たことがないのですが?デベロッパーのチームの規模はどれくらいですか?バックグラウンドは?

これまで60人近くの人たちがSkycoinで働いた、もしくは主要な貢献をしてきました。これはダークネットのプロダクトだと言えるえしょう。
この人びとの多くは匿名でした。そのうちの何人かは軍隊におり、秘密情報保護法のために、匿名でなければならなかった。San Diegoの海洋防衛研究所で働いていた人もおり、ネットワーキングプロトコルのアイデアは彼が貢献してくれました。公共セクターによる、アカデミアで検証済みのアイデアでした。
他のメンバーには、Bitcoinの極めて初期の開発を行ったデベロッパーたちや、Bitcoin以前から暗号技術に携わっていた専門家、またEthereumのコアデベロッパーがいます。
中国側のメンバーには、Alibabaの初期投資家やテレコム事業の投資家がいます。China Aviation Group(４つの航空会社のホールディングス)とパイロットプログラムを進めていますが、Sinopecも加わる予定です (世界で２番目に大きい上場企業)。
そして、アメリカとイスラエルの秘密情報組織の人間もいました。このグループの人たちは、Skycoinの送金処理の匿名化とCoinJoinプロトコルを実装する手筈に興味を示していました。フォレンジック会計の専門家からもアドバイスを受けており、Bitcoinの欠陥、メタデータの欠如、その他の知見を提供してもらいました。 
あとは博士号を保有している研究者がたくさん関わっており、データベースの合意形成アルゴリズムやプログラミング言語のリサーチをやっています。
ダークネットの深部からやってきた参加者もいます。anon、frog twitter、cipher punks、bitorrentなどのコミュニティから来た人たちです。ロシアのダークネットコミュニティからの参加者もいます。８人の参加者が同じ名前「イワン」を持っています。

> SkycoinはTCP/IPの構造を置き換え、ハードウェアの次元でメッシュネットの機能を実現するものでしょう。Arkはその上のアプリケーション層として機能できるのではないでしょうか？

それは可能でしょうね。Skycoinの根本的な要素は２つです。まず、公共鍵（ネットワーキング）にユーザーを接続することです。そして、分散化された合意形成をする、変更不可能なデータのP2P取引（送金処理、ブロック生成、データストレージ、その他）があります。
この上であれば何を作るのも可能です。これらの基礎の上にインターネットが再構築され、既存のプロトコルを置き換えることになるでしょう。 

**arc-over-water**
どの組織が資金を提供しているのですか?ICOを２回やったようですが、いくらの資金を手に入れましたか?最初の各コインの値段は10セント、２回目は50セント、合計販売量は６百万個で間違いありませんか?

**samuelvihollandia**
他の取引所への上場予定は近々にありますか?

**arc-over-water**
あなたはSkycoinの初期段階から関わっているのですか?誰が初期メンバーですか?ICOで得た資金を誰が配分するのですか？分散化されたプロジェクトというのは投資に当っては諸刃の剣ですね。私たちはチームに投資をするわけですが、そのチームの構成員が誰なのかわかりません。なので、こうして質問をするわけです。

**thrice.pi**
先ほどあげた人びとのなかで、メインのメンバーは誰になりますか？開発のために外部の人間も長期で雇われているのですか？

**synth**

> どの組織が資金を提供しているのですか?ICOを２回やったようですが、いくらの資金を手に入れましたか?最初の各コインの値段は10セント、２回目は50セント、合計販売量は６百万個で間違いありませんか?

最初の４年間に資金提供をしていたのは初期のbitcoinの関係者と、暗号技術の専門家です。Bitcoinや他のコインが根本的な問題と向き合おうとしないのに不満を覚えており、その課題を乗り越えようするSkycoinに資金を提供してくれました。合計で1200個のbitcoinがプロジェクトのために無償で与えられました。 
Skycoinの初期は学問的研究、ネットワークの設計、新たなアルゴリズムのシミュレーションをやっていました。後期ではプロジェクトマネジメントや実装に重点が置かれています。
私たちは小さな規模で４回のICOを行いました。プロジェクトのための資金集め、またプロジェクトに関わっていたデベロッパーたちへのコインの分配を目的としていました。最初のICOの値段は１コインあたり10セントで、現在の市場価格は4ドルです。既に35~40倍のリターンを出していることになります。もちろんビットコインの価格上昇に比べれば劣りますが。

**arc-over-water**
１年で35倍の価格上昇があったならば、次のICOをして価格上昇を落ち着ける時ではありませんか？もしそうであれば、どれくらいの量をどのように配布する予定ですか？

**mike**
Intel Edison、Joule、もしくはSamsung Artik 10はSkywirのワイヤレスノードとして機能しますか?スペックは2Gb-8GbのRAM、8-64Gg eMMC storage、802.11n wireless、 bluetooth、Zigbeeです。

**synth**

>あなたはSkycoinの初期段階から関わっているのですか?誰が初期メンバーですか?ICOで得た資金を誰が配分するのですか？分散化されたプロジェクトというのは投資に当っては諸刃の剣ですね。私たちはチームに投資をするわけですが、チームの構成員が誰なのかわかりません。なので、質問をするわけです。

当初は３つの異なるグループがありましたが、最初の３年で１つとなりました。それぞれが異なるプログラミング言語を使っており、python、C、golangで、golangのコードが現在のコードベースとなっています。
コインの新規配布は、グループの全員からの同意が必要であり、具体的な目的が決まっている場合のみです。
全体の資金源として、様々なプロジェクトマネジャーが使えるbitcoinがあります。デベロッパーや契約社員の給料、そしてマーケティング費用のためのオペレーションの資金です。
また、企業からの後援も受け手います。フルタイムのデベロッパーの給料のための資金源です。

**arc-over-water**
Silicon Valley (テレビ番組)の最近のエピソードで、分散化されたインターネットがスマート冷蔵庫のネットワークが登場しました。これはスマートフォン、スマート機器であれば同じように可能なわけですね?このような家庭機器もSkywireのノードとして機能して、報酬を受けることは可能なのですか？

**mike**
理想は完全なオープンソースで、ノードに自動監査システムを組み込んで、バックドアを防ぐことでしょうね。今ではチップの製造者でさえ、自分たちがチップのなかに何を組み込んでいるのかわかっていないくらいです。IPコアなるブラックボックスをASICデザインに入れるだけの単純作業になっています。

**synth**

>１年で35倍の価格上昇があったならば、次のICOをして価格上昇を落ち着ける時ではありませんか？もしそうであれば、どれくらいの量をどのように配布する予定ですか？

私の記憶が正しければ、Skycoinの値段は40日毎に2倍になっています。しかし、時価総額のトップ20に入るには数年かかるでしょう。 bitcoinでも1ドルの値段を付けるのに数年かかりました。6年間連続で毎日1%の価格上昇はありましたが。

> 理想は完全なオープンソースで、ノードに自動監査システムを組み込んで、バックドアを防ぐことでしょうね。

私たちはarmを使う予定です。

**arc-over-water**
IOTAもノードのためのハードウェアを製造しようとしています。

**synth**
全てのintelとAMDのシステムは遠隔操作でエンジンをバックドアできます。そのため、大量のコインを保管するには安全な選択肢ではありません。
Skycoinのノードにはalpineバージョンのlinuxと独自のバージョンのlinuxがOSとして用意されています。6MBで全ての仕様が揃っています。カーネルにバイナリーブロブもなく、ソースから組み立てられないものは含まれていません。systemd、gli、opensslはなく、muslのみが使われています。

**mike**
SamsungのArtik5またはArtik10がノードとして稼働するのには問題なさそうですね。ARMを基盤にしていますし。サイズはArtik10で25x35x4mm、Artik5は少し小さいですが、２つのアンテナポートがあります。無指向性アンテナには向いているでしょう。

**earlyarkinvestor**
ArkはLiskと比較してどうでしょうか?

**synth**
uploaded this image: 1923810435.jpg Add Comment

**earlyarkinvestor**
Liskは異なるブロックチェーン間の交流を可能にしようとしていますね。

**synth**
uploaded this image: 1433594905.jpg Add Comment

**synth**
uploaded this image: 1432540863.jpg Add Comment

**synth**
uploaded this image: 2049465686.jpg Add Comment

**mike**
良い写真ですね。ARMを基盤にしたサーバーラックのように見えます。
必要があれば是非手伝いましょう。solidworks上でしたら、私もユーザーなので便利です。

**synth**
これがSkycoinのクラスターです。8個のCPU板、CPU板毎に4つのコア、2GBのram、64bitのARMプロセッサーです。各CPU板で１つのプログラムが稼働するので、１つの部分に不具合が生じても、他の部分が正常に動くように設計されています。

**mike**
各CPU板に2つのethernetのポートがありますね。

**synth**
ハードウェアにはqualcomのバックドアもありません。これは中国製の機器になりますから。バックドアは通常においてカーネルレベルで行われ、ハードウェアのバックドアというのも現時点ではありませんが。 

**mike**
SATAポートはありますか？おそらく容量はM.2でしょうか?

**synth**
最終的にはARMのopenwrtを使ったルーターも作る予定です。
現在製造中のモデルはSATAがありませんが、SATAに対応するモデルもあります。16個の2TBドライブが接続できます。パイレートベイの半分のコンテンツを自分のクラスタにダウンロードするのも可能になりますね。
Skycoinのインフラはクラスタを基礎にして、300個以上のコンピューターの間で稼働するようにデザインしてあります。各コンピューターで１つのノードです。 CXOのストレージノードまたはSkywireのSDN/meshnetノード、もしくはVPNのエンドポイントノード、合意形成ネットワーク、Skycoinの送金処理ノードなど、異なるアプリケーションとノードのタイプが存在します。
これ自体がパーソナルクラウドとも言えるでしょう。
StorJのように、他の人びとが自分のデータを保管するのではありません。5個のクラスタと300個以上のコンピューターからなる自身のインターネットに、自身のハードウェアに、ファイルを保管できるのです。自分のネットワークの外に出る必要はありません。 

**mike**
M.2ソケットの列があるCPU板があれば、SSDをケーブルなしに稼働させられますね。サーキット板にバスを内包させて。 

**synth**
M.2も最終的には実装されるでしょう。
現行のものはストレージにmicroSSDを使っており、速度は48MB/秒です。

**mike**
このARM板はどれくらいの価格になりますか?IntelのBitseed V3を考えていますが、あなたの説明するARM板もよいかもしれません。SATAが付いていれば尚更。 

**arc-over-water**
現実に使用可能な機能は次のどれが公開されますか?コインとウォレットが最初のリリースでした。将来の開発と公開予定を教えてください。

**synth**
板はそれぞれ30ドルですが、SSSのメモリはCPU/RAM板よりも高い値段です。これはおかしな話なのですが。

**mike**
microSSDの最大サイズは何ですか?私たちは現在、1Tbのハードドライブを配布しているところです。

**synth**
Bitseed Mikeが手助けをしてくれる予定です。そうすれば板を集めてカスタムのPCBができます。

**mike**
そこですね。RAMとeMMCのコストのせいで価格が跳ね上がります。
低価格の板でSATAが付いているのもないですから。

**synth**
Orange Piがおすすめです。
SATAになった途端に価格が30%上がります。 

**mike**
Orange Piはスペックが優れていますね。

**synth**
最終的には、オリジナルのカスタムPCBを製造して、ブレードサーバにしたいですね。 

**mike**
Samsung Artiksは省スペースパソコンで、ドローンルーター、cubesat/picosatの可能性もあってよいと思います。
しかし、オリジナルの板を作り、サプライチェーンの深部を自身で管理できるというのは魅力的ですね。

**synth**
必要なのは、ram、CPU、microSDスロットのみで、wifiやら他の部品はただの役立たずです。コミュニケーション、ストレージ、計算能力があれば十分です。ミニマリストですね。

**mike**
同意します。pcduino nanoにもいくつかのポートを使うだけで、ビデオやらオーディオ、その他の機能は必要ありませんしね。

**synth**
オープンソースのFPGAツールチェインすら存在しますね。 a one instruction computer with subtract and jump if not zero; and if you have ram and a byte array, could even compile down to that; which is trolling, but for signing transactions or something, you could operate at that level.

**mike**
そのFPGAのリンクはありますか？私のお気に入りはZYNQ7000ですが、そのFGPAはかなり低コストになりそうです。

**synth**
FPGAの詳細を調べてみます。

**mike**
Blue CanyonはZYNQ7000をCubeSatのバスに使っていますよ。

**synth**
上海にある教育事業をやっている会社のようです。

**thrice.pi**
2人の会話を邪魔したくないのですが、1つだけ質問させてください。Mikeさんも先ほど聞いていましたが、Skycoinのノードが動作するために必要なスペックは何ですか？

**synth**
CubeSatの打ち上げにはいくらかかりますか?200個で3百万ドルくらいですか?

**mike**
デュアルコアのARMと附属のFPGA、GIOとPWMでしたかね。 

**synth**

> Skycoinのノードが動作するために必要なスペックは何ですか？

2GhzのARM板と1GBのRAMが動作するようにしたいと思います。理想的には、ですが。 

**mike**
1U人工衛星につき5万ドルが市場価格ですが、値段は落ちてきています。

**synth**
Skycoinはミニマリストです。bitcoinやethereumと比較してリソースの消費も非常に低く、帯域幅の仕様も10KB/秒以下となるでしょう。

**thrice.pi**
返事をありがとうございました。
次のICOはいつになりますか？

**mike**
現行のBitseed V2でノードは動作するのですね。デュアルコアのArm板で、1GBのRAM、1Gのethernet、SATA、4GBのeMMCというスペックです。

**synth**
次のICOはマーケティング目的ですが、7月20日に実施されます。
大きな取引所への上場とその他のマーケティング、PRの取り組みのはじまりとなるイベントです。
デュアルコアARMであればbitcoinやethereumもマイニングできますね。

**thrice.pi**
ICOはどれくらいの期間開催されますか？

**michaelthecryptoguy**
techbytesが良い質問をしていましたね。 >>>>> Skywireや合意形成アルゴリズムのノードとなるためにはSkycoinを保持する必要がありますか？例えば、他のコインでいうマスターノードのよう仕組みはありますか？ 

**synth**

> Skywireや合意形成アルゴリズムのノードとなるためにはSkycoinを保持する必要がありますか？例えば、他のコインでいうマスターノードのよう仕組みはありますか？ 

いいえ、それはありません。基本的なサービスは無料で提供したいと考えています。高品質なサービスを求める場合にはSkycoinが必要となります。コインを保持していない場合、ノードは帯域幅の20%のみをユーザーに提供するような仕組みです。
有料のユーザーは通信がつまることもないですし、スピードも安定感もあるインターネットが使えます。しかし、コインがなければサービスが使えないような仕組みにはしたくありません。
気をつけるべき点は、無料のユーザーの仕様上限を決め手、ネットワークが混雑し過ぎないようにすることでしょう。

**michaelthecryptoguy**
なるほど、素晴らしい。

**thrice.pi**
7月のICOはマーケティング目的だと言っていましたが、次の質問が指している内容も意図は同じですか？ "元々計画にあったように、Skywireのノード参加を促すための報酬を与える予定ですか？"

**synth**
人びとをネットワークに加わらせるのは比較的簡単です。一旦加わってしまえば、32のノードのクラスタをセットアップする方法、linuxの操作方法、コマンドラインの使い方、10Gbpsのアップリンクとケーブルをご近所に繋げて、屋根にwifiのノードを取り付けて、などのマイナーになるための作業を人びとは学ぶわけです。

**thrice.pi**
lol

**mike**
USBとethernetのポートが付いた仕様のOrange PiのPCを使うことになるようですね。. http://www.orangepi.org/orangepipc/ orangepi.org orange pi pc - Orangepi

**synth**
40Ghzの指向性アンテナ、人工衛星、または街の間のトラフィックを輸送するにはドローンも有効ですね。もし実現されれば、マイナーとハードウェアのイノベーションはすさまじいことになるでしょう。
Skycoinのメンバーに、有機半導体を用いたフェーズドアレイレーダー、フラクタルアンテナについて博士論文を書いた研究者がいます。彼は今すぐにでもSkycoinのマイニングハードウェアのためにアンテナを作りたいと言っていますが、まずはソフトウェアの開発を終えなければなりません。

**mike**
Bitseedを使ってそれをやりたいですね。それまではBitcoinのマイニングで我慢しましょう。

**thrice.pi**
Skycoinの構想はものすごいですね。しかし、詳しくないユーザーにとっては、全貌を理解するのが難しそうです。例えば、そのためにarkをSkycoinのゲートウェイとして使うことは可能だと思いますか？そうすれば、シンプルで簡潔な仕様のArkを通して、普通のユーザーもSkycoinの革新的で複雑なネットワークに参加できます。

**synth**
Mikeさん、あとで設計ファイルを送りますから、今からでもマイナーを組み立て始められますよ。まだ工場はなく、同時に30台のマイナーを組み立てるのも現段階では難しいのです。

**thrice.pi**
上の質問が既にされていたとしたら失礼しました。どの質問もとても良いものです。

**mike**
アンテナはグラフェンインクを使えばよいですよ。利得も200dBの増加となり、CubeSatとも相性がいいです。

**michaelthecryptoguy**
これは良いプロジェクトですね。 :dancing: 第三世界に生きる個人の人間が :sun: (self :this:owned) 自ら金融機関とテレコム企業を代替することができるのです:bananadance::goodjob: :hadouken: あとは彼ら彼女らにスマートフォンを持たせる手段があれば完璧ですね :partysaurus::tophat: (edited)

**mike**
マイナーの構築にはとても興味があります。組み立てに時間がかからない、低コストのパッケージングを考えつく必要があるかもしれませんね。ストレージ機能のある定位置のハードウェアのノードと、メッシュネットの付いたオープンソースのモジュラーモバイル。安定な、暗号化されたグローバルネットワーキングがSkycoinによって実現されるわけですね。

**synth**
定位置であるのが重要です。ノードが動いては問題が色々ありますから。
Skywireが可能なのも、ポイント・ツー・ポイントのセグメント上で動作するです。モバイルアドホックネットワーキングのように、人びとが動き回る場合には不可能です。 

**arc-over-water**
Skywireの基本的なプログラムは公開されていますか?現時点ではウォレットのみが公開されているのでしょうか?

**mike**
そうなると、ルーティングテーブルは頻繁には更新されないわけですね?

**synth**
https://github.com/skycoin こちらでSkycoinの様々なアプリケーションが見られます。
https://github.com/skycoin/bbs 現時点で既に動作しているものです。
ルーティングテーブルは新しい接続先が見つかったときのみ更新されます。例えば、10個以下の接続先を公共鍵に結びつけたとして、何個かが接続を解除したので、新たな接続先を見つけるとします。これはパスと転送方法に冗長性があることを意味しています。ダイバーシティルーティングと言います。
ノード間の直接接続の変わる頻度は少なく、10秒間隔以下が標準になります。もちろん、決して変わらないのが理想的です。物理的な接続に関する変化は更新の波を引き起こし、ネットワークのトポロジーを変化させてしまいます。この変化は最小に抑えられなければなりません。
接続の中断、新規接続やルートの確立はネットワークのトポロジーを変化させず、帯域幅にも影響を与えません。 
近距離のモバイルアドホックルーティングはBATMANのような別のプロトコルを必要とします。逆に、WiFiのホットスポット、都市間のファイバー、イーサーネットケーブルのように固定化されたインフラは、Skywireで代替可能になります。例えば、コーヒーショップにいって、30分間の接続をするのは大丈夫です。しかし、車を運転しながらの異なるホットスポットに5秒毎に接続するようなことはできません。モバイルには別のレイヤーのプロトコルが必要になります。

**mike**
つまり、情報の転送が邪魔されなければノードは動いても大丈夫なのですか？ビームフォーミングアンテナで、ビームの速度が限りなく速くできれば、コミュニケーションを邪魔することもありません。これならばノードが動いても大丈夫になるでしょう。

**mike**
情報の転送が邪魔されなければノードは動かせます。
小さなタワーやアクセスポイントでは実現可能かもしれません。手のひらサイズのモバイル機器だとしたら他のプロトコルが必要になるでしょうが。

**synth**
フェーズドアレイレーダーもよいでしょう。シグナルが数秒、もしくは数時間途切れたとしても、また戻ってこれば問題ありません。
しかし、ネットワーク・トポロジーへの根本的な変化の場合は影響が出ます。ネットワーク全体のルーティングに関わる人たち全員が通知を受けるからです。そのためP2PでCXOを通して更新がされなければなりません。最終的にネットワークはセグメント化される必要があります。それぞれのノードが、区画化されたルーティング、登録ドメインに属するようになります。
現行のインターネットでは2者間のホップ数は40か80だったか、とにかく正気でない数字です。Skycoinではホップ数は最大でも7、平均では4になります。家庭から近所、近所から都市、そして国、目的地へと転送されます。
フェーズドアレイレーダーの利点は、屋根に設置するだけで、誰でも接続可能な相手に接続されるということです。他の人につなぎ直したり、最も条件のよい相手に自動的につながれるのです。屋根に上がってアンテナの向きを調整したりする必要もありません。ソフトウェアによってビームはコントロールされるのです。 
BBSとVPNは私のお気に入りのアプリケーションです。なぜなら、物理的に新たなインターネットを作らなくても、それらは動作するからです。既に存在するインターネット上でも役に立つアプリケーションです。実際にハードウェアのレベルでインターネットの次の姿が表れるのは数年後の話でしょう。 例え、月間10万人がノードをインストールして、毎日1%のペースで成長しても、現在のインターネットを代替するためには10年から15年はかかるでしょう・
機材もたくさん必要になりますので、例え成長速度が驚くべきものとなっても、実現には長い時間が必要とされます。

**mike**
その点は私も気に入っています。手動ではなく、自動調整されるアンテナは必要不可欠ですね。低い周波数を設定して、ノードがGPS機能を使って互いを探せるようにするのもよいかもしれません。そして高い周波数を互いに接続するためのものとするのです。 

**synth**
VPNはSkycoinの主要アプリケーションとなるでしょう。ハードウェアVPN、家全体のVPNです。接続すれば、家全体のコネクションがVPNを通したものとなります。 
インターネットサービス・プロバイダは現在、集めたデータを自由に売ることができるようになっています。
これに対して、ハードウェアの段階で広告やトラッキングサービスに紐付けられているIPアドレスをブロックできるようになります。ローカルネットワーク内の異なるデバイスにはそれぞれのVPNエンドポイントが割り当てられ、デバイス間で自動的にスワップすることも可能になります。
今後、全てのトレントサイトやコミュニティはアンダーグラウンドに追いやられるでしょう。そして、インターネットサービスプロバイダーによってダウンロード速度が調整、またはブロックされるようになるでしょう。このときこそ、新たなインターネットの出番です。将来的にブロックされるコンテンツを、今と同じように自由にアクセスできるようにするための場所です。
5年前であれば問題なかった話でしょう。しかし、今日、新たなものを必要とする環境が整いつつあります。 
他には、redditのようなオンライン掲示板がボットによって荒らされ、投票数やコンテンツが操作されている問題もあります。フェイスブックやツイッターは企業によって完璧に支配されてしまいました。
このような状況で、人びとは分散型のインターネットを求めるようになるでしょう。ボット操作の問題、金による広告の操作、金による情報操作など、数ある現行のインターネットの問題を解決できる新しいプラットフォームへの、大規模な移動が始まるのです。
分散型のツイッターやフェイスブックを作ろうとする試みは以前もありましたが、5年前には必要ありませんでした。現在、人びとも技術も移行を始めることができる段階に入っています。
Skycoinはこの最も基礎的なレイヤーを作っており、コミュニティがアプリケーションを開発しています。私たちはただ、ツールを提供するだけなのです。 

**mike**
ネットの集権化の問題は深刻になりつつあります。例えば、私のツイッターアカウントで、理由もなくメールアドレスが公にされてしまったことがありました。重複していたプライバシー通知を止めてもらうように頼みにツイッターに行ったら、その理由もわかりましたが。 
SkycoinとArkをつなげて、SkycoinのVPN上でArkが稼働するようにしたいですね。SkycoinのVPNは他の選択肢と比べて非常に分散化されています。

**xano**
Skycoinは違法行為に最高のプラットフォームだという印象を抱いたのですが、これはSkycoinの将来と大衆による受容にどう影響を与えるでしょうか?

**charles**
Skycoinがどのようにredditのボット問題を解決するのかわかりません。

**xano**
Skycoinの構想はよいですね。誰もが無料で映画、ドラマ、音楽を楽しみたいと思っていますから。しかし、例えば、ISISが利用し始めたらどうします？

**synth**
まず、ツイッターの問題です。実際、ヒラリー・クリントンは「ブランド・マネジメント」という建前でツイッターに金を払い、彼女についての否定的なツイートがフィードに上がらないように操作していました。逆に、4000人中の1人でも肯定的な意見を発した場合には、その人をフォローしている全ての人にそのツイートがフィードに表示されるようにしました。
企業は人びとがアクセスする情報を操作しています。フィードに表示される内容を意図的に編集するようでは、自然な形とはいえないでしょう。ユーザーの好みはもはや関係なく、プラットフォームを広告主の好みと金で変えられるようにしてあるのです。社会的なアジェンダを拡散するのにさえ使われており、プラットフォームにお金を払って、特定の人間やムーブメントを検閲するようにさえ仕向けています。
Googleでさえトレンドからは自由ではありません。Fortune500の企業が年間700億ドルの広告収益を盾にして、Googleが検索結果を広告主にとって有利なように操作することを約束させました。また、企業や政府の言うことに従わなければ、大量の罰金を支払うようにという制約がEUでは設けられています。
分散化されたソーシャルメディアでは、ユーザー自身がデータを所有します。自らのコンピューターで、自身のフィードを分類化、優先化しているアルゴリズムを管理します。金と政府の下僕となっている第三者の企業に情報が操作されることはありません。
もちろん、ARKはSkycoinのネットワークを使い、ブロック生成と処理の分配を行えるでしょう。インターネットからブロックされることなく、ネットワーキングができるでしょう。
そしてSkycoinと同じフレームワークとクラスタ内に、ARKをノードとして設計することもできます。
https://github.com/skycoin/viscript ここにARKを追加することができます。最終的には、異なるプラットフォーム間のCLI、アプリケーション実行プログラム、また、クラスタマネジメントが揃う予定となっています。

**mike**
どうもありがとう。デベロッパーたちに伝えておきます。私たちは現在、様々なプログラミング言語のためのAPIとCLIをARKに追加していますので。

**synth**

>Skycoinがどのようにredditのボット問題を解決するのかわかりません。

Skycoinのプロジェクトの焦点ではありませんが、BBSを開発しているデベロッパーたちが作ったフィルター用アルゴリズムがあります。これは参加者の公開鍵により身元証明がされ、信頼の環を作ることで、分散化と自動化されたモデレーションの仕組みができるのです。それぞれのユーザーの言動に対する評価がなされます。
ところでARKの開発言語はgolangですか?

**jarunik**
ArkのブロックチェーンはJavascriptですが、golang用のAPIがあります.

**arc-over-water**
なぜrustやscalaではなく、golangなのですか?

**mike**
Arkのコアはnode.jsで書かれています。goに対応させることも可能かもしれません。@christがgo用のAPIとCLIを既に作っていたと思います。

**arc-over-water**
lispで書かれたコインはいつ生まれるのでしょうか？ :slightly_smiling_face:

**mike**
golangにも対応可能なようです。素晴らしい!

**boldninja**
https://github.com/ArkEcosystem/ark-go GitHub ArkEcosystem/ark-go ark-go - Ark GO client for ARK.io blockchain ecosystem #golang #ark #blockchain

**mike**
lisp - それも良いでしょうね!まだlispが存在していることは驚きですが、機械学習のアプリケーションによく使われるようですね。lispも追加する必要があります。arc-over-waterが担当してくれるのでしょうか?
lispは並行処理の機能を開発するのに向いていそうですが、詳しくは知りません。

**arc-over-water**
Shenもあるようですね.. http://shenlanguage.org/

**synth**

>Skycoinは違法行為に最高のプラットフォームだという印象を抱いたのですが、これはSkycoinの将来と大衆による受容にどう影響を与えるでしょうか?

薬物のディーラーはSkycoinを重宝するでしょうね。Bitcoinは人々が薬物を購入し始めるまでは無価値でした。1年で0.01ドルから1000ドルに上がったのは薬物購入のおかげです。
インターネットが最初に作られたとき、最初に人々がしたことはポルノ動画のダウンロードでした。Bitcoinが最初に作られたとき、最初に人々がしたことは薬物と銃器の購入でした。
しかし、ISISはSkycoinを必要としないでしょう。なぜなら、ISISはxboxとfacebookのメッセンジャーを使っているからです。暗号技術は必要ないのです。テロリストの攻撃がある度に政府の予算は大きくなるので、政府はISISを必要としています。テロリズムは金を生む箱であり、恐怖が大きくなれば、それだけ生まれる金も増えるのです。ISISはたくさんの金を世の中に生み出しました。このためにテロリズムの問題はなくなるまで時間がかかるのです。
幼児虐待者もステガノグラファー、i2p、tor、tails、bitmessageなどの技術を受容した最初の人々でした。その後も、この類の人びとたちが暗号技術のプロダクトを最初に試そうとするという事実は変わりません。ステガノグラファーのロゴを見てみれば、どのような種類の人間がそれらの技術を開発したのかわかるでしょう。
これはSkycoinの場合でも似ています。公開される2年も前の段階に、機密情報組織の人間やマネーロンダリングの専門家たちがプロジェクトに加わり、メタデータのスクラビングや保護に必要な技術の詳細を共有していきました。
もし私が次のシルクロードを作るとしたら、Skycoinが開発しているような技術を使うことでしょう。誰もがそう思うはずです。
人びとがこの技術をどのように利用するかは私たちのコントロールを超えています。進歩には付きものの問題であり、それはSkycoinにしろMaidSafeにしろ、必ず起こることです。

**mike**
とても興味深いですね。juliaのウェブサイトは見たことがありますか？ https://julialang.org/ このベンチマークは驚くべきものです。
テロリズムを終わらせるには外国への干渉をやめることだと私は思います。 少なくとも、スイスはテロリストの問題を抱えていません。

**arc-over-water**
killaryとobombaですか。

**michaelthecryptoguy**
それは悲しいことながら真実です。

**mike**
そしてbushesですね。

**synth**
uploaded this image: Screenshot from 2017-06-29 14:42:25.png Add Comment

**synth**
uploaded this image: Screenshot from 2017-06-29 14:41:55.png Add Comment

**arc-over-water**
驚くレベルのフェイクニュースが世に溢れていますよ... サンディフック.. 911
月面着陸... Stephen Hawking...
やれやれ..

**charles**
北朝鮮もテロリズムの問題を抱えていませんね :)

**arc-over-water**
空の広さにも限りがあるということですね!

**mike**
そこまで論理を飛躍させずとも、ロシアによるアメリカ大統領選挙への干渉、トランプ大統領とロシアの繋がりを考えてみてください。つまるところ、戦争の存在は企業的国家の健康度を示すものなのでしょう。

**synth**
今やテロリストによる攻撃は、Nikeの宣伝広告と化しています。最新のISISによる攻撃のニュース報道に、どの会社の製品の広告掲載するかで競っているのです。このような報道があれば人びとはテレビに釘付けになりますから。逆にこのような事件でなければ、ニュースなど誰が見るでしょうか？テロリストによる攻撃は人びとをテレビに釘付けにし、そのチャンネルと時間の広告枠を確保しようとFortune 500の企業が争っているのです。
政府や素早いサメのように国民を監視するための法案を作り、企業から必要のない機器を何兆円も買い集めるのです。政府機関は報道機関を操作して、予算の上乗せのための法案を通してしまいます。これは狂っている


**mike**
it would be very inconvenient to improve relations with Russia for those making money and expanding power over escalating global tensions.

**arc-over-water**
wasnt the first main scandal trump attack that he weed on some prostitutes in Russia. OMG

**synth**
they have oil companies and russia produces oil; so hey want any execuse for "sanctions" to force people to buy their oil instead of russian oil. They would do a war, just to stop any Russian oil pipeline to Europe.
It just about money.

**arc-over-water**
Putin is actually kicking some ass with his speeches the last years.

**synth**
if russia gave me free prostitutes, I would pee on them too, lol. Why not? (edited)

**mike**
don't forget Pussygate - the press sat on the tape for 10 years until 3 weeks before the election, instead of during the primaries.

**arc-over-water**
crazy shit out there...
time for crypto to shine..

**xano**
I just wonder how services like mega would have ended up with Skycoin

**synth**
the "Y2K" was also excuse, to sell tens of billions of dollars of "upgrades" to government and corporations. They told them "give us your money or the sky will fall".
terrorism is the same story, its just turned into a money making scam. 90% of the surveilence crap is just companies finding excuses to lobby the government to buy over priced equipment, so they can make money. They do no even know what to do with the data they collect. They are doing insider trading and rigging markets and all sorts of crap with the data and then panicing when people start using HTTPS because its harder for them to keep making money the same way.

**arc-over-water**
Mega2 is about to show its prototypes

**synth**
you have mom and pop local police departments, buying $150,000 string ray cell phone interception equipment that is NSA level, who could not even afford it, but its paid for out of 10 billion dollar DHS "terror" fund to buy useless equipment for local police. To "fight terrorism". Its really a joke.

**arc-over-water**
Sky list of aims over the next two years?
Next ICO cost and how it will be released?

**synth**
people know that companies like apple and goolge are required to hand over all their data to the government. including messages, so why would anyone use imessanger or icloud?
So they are staging fake events with "police cant break the 4 digit pin on an iPhone and its unbreakable" when they can actually trojan the phone from the carrier, etc and have all sorts of insane mandatory backdoors.
So we are heading towards a decentralized internet and these new apps, as people get sick of being tracked like animals.

**michaelthecryptoguy**
@synth What is your background? Can you tell me a little about your prior experience, regardless of what area it was in? (edited)

**synth**

> Sky list of aims over the next two years?

Get meshnet working Get BBS and first demo apps working Get VPN working and get it to users List on more exchanges Build up community Improve the wallet, fix website, translations into more languages ec

**arc-over-water**
Also the two Chinese guys who wrote the technical whitepaper, the scholars, are part of the team?

**synth**
@synth What is your background? Can you tell me a little about your prior experience, regardless of what area it was in?
I did a lot of things. video games, hedge fund/finance, crypto, investment stuff etc... Now am I a sort of project manager.

**charles**
How will the price of skycoins be determined for the next ICO, I, suppose it cannot be above market price, else people would not buy it, but too far below would depreciate the coin

**arc-over-water**
do they want high price at this point or well even distribution to the best placement of people?

**synth**

> Also the two Chinese guys who wrote the technical whitepaper, the scholars, are part of the team?

One of the chinese guys has nothing to do with it. He is a professor that put his name on paper his graduate student published. And now the professor wants to hide the paper, because he thinks the chinese government is cracking down on bitcoin; but he is wrong and the government doesnt care and the paper is in english so they cant read it anyways.
And the other one is a core ETH developer. Chen was core ETH and wrote the golang implementation of Ethereum. He is not very public and does not want to be in spotlite or bothered.
most of the contributors for skycoin are in the background or hiding actually (edited)
many of the ETH people are all whoring themselves out to advisor boards to various tokens, or dozens of tokens and ICOs; but most of the serious crypto people are very private and hiding themselves. They do not want to be known, do not want to promote or advertise themselves and they are in the background.
Or they have too much money already and just want to hide. They are also lazy because they do not have to work anymore, or they are busy with other things.
they also want to avoid taxes and being targetted for theft and do not want attention from government
skycoin cannot have a "Team" or "Advisor Board" on website, because we asked everyone and no one wants to be public or wants to be in a public position....

**arc-over-water**
yes best to live in a country your not citizen of and earn money from a country your not living in... Been doing it for ten ears, way less stress, (edited)

**synth**
many early bitcoin people, who identified themselves publicly on twitter; they cannot travel to brazil or certain countries without risking being kinapped and ransomed for money
lololol

**arc-over-water**
vitalic knows kung fu maybe,,, well he speaks Chinese..

**charles**
Do you think skycoin not having a public figure will negatively affect adoption?

**arc-over-water**
i think it has.. 6 years on and quiet forums and slack

**synth**
we can buy public figures or an adviser board; but they would not have anything to do with project except to put their name on it to create confidence for public; which is what all these advisor boards really are

**arc-over-water**
in the background assuming tek development.
Next ICO cost and how it will be released?
github is always active...

**synth**
i really do not know
about the next ICO

**arc-over-water**
ok

**synth**
it is around the 20th of next month. and will be 1% to 10% of the skycoin. I am not sure the exact number is set
and it will probably be a fixed price

**dr10**
this ama is a marathon :trollbounce: nice!

**arc-over-water**
how much of the 100 million is obligated to your team and the people who funded it?

**synth**
but then followed by a weekly auction or second priced auction for a fixed number of coins, that will occur every week for 8 weeks; but not sure how many coins or if it will actually happen

**arc-over-water**
so if its a high price it is 1% and low price it could get to 10%

**synth**

> how much of the 100 million is obligated to your team and the people who funded it?

The people who funded skycoin, did not receive anything for it. They have no entitlement to the coins.
they had to buy in at ICO like everyone else. Even the developers working on it, had to buy in.

**arc-over-water**
ok so they have already been looked after in the 10c ICO round

**synth**
i think the next ICO is mostly marketing event, and to "get it over" with. We are in a bubble now, so we should raise money now, before the ICO bubble pops. Is what people are telling us.
we cannot spend more then 50 million, so selling an insane number makes no sense. 10 to 15 million is probably reasonable, for next 3 years. And that is with a really good full time marketing team, and trippling number of developers AND funding several parrallel hardware projects.

**mike**
My approach to Skycoin is regardless how much of a financial return it might provide, it is an investment into producing a future I want to see.
Also look forward to earning it by running nodes.

**arc-over-water**
So that could be you release 10,000,000 coins and get $10,000,000 dollars for your covering expenses next three years

**charles**
Can a person with limited technical capabilities run a node?

**arc-over-water**
or $20,000,000 as it goes

**synth**
the people who are going to pump the coin, want us to sell off as much as possible. They are pressuring us to do that.
However, if we sell fewer coins, then the price per coin will be higher.
If we only sell 10 million in coins, then the price can go up a lot higher than if we sold 500 million in coins.
I think EOS is going to raise a billion dollars and I have no idea what they will with the money, except use it to buy EOS and drive the price up or some scam. They are not going to spend it on development. lol
> Can a person with limited technical capabilities run a node?

eventually, yes. maybe not right now. after tutorials, yes

**arc-over-water**
EOS seems like it is trying to go bear bones and not be as complicated as ETH...

**mike**
I think it is smart to hold a lot for distribution to node operators as a replacement to mining for a good distribution, also selling some to have distribution among those who are interested but not technically inclined to run nodes.

**synth**
So that could be you release 10,000,000 coins and get $10,000,000 dollars for your covering expenses next three years
The coin price is like $4 or almost $5 at high. It will be at $5 by ICO I think, atleast. The market cap has doubled every 40 days, for a while now.
10 million coins at $5 per coin, is 50 million.
We have to distribute coins via the skywire nodes, to make it fair; because ICO is not a good way to get coins into the hands of users. Its only good for fund raising and for whales.
We decided that we will distribute most of the coins to users and just use sales to whales, to fund development.

**arc-over-water**
there must be ways to spread to diverse groups the 10,000,000 coins?

**synth**
the problem is that all ICOs end up going to less than 20 whales

**arc-over-water**
every member of a altcoin slack gets a coupon invite
If an ICO knows their customer that can be prevented..

**synth**
there are people who own a large percentage of ETH and they want to diversify; they can gamble 20 million in an ICO and could make 50x more, but if they lose it, then its a slight loss; they have so much ETH that they cannot even sell it or convert it, without tanking the market

**arc-over-water**
in one day every altcoin slack member of every altcoin could get a btc address used once in their pm, allowed a max amount sent etc..

**synth**
yes, ideally, that might work
we have been doing OTC sales at market price; with a cap of 10 BTC and that works well

**arc-over-water**
do the OTC reflect in the blockchain? (edited)

**synth**
but we have single whales that want to put in 700 BTC and each one individually, is larger than whole individuals doing the OTC sales
OTC is "over the counter", or direct sale; when people private message a developer and ask to buy

**arc-over-water**
ok so private sales are happening

**mike**
uploaded and commented on this image: TEC chart.png 1 Comment Here is a sample method based on power law for pricing I have planned for Ark based Token Exchanges for projects, including funding Ark/Skycoin based nodes. As more as sold, the price increses by a power law so people can enter at the irsk and expected ROI combination they feel comfortable without being pressured into hasty emotional decisions by FOMO.

**mike**
*irsk=risk
so entering on any part of the curve looks the same as any other part.

**synth**
hmmm
how does this work?
the more money you put in, the more you pay?

**arc-over-water**
but as you do these OTC sales it reflects here in distributed? http://explorer.skycoin.net/blocks

**mike**
here is a link to the spreadsheet, has the formulas and table of calculations for the graph, https://docs.google.com/spreadsheets/d/1en9lqzBIuHgp0-Q3ohoq3yJUe1lJcOK9U4bF2TiXZew/edit?usp=sharing
yes, the more that is put in, the higher the price.
it will take some experience to determine the best parameters to prevent instant sell-off while not stalling the exchange indefinitely, and different project might be best suited for different exchange rates over time period.

**synth**
we have a really good strategy now
We can distribute coins to top content producers on the BBS
to people doing bountries (like skycoin logo, sticker design etc)
to people who want to do development (mobile wallet etc, some features for bbs and bug fixes)
Then massive substained distribution, over time to the people running the skywire nodes.
Then disribution also to nodes hosting content on CXO.
Then distribution to people coming on to platform who are bringing user communities with millions of people (we have been talking to these people for years and they do not have real developers, so we have to help them; they only have web designers and curators and community managers but cannot actually develop anything new).

**mike**
like a long term term ArkSpace project for space exploration and development will be sold over a lot longer time frame than funding an index coin bridged to Ark.
yes, and either way, the project can award blocks of tokens to contributors other than just for money.
I'm a fan of the Slicing Pie method.

**arc-over-water**
Ok so your saying it will be between 1%-10% next month to get funding and start the marketing campaign. Then after that distribution then there are monthly small releases of ICO and the majority being bounties for services rendered. and nodes etc

**mike**
http://slicingpie.com/ Slicing Pie Perfect Equity Splits for Bootstrapped Startups Slicing Pie is a formula that allows founders to create a PERFECTLY FAIR equity split between founders, investors, partners and employees. (92kB)
Skycoin is very similar, but doing it manually with adjustment.

**synth**
yes
what i am interested in, is if we can block the BBS up and get alot of users with the incentives
every dollar in coins we sold over OTC, drove the skycoin market cap up $4
we would sell coins, then price explodes the next week; because people promote it on twitter and blog about it
skycoin needs to get on more exchanges

**synth**
I have to sleep now. LMAO. We should end AMA soon

**arc-over-water**
cool thanks for your time... haha 3.17 am here

**synth**
4 hours?

**dr10**
XD

**synth**
is there an archive for the AMA?

**dr10**
reddit hopefully :joy:

**michaelthecryptoguy**
Thank You for taking your time to answer everything in complete detail. It was nice that you cared enough to make sure everything was answer very thoroughly.

**boldninja**
@michaelthecryptoguy can you copy everything and make it reddit friendly?
thanks @synth for taking the time for this AMA it was :mindblown: really interesting stuff

**techbytes**
marathon session today.

**michaelthecryptoguy**
I sure can. As long as jarunik hasn't already started. (edited)

**mike**
Thank you very much for joining us synth, please stop by again.
I will also be continuing to check in on skycoin slack for updates as well,
[skycoin.herokuapp.com](https://skycoin.herokuapp.com)
The closer the integration of Skycoin with Ark, the better.