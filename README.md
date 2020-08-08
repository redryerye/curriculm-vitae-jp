# 職務経歴書
Ruby On Railsを用いたWEBアプリ開発を１年ほど行った後に、渡米。大学でデータ構造・アルゴリズムを学び、友人が起業する会社に参画しました。iOSアプリを含む[VALL](https://vall.app/)の立ち上げを担当。他にはチームビルディングをしたり、Nuxt.jsとAWS Cloud Formationを使ってフルスタックで開発したり幅広く開発をしています。現在もSwiftが好きで、業務では主にiOS開発の比重が大きいです。

## 基本情報
|||
|---|-----|
|Name|山本裕貴 (Yuki Yamamoto)|
|Twitter|[@redryerye](https://twitter.com/home)|
|Github|[@redryerye](https://github.com/redryerye)|
|Speaker Deck|[@redryerye](https://speakerdeck.com/redryerye)|
|Qiita|[@redryerye](https://qiita.com/redryerye)|
|LinkedIn|[Yuki Yamamoto](www.linkedin.com/in/iamyukiyamamoto)|

## 職務経歴

### アマトリウム株式会社

CTO (2018/08 - 現在)
- **iOS向けアプリの開発**
  - [役割] iOSエンジニア(1人体制)
  - [技術] Swift, AWS(Cloud Formation, App Sync, Cognito, DynamoDB, Cloud Watch), Firebase(Analytics, Cloud Message), [Datomic Cloud](https://docs.datomic.com/cloud/index.html), [Dark](https://darklang.com/), ライブラリ等([KingFisher](https://github.com/onevcat/Kingfisher), [Nuke](https://github.com/kean/Nuke), [SwiftGen](https://github.com/SwiftGen/SwiftGen), [Alamofire](https://github.com/Alamofire/Alamofire), [SwiftJWT](https://github.com/IBM-Swift/Swift-JWT), [ReactiveSwift](https://github.com/ReactiveCocoa/ReactiveSwift))
  - [担当箇所、凝った箇所、悩んだ箇所など]
    - **FatViewcontroller**
      - Reactiveなフレームワークを使わなくてもシンプルに実装出来る[MVVMを実装した](https://speakerdeck.com/redryerye/implementing-mvvm-in-2019)。スタートアップなのでReactiveを習得する学習コストを払う余裕がなかった
      - 後にReactiveSwiftを導入して整備した
    - Assetがプロジェクトが成長するにつれて肥大化した
      - SwiftGenを用いて一箇所にまとめ、動的に生成することで変更や管理が楽になった
    - Immutableなデータ構造を実現するためにDatomicをバックエンドに採用
      - チームのアーキテクトの発案でClojureで実装するDatomic Cloudをデータベースに使用した。各データがDatomic上で保有する[Datoms](https://docs.datomic.com/cloud/whatis/data-model.html)と言うデータタイプを使うことで、他のプラットフォームでは実現できないフレキシブルなスキーマ設計が可能になった
    - バックエンドエンジニアの体調不良をカバー
      - 2020年冒頭よりバックエンドを担当していたエンジニアが健康上の理由により急遽抜けた。そこから自分がAWS Cloud Formation用いたクラウド開発も含めてフルスタックで開発。ドキュメントの大事さを噛み締めた。
    
- **WEBアプリ開発**
  - [役割] フロントエンジニア(2人体制)
  - [技術] Nuxt.js, Vue.js, AWS(Cloud Formation, DynamoDB, Cloud Watch, Cognito), [Stackery](https://www.stackery.io/), Firebase(Function), [Datomic Cloud](https://docs.datomic.com/cloud/index.html), [Dark](https://darklang.com/)
  - [担当箇所、凝った箇所、悩んだ箇所など]
    - コンテンツの管理担当者を分担するために社内ツールを作成
      - 作成したアプリケーションのCMSとして[Retool](https://retool.com/)で社内ツールを作成した
    
- **tvOS向けアプリの開発**
  - [役割] フロントエンジニア等(1人体制)
  - [技術] Swift, ライブラリ([Multipeer Connectivity](https://developer.apple.com/documentation/multipeerconnectivity))
  - [担当箇所、凝った箇所、悩んだ箇所など]
    - iOSからの操作性を向上させるためにMultipeer Connectivityで通信するデータ量を最適化して減らした
    - tvOSの知見がインターネットで少ないのを知った（これをきっかけに[登壇](https://speakerdeck.com/redryerye/implement-p2p-connection-and-stream-your-content)を決めた）
- **チームビルディング(エンジニア採用、スクラムの導入)**
  - [役割] プロダクトオーナー
  - [担当箇所、凝った箇所、悩んだ箇所など]
    - チームのメンタル管理とプロダクティビティの向上
      - チームに根ざしたスクラムに変えるためのイテレーションを重ねた。レトロスペクティブの進め方を定期的に変えることでマンネリ化を防止し、チームの活性化につながった
    - リモート化の対応
      - コミュニケーションの機会を増やすため、開発者間のコラボレーションの多いタスクを作るようにした事でチームとしての一体感を取り戻せた
      


---

### 株式会社メディオテック

インターン (2016/12 - 2017/07)
- **施工管理のWEBアプリケーションの開発**
  - [役割] フロントエンドエンジニア
  - [技術] Ruby On Rails, MySQL
  - [担当箇所、凝った箇所、悩んだ箇所など]
    - 初めてのWeb開発
      - MVCを意識した開発を学べたほか、MySQLでのデータベース管理を習得した
      - 複数人で開発する時は命名規則が特に大事だと思った

## 登壇実績
|Year|Title|Event|
|--|--|--|
|2020|(Upcoming) [In App Purchaseのこれからの在り方を考える](https://fortee.jp/iosdc-japan-2020/proposal/36676fca-9823-4a22-a90b-8eb2e98f4b1a)|iOSDC Japan 2020|
|2019|[tvOSにちょっと注目してみる](https://speakerdeck.com/redryerye/tvosnitiyotutozhu-mu-sitemiru)|iOSDC Japan 2019|
|2019|[Implementing MVVM in 2019](https://speakerdeck.com/redryerye/implementing-mvvm-in-2019)|Otemachi.swift|
|2019|[Implement P2P connection and stream your content](https://speakerdeck.com/redryerye/implement-p2p-connection-and-stream-your-content)|try! Swift Pre Talks 2019|
