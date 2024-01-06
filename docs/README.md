# 職務経歴書

## 基本情報

**フロントエンドエンジニア**

| key      | value                       |
| -------- | --------------------------- |
| 氏名     | 菅原 康平（Sugawara Kohei） |
| 生年月日 | 1987/10/31                  |
| 居住地   | 神奈川県                    |
| 最終学歴 | 北海学園大学英米文学科      |

---

## 経歴サマリー

WIP

---

## 各種アカウント

<a href="https://github.com/suzy1031" target="_blank"><img alt="GitHub" src="https://img.shields.io/badge/suzy1031-%2312100E.svg?&style=flat-square&logo=Github&logoColor=white" /></a>
<a href="https://qiita.com/suzy1031" target="_blank"><img alt="Qiita" src="https://img.shields.io/badge/suzy1031-55C500.svg?&style=flat-square&logo=qiita&logoColor=white" /></a>
<a href="https://www.wantedly.com/id/kohei_sugawara_b" target="_blank"><img alt="Wantedly" src="https://img.shields.io/badge/Wantedly-21bddb.svg?&style=flat-square&logo=wantedly&logoColor=white" /></a>

---

## 保有スキル

- **プロジェクトマネージメント**
  - ビジネス要件の収集と分析
  - 仕様書の作成と管理
  - 詳細設計の策定と実行
- **UI/UX デザイン**
  - アクセシビリティを考慮したフロントエンド開発
  - UI/UX デザイン原則の実装
  - ユーザビリティ向上のためのコーディング
  - デザイナーとの効果的なコミュニケーションと協力
- **エンジニアリング**
  - JavaScript / TypeScript + React.js / Next.js でのフロントエンド開発・設計
  - Storybook を使用した UI コンポーネントのテスト設計と実施
  - E2E 自動テストの構築と実行
  - GitHub Actions を利用した CI 自動化の実装

---

## 技術スタック

### 言語

<p>
  <img alt="TypeScript" src="https://img.shields.io/badge/-TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white" />
  <img alt="JavaScript" src="https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logo=JavaScript&logoColor=white" />
  <img alt="Ruby" src="https://img.shields.io/badge/-Ruby-CC342D?style=flat-square&logo=Ruby&logoColor=white" />
</p>

### フレームワーク･その他

<p>
  <img alt="React" src="https://shields.io/badge/React-black?logo=react&style=flat-square" />
  <img alt="Next" src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" />
  <img alt="Ruby-on-Rails" src="https://img.shields.io/badge/-Rails-CC0000?style=flat-square&logo=Ruby-on-Rails&logoColor=white" />
  <img alt="Vite" src="https://img.shields.io/badge/-Vite-646CFF?style=flat-square&logo=Vite&logoColor=white" />
  <img alt="Webpack" src="https://img.shields.io/badge/-webpack-8dd6f9?style=flat-square&logo=webpack&logoColor=white" />
  <img alt="Docker" src="https://img.shields.io/badge/-Docker-46a2f1?style=flat-square&logo=docker&logoColor=white" />
</p>

---

## 意欲･興味

WIP

---

## この先やってみたいこと

WIP

---

## 希望条件

子どもが小さく家事･育児を最優先したいため､フルリモートでの勤務を希望します(月数回の出社は可)

---

## 職務経歴詳細

### [ClipLine 株式会社](https://corp.clipline.com/)（2021/09〜現在）

他店舗企業向け動画型実行支援 Saas｢[ABILI](https://service.clipline.com/)｣フロントエンド開発に従事

#### 2023/07~2023/10

**｢ABILI Clip｣管理者向け･エンドユーザー向け web アプリケーション新機能開発**

WIP

#### 2022/07~2023/02

**｢ABILI Clip｣エンドユーザー向け web アプリケーション リアーキテクチャ**

役割：`エンジニアリーダー`･`PM`･`PdM`

チームメンバー：`7 人`

仕様技術：`React`

**背景**

```
従業員(アルバイト中心)向けwebアプリケーション

創業当初からあるプロダクトで､Ruby on Railsモノリシック -> React + Ruby on Rails APIと､アーキテクチャを変えながら様々な機能追加が行われてきた

フロントエンドにはReact + Redux + Redux Saga / Atomic Designが採用されており､開発当時はデファクトスタンダードな技術スタックだったが､このアプリケーション規模では､Reduxを使ったglobalな状態管理は不要で､メリットよりデメリットが目立つようになった

Atomic Designはメンバーにより､コンポーネントの粒度がバラバラになってしまった｡またメンバーも､コンポーネントの依存関係や影響範囲が十分に把握できずに､QAしてもらうことになり､全体工数が膨らんでしまい､リリーススピードが遅い課題があった

また､依存関係や影響範囲が読みにくいため､開発者はファイル名が違う､中身はほぼ変わらないコンポーネントを自身が担当する機能開発の際に作るようになり､UIコンポーネントが爆発的に増えていき､より複雑性を助長させてしまっていた

様々な機能追加がされてきたので､今では利用されなくなった機能もそのまま残っており､アプリケーションを操作するうえで､ノイズになり､ユーザーが複雑に感じてしまっており､活用が定着しない従業員がいる課題があった
```

**アーキテクチャ選定**

```
ABILI Clip LEADでは技術顧問が技術選定の中心となり､Next.jsを採用したが､弊社アプリケーションは､ほぼすべての画面が認証が必要であるため､Next.jsの強みである､SSG･SSR･CSRをページごとに使い分けるメリットを教授できない､サーバを立てる必要があり､サーバ運用コストがかかる､などの理由から引き続きReactを採用した

Redux + Redux Sagaを使い､APIレスポンスを含めた､ほぼすべての状態を中央集権的に管理していた｡ただ､このアプリケーション規模であれば､APIレスポンスはキャッシュを活用し､一部の状態のみglobalに管理すれば十分だったので､Recoil + SWRを採用した

この時期､デザイナーが不在であり､この先いつ採用されるのか不透明であったこと､デザイナーとフロントエンジニアが密に連携して､厳密なコンポーネント管理が必要になるAtomic Designは､弊社の現在の事業フェーズを含めて考えると､この先の運用に無理が出てくると判断し､package by featureなディレクトリ構造へ変更した

package by featureに変更したことで､画面ごとに使われているコンポーネントが1つのディレクトリ内で管理でき､知識が分散せず、機能の把握や機能ごとの分割が容易になった

Atomic Designを採用した時点では､styled-componentsを使い､フルスクラッチでcssを書き､UIコンポーネントを作っていたが､少ないエンジニアリソースで､運用していく + 高速なリリースを実現するためには､ある程度できあがっているコンポーネントと少々のスタイリングでUIが組めるMaterial UIを採用した

Material UIはバージョンが5系になり､v4 -> v5のような破壊的変更が直近では発生しにくいと推測できること､提供されるコンポーネントの種類の豊富さ､runtime cssでパフォーマンスがtailwind cssなどに比べると劣るが､ABILI Clipではシビアなパフォーマンスが求められていない点も加味して採用に至った

コンポーネントの粒度が開発者によってバラバラになってしまう課題に対しては､共通で使うUIコンポーネントは､｢ドメイン知識が含まれるコンポーネントか､含まれないコンポーネントか｣の観点で分割するルールをフロントエンドメンバーで合意した｡

これによりドメイン知識が含まれないUIコンポーネントは､uiディレクトリ配下で管理､ドメイン知識が含まれるUIコンポーネントは､projectsディレクトリ配下で管理､へ変更して､ディレクトリ構造の簡素化が進んだ
```

**実績**

```
新しいアーキテクチャに変更したことで､開発者は影響範囲を把握でき､QA対象範囲が限定できるようになり､QAのテスト範囲を絞れるようになった（リアーキテクチャ前は､開発者もQAも影響範囲を十分に把握することができず､フルなテストをQA期間はする必要があった）

これにより､全体工数が圧縮でき､今まで月1回のリリースが限界だったが､週1回リリースが可能になった
```

#### 2021/10~2022/06

**｢ABILI Clip LEAD｣エンドユーザー向け web アプリケーション 新規開発~エンハンス**

役割：`エンジニアリーダー`･`PM`･`PdM`

チームメンバー：`4~9 人`

仕様技術：`Next.js`

**背景**

```
店舗責任者(店長･スーパーバイザー)向けwebアプリケーション新規開発にて全フェーズを担う

当時､プロダクトラインナップにスマホファーストなwebアプリケーションがなく､拠点外での業務が多い､移動が多いなどの勤務をしている店舗(拠点)責任者が｢ABILI Clip｣を利用できない課題があった｡スマホに最適化された｢ABILI Clip LEAD｣を新規開発に着手
```

**version1.0 リリース**

```
フロントエンジニアとして開発をしながら､詳細設計を作成し､日本メンバー1人･ベトナムオフショアメンバー4人へ落とし込みプロジェクトを進める

また､小売業時代の経験･知見を活かしながら､CEO･CTO･Bizメンバーとコミュニケーションを密に取り､要件･ユースケースの理解を深め､プロダクトへ反映

はじめてQAフェーズに携わり､テスト観点･テストケースの作成から､バグチケットのトリアージなど､設計からQA､またリリーススケジュール管理など､すべてのフェーズを経験
```

**エンハンス開発**

```
リリース後､利用ユーザー･クライアントからいただくVoCや､機能開発を行う

google analytics4やgoogle tag managerを使い､利用者の活用度を継続して観察する中で､コンテンツを新規作成するコア機能を活用していない課題が見つかる｡当初は､新規作成の手順の簡素化や､スマホでこのコア機能が使えることで､コンテンツ作成数が増加すると想定していた

コンテンツは利用クライアント内のABILI担当者が､動画を中心に一括で作成することが多いが､店舗(拠点)責任者は､部下や従業員に対して発信したいことがあっても､動画作成ハードルが高く､活用が進まないのではないか?と原因を調査し､｢店舗(拠点)責任者は､文字ベースでコンテンツ配信できることで､スマホでABILI Clipを利用するメリットをより強く打ち出せるのではないか｣を仮説を立てた

そこでBizメンバーを巻き込み､自身でプロトタイプを開発しながら､通称｢ノート｣機能開発を進める

技術的には､プロダクト全体のコア機能への改修であるため､他の既存プロダクトへの影響が懸念だった｡しかし､クライアントにはやく活用してもらい､フィードバックをもらい､改善サイクルを回したいので､コア機能への影響を最小限にとどめる改修のみ行う決断をする

それにより全体の開発工数を圧縮して､複雑度を低下させることで､高速な機能開発ができた

また､MVPを活用してもらうため､クライアントとのMTGへ参加し､この機能を活用することで､店舗のどんな作業が効率化し､店舗運営コスト削減するか､など提案

実際に利用いただく中で､ヒアリングした機能の不足を追加開発し､改善サイクルを回しながら､β版という形で機能リリース
```

**実績**

```
外食業のスーパーバイザーや､運輸業の拠点長を中心に月間アクティブユーザー約3000人が活用する

自身を中心に機能開発した｢ノート｣機能が､外食業(約1200店舗規模)に導入され､コンテンツ総量のうち､約40%をしめる
```

### miracleave 株式会社(2019/12~2021/08)

SES / 受託にて､主に`Ruby`(Ruby on Rails)や`Java`(spring / struts2)を中心としたバックエンド開発､ `JavaScript`(jQuery) / `TypeScript`(React / Next.js)を中心としたフロントエンド開発に従事｡また､クライアント折衝や､オフショア先とコミュニケーションなど､PM / PdM の役割も担う

| 期間            | プロジェクト概要                                                                     | やったこと / 実績                                                                                              | 言語･その他                                                                           |
| --------------- | ------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| 2021/06〜08     | 機能開発(SES) AI 株価予測 web アプリケーション内に株式売買 / 投資信託の検索          | - 基本設計 / 詳細設計                                                                                          | 【BE】Ruby（Ruby on Rails）<br>【FE】React                                            |
| 2021/02〜05     | web アプリケーション開発(SES) 某生命保険会社保険比較サイト                           | - api 詳細設計 / 開発<br>- UI / UX 設計 / 開発                                                                 | 【BE】Ruby（Ruby on Rails）<br>【FE】Next.js（React.js / TypeScript）<br>【infra】AWS |
| 2020/09~2021/01 | エンハンス開発(受託) 某アミューズメント会社ポイント管理 web アプリケーション保守運用 | - ios アプリ Webview リプレイス<br>- ios / android アプリ リリース<br>- クライアント折衝                       | 【BE】Java / Android-Java<br>【FE】JavaScript（jQuery）<br>【infra】AWS               |
| 2020/05~08      | 機能開発(受託) 某アミューズメント会社ポイント管理 web アプリケーション               | - ポイント機能 / 帳票出力機能の開発<br>- クライアント折衝<br>- オフショア先とのコミュニケーション<br>- DB 設計 | 【BE】Java / Android-Java<br>【FE】JavaScript（jQuery）<br>【infra】AWS<br>           |
| 2020/02~04      | 某歯科向け web アプリケーション開発(SES)                                             | - 1200 万件データ移行ツール開発<br>- SQL パフォーマンスチューニング<br>- フロントエンド / バックエンド改修     | 【BE】Java（spring）<br>【FE】javascript（jQuery、Angular）<br>【infra】oracle cloud  |
| 2020/01         | 某設計建築会社の基幹システム開発(受託)                                               | -                                                                                                              |                                                                                       |

### [株式会社パルホールディングス](https://www.palgroup.holdings/#topOL) (2015/04~2019/09)

店長として店舗運営全般と人材育成などのマネジメント業務をする傍ら､[TECH CAMP(旧 TECH EXPERT)](https://tech-camp.in/expert)にてプログラミング学習を行う

- **プロジェクト規模：**
  - 個人開発
  - 4 人チームでアジャイル開発
- **役割：**
  - コーディング､レビュー､チームビルディング
- **プロジェクト詳細：**
  - Ruby/Ruby on Rails､jQuery､AWS を使い､チャットアプリケーションやフリマアプリをフルスクラッチで開発

### [バンタンデザイン研究所 東京校 ファッションビジネス学科](https://www.vantan.com/) (2014/04~2015/03)

- 学んだこと
  - 店舗の立地選定から店舗デザイン、プロモーションの打ち出し方、損益分岐点を設定して利益を出す為の店舗運営の仕方を学ぶ
  - 卒業制作にてオリジナル商品を作成

### [株式会社しまむら](https://www.shimamura.gr.jp/company/profile/) (2011/04~2014/03)

- 事業内容：
  - 婦人服・紳士服・雑貨等の企画・製造及び卸・小売
- 業務内容：
  - 店長として店舗運営全般と人材育成などのマネジメント
