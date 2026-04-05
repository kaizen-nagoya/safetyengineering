---
title: プログラマが安全工学シンポジウムで発表する動機、題材、技法。安全（22）OSEK(70), Ethernet(70)
tags: 安全 プログラマ C OSEK ethernet
author: kaizen_nagoya
slide: false
---
# はじめに
日本学術会議が開催している行事に、安全工学シンポジウムがあります。
https://www.anzen.org

共催学会は、
安全工学会
化学工学会	
火薬学会	
計測自動制御学会
自動車技術会	
静電気学会	
地域安全学会
低温工学・超電導学会
電気学会	
電気化学会	
電気設備学会	
電子情報通信学会
土木学会	
日本化学会	
日本火災学会	
日本機械学会
日本技術士会
日本計算工学会
日本原子力学会
日本建築学会（幹事学会）
日本高圧力技術協会
日本航空宇宙学会
日本材料学会	
日本信頼性学会
日本心理学会
日本船舶海洋工学会	
日本鉄鋼協会
日本人間工学会
日本燃焼学会
日本非破壊検査協会	
日本溶接協会
日本リスク学会
日本冷凍空調学会
廃棄物資源循環学会			

学会という名称でない団体の共催しています。

協賛（予定）は、
応用物理学会		
日本地震工学会		
日本経営工学会	
日本知能情報ファジィ学会		
日本デザイン学会		
日本プラントメンテナンス協会	
粉体粉末冶金協会		
日本保全学会		
日本ロボット学会	

です。プログラマに関連する学会で、共催・協賛は、
計測自動制御学会 https://www.sice.jp
自動車技術会 https://www.jsae.or.jp	
電子情報通信学会 https://www.ieice.org/jpn_r/
日本信頼性学会 https://www.reaj.jp
日本心理学会 https://psych.or.jp	
日本リスク学会 http://www.sra-japan.jp/cms/
日本人間工学会 https://www.ergonomics.jp
日本技術士会　https://www.engineer.or.jp
日本計算工学会　https://www.jsces.org

共催、協賛していない学会は、
情報処理学会 https://www.ipsj.or.jp
日本ソフトウェア科学会 https://www.jssst.or.jp
などです。

その他、著名な学会で参加していないのは、
医学係の学会と、数学・物理関係の学会と、社会科学系・人文科学系の学会です。

# 背景
2004年から、AUTOSARのopen souceの取り組みの中で、
アイシン精機さんの豊頃試験場で、試験運転実験に参加させていただき、安全工学シンポジウムでの発表題材を明確化できた。

ご指導いただいた、安全工学の専門家の方から
安全工学シンポジウムで発表するように勧められた。

以降、十数年ちょっと、合計１１回参加してきた。

今年の発表予定題材を整理する。

一人１主題を原則としており、共同研究者がほかに数人集まることを想定して３つの主題を準備してきた。

### 20210213 追記

テレビ会議や、その後のLine, Facebookでの議論に基づき、現在準備している３つの題材のうち、一つは、、SWESTまたは来年の安全工学シンポジウムまでにまとまった資料作成に専念することにした。

他の二つのうち、一つは、個人投稿とし、もう一つの連名を募集して、受諾されれば投稿することにした。


# OSEK/Ethernet関連
電気自動車と自動運転を中心に、AUTOSARでまだ十分に仕様になっていない部分を洗い出し、安全に貢献するために何ができるかを整理している。

プログラマが電池設計に寄与できるプログラムを書くために
https://qiita.com/kaizen_nagoya/items/73e44e4f1ebf161f58cc

TOPPERS のAUTOSARへの貢献(更新中)
https://qiita.com/kaizen_nagoya/items/d363cf06e2176207b391

あなたの模型(Model)は離散(digital)ですか連続(analog)ですか
https://qiita.com/kaizen_nagoya/items/009b344ee145d7969d61

「風をあつめて」を計画書として事業展開してみる
https://qiita.com/kaizen_nagoya/items/92365c542714f27e5658

人間が計算機に勝てる３つのこと
https://qiita.com/kaizen_nagoya/items/49dc709d289d22846044

# MISRA C/C++ 関連
C言語規格およびC++言語規格が出るたびに、
例題を試験できる形にして、compile and go してきた。

最近はdockerを中心にgcc, clang, visual cの３種類を用いている。

MISRA C/C++, CERT C/C++も同様である。
また、AUTOSAR C++もQiitaに上げてきた。

Autosar Guidelines C++14 example code compile list(1-169)
https://qiita.com/kaizen_nagoya/items/8ccbf6675c3494d57a76

C++N4606, 2016符号断片編纂一覧(example code compile list)
Working Draft 2016, ISO/IEC 14882(1)
https://qiita.com/kaizen_nagoya/items/df5d62c35bd6ed1c3d43/


C++N4868,2018(1)3.21 expression-equivalent [defns.expression-equivalent] p5
https://qiita.com/kaizen_nagoya/items/a4487cda12d9f97c275e

OSはC++で書き直したい。その際に、C言語の#define分のマクロをC++ Templateに書き直す際に解決できていない課題がある。

C言語の#define文マクロをC++のTemplateか何かにする方法
https://qiita.com/kaizen_nagoya/items/20c3f5964cef1da037cb

[C][C++]の国際規格案の例題をコンパイルするときの課題７つ。
https://qiita.com/kaizen_nagoya/items/5f4b155030259497c4de

# HAZOP 関連
## 自動運転
自動運転の安全分析
https://qiita.com/kaizen_nagoya/items/b7f4a714f6016d3c1bf3

## AUTOSAR/OSEK
角速度制御によるエンジン制御、電動機制御において、
CAN通信が邪魔をしないだけでなく、
CAN通信を円滑に行うようにOSEK OSがあることを、
HAZOP分析することにより示す。

## Ethernet
CANに比べて、ノイズ対応、電力消費、遅延がどうかの横顔（Profile)を作成するとよい。

## MISRA
MISRA C/C++の規則をFMEA的な視点で分類するとともに、
HAZOPでも分類するとわかりやすくなる。

## QC検定
安全分析手法であるHAZOPを、QC検定の題材に適用し、
QC検定の内容がHAZOPを導入すれば豊富になることを提案しようとしている。

プログラマがQC検定受けることの意味・価値・課題
https://qiita.com/kaizen_nagoya/items/b03216eb6ab09eacc957

# まとめ
社名入り、社名なし
連名者あり、単独（単独の場合は１件のみ）
連名者社名あり、連名者社名なし
のいずれをも想定。

場合によっては、英語にして自動車技術会に投稿するかもしれない。（その場合の連名の可否は別途相談）

|題材|自社名あり|自社名なし|連名者なし|連名者あり|
|--:|--:|--:|--:|--:|
|AUTOSAR/OSEK|10|10|30|30|
|MISRA |10|10|20|20|
|HAZOP|10|10|20|20|

資料の内容が充実していくと、上記確率が上昇する予定。
連名者なしの場合は、合計が100%越えることはない。
それ以外は、対応して隣接する２つの合計が100%を越えることはない。

自分が参加した過去の目次を掲載しました。

#### 第37回　安全工学シンポジウム (2008)
標題一覧
https://researchmap.jp/multidatabases/multidatabase_contents/detail/231120/778165f035bc3bf3a87546d449d1fa6c?frame_id=576083

#### 第38回　安全工学シンポジウム(2009)
標題一覧
https://researchmap.jp/multidatabases/multidatabase_contents/detail/231120/093356c653ddda117afe695897a2cb23?frame_id=576083

https://researchmap.jp/multidatabases/multidatabase_contents/detail/231120/671def8a04af8b39b5cd96ec68acf503?frame_id=576083

#### 第39回　安全工学シンポジウム(2010)
標題一覧
https://researchmap.jp/multidatabases/multidatabase_contents/detail/231120/6eec73f0e2612a815dc7e8bc4d8a3602?frame_id=576083

#### 第40回　安全工学シンポジウム(2011)
標題一覧
https://researchmap.jp/multidatabases/multidatabase_contents/detail/231120/0aa49a5883ed84f300d6657f4b30ef8f?frame_id=576083

#### 第42回　安全工学シンポジウム(2013)
HAZOPと関連手法の展開
https://www.slideshare.net/kaizenjapan/hazop-anzen21013

#### 第44回　安全工学シンポジウム(2015)
 安全(safety)と安心(security)に関す るC言語コーディング標準の取組     安全工学シンポジウム2015 小川清（技術士（情報工学）・工学博士・   　 名古屋市工業研究所）
https://www.slideshare.net/kaizenjapan/study-on-safety-and-security-ccoding-standards

 安全分析において、HAZOP, FMEA, FTAの組み合わせによる リスクアセスメントの進め方の検討 HAZOP, FMEA and FTA for Risk Assessment 日本学術会議安全工学シンポジウム Tokyo, July 2, 2015 ○ 小川明秀（大同大学） 小川 清 （技術士（情報工学）・工学博士・ 名古屋市工業研究所）
https://www.slideshare.net/kaizenjapan/hazopogawa2015

#### 第45回　安全工学シンポジウム(2016)
安全工学シンポジウム（安全と安心）2016
https://researchmap.jp/blogs/blog_entries/view/82322/26d6134a86a9ea86df64be42487d821d?frame_id=445675

安全分析における HAZOP-TRIZ連携の試み
https://www.slideshare.net/kaizenjapan/hazop-and-triz-byoffor-the-children13
#### 第46回　安全工学シンポジウム(2017)
HAZOP-­‐TRIZ連携による   交通安全分析  
https://www.slideshare.net/kaizenjapan/road-traffic-safety-analysis-with-hazop-and-triz

#### 第48回　安全工学シンポジウム(2019)
https://researchmap.jp/blogs/blog_entries/view/109203/b3e2ade8d2fcb4089c66f602f316b40a?frame_id=416975&lang=en

1-4機械の制御システムの設計における安全分析の事例報告尾崎秀典，青島武志，可兒利弘，路　海寧（オプトン），○間瀬　剛，松原和音，斉藤直希，小川　清（名古屋市工業研究所）
1-5HAZOPとTRIZを適用した新製品開発とその安全分析○斉藤直希，間瀬　剛，松原和音，小川　清（名古屋市工業研究所），寺久保　敏，石津和紀，坪井俊之（システム技術研究会）
1-6医療システムへのHAZOP適用○松原和音，間瀬　剛，斉藤直希，小川　清（名古屋市工業研究所）
4-1災害支援無線系における安全分析手法の応用○小川　清，斉藤直希，間瀬　剛，松原和音（名古屋市工業研究所），村上　孝，小寺浩司（デンソークリエイト），福田仁志（豊田自動織機）
5-3安全分析の図的表現方法、及び設計文書と親和性の高いツールの提案○田中伸明（ガイオ・テクノロジー），小川　清（名古屋市工業研究所）

鍵：anzen
未来（未来短歌会）月と鏡集　佐伯裕子　選　p.65 安全工学シンポジウム 　 小川清
https://researchmap.jp/blogs/blog_entries/view/78881/2af9d72857252c9112e4d98dbcca7d59?frame_id=412479

>零細な工場を安全にするため機械分析設計極める
非常時の無線連絡見直して職務で亡くなる人がなきよう
Wi-Fi（ワイファイ）の相互接続容易化にSSID(エスエスアイディ)00000JAPAN（ファイブゼロジャパン）
医療系システムオープンソースでと言ったら医師から声がかかった
各アプリ相互接続できるよう災害想定して実験す
Twitter, facebookとLineからinstagram, mastodonまで
災害が起きたらすぐに知らせるよIT技術その日のために

## 2021安全工学シンポジウム
安全工学シンポジウムの発表を２週間で作る方法
https://qiita.com/kaizen_nagoya/items/13e2d3d2421694bf950d
安全工学シンポジウムへの投稿を１週間で作成する方法
https://qiita.com/kaizen_nagoya/items/181f2ced6d418de9c7a6

オープンソース計算機模擬試験による安全関連系の設計と分析
https://qiita.com/kaizen_nagoya/items/a317bf6570cb3bdf185b

# 参考資料(Reference)
WSL上にnxtOSEKの開発環境を構築する方法
https://qiita.com/TsuneoNakanishi/items/76999b2e6b4e9cd30117

Raspberry Pi 3 Model B+ 向けにリアルタイムOSを実装してみた話
https://qiita.com/tenkoh2/items/baa8e0b6c09669793b4f

[メモ] TrampolineRTOSでLチカ (OSEK/VDX & AUTOSAR APIにあわせたRTOS)
https://qiita.com/mt08/items/65f2ac9bbdae09a34470

MacでLego Mindstorms NXT環境構築 in 2018
https://qiita.com/vivid344/items/2f23f846cd3b135c5a74

ETロボコン開発環境構築 for Mac
https://qiita.com/tac0x2a/items/b1d82050c660935765ef

[メモ] ERIKA様でLチカ (Arduino)
https://qiita.com/mt08/items/adc90efbbfc938be7cc4

COFEを使って水-エタノールの分離シミュレーションを行う
https://qiita.com/kijuky/items/0979327cf7e7c091da02

# 自己参考(Self Reference)
物理記事　上位100
https://qiita.com/kaizen_nagoya/items/66e90fe31fbe3facc6ff

数学関連記事１００
https://qiita.com/kaizen_nagoya/items/d8dadb49a6397e854c6d

言語・文学記事　１００
https://qiita.com/kaizen_nagoya/items/42d58d5ef7fb53c407d6

医工連携関連記事一覧
https://qiita.com/kaizen_nagoya/items/6ab51c12ba51bc260a82

自動車　記事　１００
https://qiita.com/kaizen_nagoya/items/f7f0b9ab36569ad409c5

日本語（０）一欄
https://qiita.com/kaizen_nagoya/items/7498dcfa3a9ba7fd1e68

一覧の一覧( The directory of directories of mine.) Qiita(100)
https://qiita.com/kaizen_nagoya/items/7eb0e006543886138f39

仮説（0）一覧（目標100現在40）
https://qiita.com/kaizen_nagoya/items/f000506fe1837b3590df

安全（0）安全工学シンポジウムに向けて: 21
https://qiita.com/kaizen_nagoya/items/c5d78f3def8195cb2409

通信記事１００
https://qiita.com/kaizen_nagoya/items/1d67de5e1cd207b05ef7

Ethernet 記事一覧　Ethernet(0)
https://qiita.com/kaizen_nagoya/items/88d35e99f74aefc98794

Wireshark 一覧 wireshark(0)、Ethernet(48) 
https://qiita.com/kaizen_nagoya/items/fbed841f61875c4731d0

線網（Wi-Fi）空中線(antenna)(0) 記事一覧(118/300目標)
https://qiita.com/kaizen_nagoya/items/5e5464ac2b24bd4cd001

OSEK OS設計の基礎　OSEK(100)
https://qiita.com/kaizen_nagoya/items/7528a22a14242d2d58a3

Error一覧
https://qiita.com/kaizen_nagoya/items/48b6cbc8d68eae2c42b8

OSEKはもう流行らないのでしょうか。AUTOSAR（64）OSEK(1) https://qiita.com/kaizen_nagoya/items/b87687254b11f30cc2ee
OSEKを図から理解 OSEK(2) https://qiita.com/kaizen_nagoya/items/f87a7ff5aeb63803a022
OSEK OS（AUTOSAR OS）をざっくり理解するには OSEK(3) https://qiita.com/kaizen_nagoya/items/c68c0b86b97d4a90e6e2
calloutとcallback, OSEK/VDX OS and AUTOSAR OSEK(4) https://qiita.com/kaizen_nagoya/items/b95b81354d07b9172a56
OSEK/VDX ISO and 2.23 OSEK(5) https://qiita.com/kaizen_nagoya/items/4d6bcec01e0132f9c41c
OSEK/VDX OSEK(6) https://qiita.com/kaizen_nagoya/items/a7720994f2178a15be81
ISO OSEK/VDX and ISO Linux OS 同梱ソースをC++またはRUSTで書く企画　OSEK(7) https://qiita.com/kaizen_nagoya/items/27899e936c90b415d700
OSEK 記事で views 100,000を目指して　OSEK(8) https://qiita.com/kaizen_nagoya/items/ff45ee55566eeff5f62e
自動車用OSを網羅する OSEK(9) https://qiita.com/kaizen_nagoya/items/a61144daf500a3f2b4f4
Smallest Set Profile and Automotive Profile, OSEK(10) https://qiita.com/kaizen_nagoya/items/0c5484f6562cc259e7f0
Exclusive Area, OSEK(11)　https://qiita.com/kaizen_nagoya/items/d87ff4e08378dbcf68a7
自動車のソフトウェア、例えばAUTOSAR の仕事を始めてする方に, OSEK(12) https://qiita.com/kaizen_nagoya/items/1832634788c23498e054
名古屋で自動車関係のソフトウェア設計する際にあるといいかもしれない知識, OSEK(13) https://qiita.com/kaizen_nagoya/items/9f01d55e4bd0bd931c96
single task os and data, OSEK(14) https://qiita.com/kaizen_nagoya/items/6acbd5d2cfd3ed8bca60
AUTOSARといえば O で始まる用語は? OSEK(15) https://qiita.com/kaizen_nagoya/items/06c969fe5c4b3e7319e0
Automotive Software Expert Examination Exercise, Examples or Extract. OSEK(16) https://qiita.com/kaizen_nagoya/items/1762e0612ef01e036efb
自動運転資料集(1) OSEK(17) https://qiita.com/kaizen_nagoya/items/42eb2129e281f25eaab8
TOPPERS of the YearとAUTOSAR, AUTOSAR(39), OSEK(18) https://qiita.com/kaizen_nagoya/items/f241bb4a819733110b7a
Autosar 2.0を読む, AUTOSAR(25), OSEK(19) https://qiita.com/kaizen_nagoya/items/b44a1047c2c517d522fe
IT関連技術でお世話になった方々, OSEK(20) https://qiita.com/kaizen_nagoya/items/8a5bf487594cd106e8b8
AUTOSARの４つの入力, OSEK(21)  https://qiita.com/kaizen_nagoya/items/72cef6028b9697f7968e
AUTOSAR これだけ知っていればなんとかなる。OSEK(22) https://qiita.com/kaizen_nagoya/items/7a63e706bfb8f331cfe4
AUTOSAR based on ISO, OSEK(23) https://qiita.com/kaizen_nagoya/items/867a709cdf6f4dbdecc6
AUTOSARと国際規格。AUTOSAR（65), OSEK(24)  https://qiita.com/kaizen_nagoya/items/4ddba03efb942969b125
AUTOSAR入門, AUTOSAR(16), OSEK(25) https://qiita.com/kaizen_nagoya/items/5e43b8ef0935c32ee11d
AUTOSAR 記事1000までの道, OSEK(26) https://qiita.com/kaizen_nagoya/items/785473512f5f7f85a6bf
Autosarの課題, OSEK(27)  https://qiita.com/kaizen_nagoya/items/617d10b0e34143030600
AUTOSAR: The past 20 years and he next 10 years, OSEK(28) https://qiita.com/kaizen_nagoya/items/2dab0707c01059c152c4
Autosar文書を読む（準備), OSEK(29)　https://qiita.com/kaizen_nagoya/items/5f547173544703d267aa
AUTOSARが手に取るように分かるようになる。AUTOSAR(29), OSEK(30) https://qiita.com/kaizen_nagoya/items/ae092ea6aef89cdc15df
posixとethernet, osekとTCP/IP, osek(31) https://qiita.com/kaizen_nagoya/items/73b79a4a56f433bd53c0
斉藤直希「組み込み向けリアルタイムOSの基礎知識を整理する」を整理する, OSEK(32) https://qiita.com/kaizen_nagoya/items/d305e83b37d0c57dceb3
TOPPERS活用アイデア・アプリケーション開発コンテスト受賞作品紹介　まとめ作成中, OSEK(33) https://qiita.com/kaizen_nagoya/items/72b882d96b2841f25faf
はじめてのAUTOSAR(classic platform) ＜エンジニア夏休み企画>【読書感想文】, OSEK(34) https://qiita.com/kaizen_nagoya/items/696ad320f76f284664d7
AUTOSARとSimulink: Adaptive Platform, Classic Platformとマルチコア・共通化, OSEK(35) https://qiita.com/kaizen_nagoya/items/d613b0b14bfd91989a13
AUTOSAR Abstract Platformへの道（詳細編）, OSEK(36) https://qiita.com/kaizen_nagoya/items/cb217133884fa0a2c704
building block：AUTOSAR Abstruct Platform , OSEK(37), https://qiita.com/kaizen_nagoya/items/bf7c17624f648fb9f392
系建築家(system architect)になるには, OSEK(38) https://qiita.com/kaizen_nagoya/items/8c341e69233cb32f6275
自己紹介 OSEK(39) https://qiita.com/kaizen_nagoya/items/90aa368f296613ec93b5
AUTOSAR 「完全に理解した」, OSEK(40) https://qiita.com/kaizen_nagoya/items/51983798ad7902b33cb1
Architecture 「toaster model」を出発点として, OSEK(41)　https://qiita.com/kaizen_nagoya/items/9ab8b4bea3ff4e94b192
AUTOSAR Q&A。 AUTOSAR(30), OSEK(42) https://qiita.com/kaizen_nagoya/items/ba6c02b772e9617dc138
「人生で影響を受けた本100冊」に28冊足す計画（18冊）, OSEK(43) https://qiita.com/kaizen_nagoya/items/3ae6633725df77261df8
Bosch Automotive Handbook and so on. OSEK(44) https://qiita.com/kaizen_nagoya/items/8e330ce57880f04d71d9
動車　記事　１００, OSEK(45) https://qiita.com/kaizen_nagoya/items/f7f0b9ab36569ad409c5
何故、今、国際規格なのか。OSEK(46) https://qiita.com/kaizen_nagoya/items/6970577e3e94e5b51ccc
名古屋のIoTは名古屋のOSで。仮説（186）OSEK(47) https://qiita.com/kaizen_nagoya/items/fa6694bbec50723ea90a
AUTOSAR一覧作っていて気が付いたこと順位(ranking) osek(48) https://qiita.com/kaizen_nagoya/items/2c800548690dd9fb9f53
AUTOSAR教材作成３年計画, AUTOSAR(19) OSEK(49) https://qiita.com/kaizen_nagoya/items/84d8f1ecbbe7af7803af
AUTOSARの利点と方向性, OSEK(50) https://qiita.com/kaizen_nagoya/items/681902476520cccf3c3e
TOPPERS のAUTOSARへの貢献(更新中), AUTOSAR(15), OSEK(51) https://qiita.com/kaizen_nagoya/items/d363cf06e2176207b391
TOPPERS の AUTOSAR への貢献 II (改定中), OSEK(52) https://qiita.com/kaizen_nagoya/items/4614c04cfff70a241f77
A big wrapping cloth with the miniature garden, OSEK53) https://qiita.com/kaizen_nagoya/items/96411f20632e7f3ff73a
AUTOSAR R23-11 資料整理の計画（年越し懇親会遠隔開催時間投票含む）OSEK(54)　https://qiita.com/kaizen_nagoya/items/6b939e2373e0e6047ae8
自動車用（車載）ソフトウェアの基本設計提案を作る。OSEK(55)  https://qiita.com/kaizen_nagoya/items/9c218e65d98084b24dfe
自動車用（車載）ソフトウェアの基本設計提案を作る(2), OSEK(56) https://qiita.com/kaizen_nagoya/items/38cb4710410a0d51e7a0
マルチコアの壁, OSEK(57) https://qiita.com/kaizen_nagoya/items/f38e47574905c80c0706
実時間処理, OESK(58) https://qiita.com/kaizen_nagoya/items/1e36077736d11960bb64
CPU マルチコア　マルチOS, OSEK(59) https://qiita.com/kaizen_nagoya/items/6bdb6116f0aa50c5372a
AUTOSAR related Standard, OSEK(60) 
https://qiita.com/kaizen_nagoya/items/13b163f8515615ecc648
「あなたがAUTOSARのEditorだったらどの文書をどう書き換えたいか」選手権(0), OSEK(61) 
https://qiita.com/kaizen_nagoya/items/0055bb88f43f98a61739
Call back, OSEK(62) 
https://qiita.com/kaizen_nagoya/items/8c76f5e05cbd9125f86d
C言語教育はCコンパイラの写経で, OSEK(63) 
https://qiita.com/kaizen_nagoya/items/088a9906797559cd8b8a
Reentrant とRecursive, OESK(64)　
https://qiita.com/kaizen_nagoya/items/cdc028f73fe2dea3090f
AUTOSARの基礎の仮説, OSEK(65) 
https://qiita.com/kaizen_nagoya/items/ceaf360e69f81c332677
Linuxを学ばずに使う, OSK(66)　
https://qiita.com/kaizen_nagoya/items/b9859782bab0cf6c78a4
AUTOSAR わかりにくいこと12, AUTOSAR(27), OSEK(67) 
https://qiita.com/kaizen_nagoya/items/68b0da5bee1421200a11
お盆には「箱庭」記事を書きましょう「もくもく会」の題材になる（１）, OSEK(68) 
https://qiita.com/kaizen_nagoya/items/a22bf2b1dab0ad3258d4
逆も真：社会人が最初に確かめるとよいこと。OSEK(69) 
https://qiita.com/kaizen_nagoya/items/39afe4a728a31b903ddc
プログラマが安全工学シンポジウムで発表する動機、題材、技法。安全（22）OSEK(70) 
https://qiita.com/kaizen_nagoya/items/b7adf3001eb325166e52
プログラマにも読んでほしい「QC検定にも役立つ！QCべからず集」OSEK(71)　
https://qiita.com/kaizen_nagoya/items/d8ada7b7fceafe2e5f0e
AUTOSAR文書の読み方（文書番号と発行年）, AUTOSAR(23), OSEK(72) 
https://qiita.com/kaizen_nagoya/items/daa3f7de7e86b89bcc33
計算機系事故記録(computer system trouble record), OSEK(73) 
https://qiita.com/kaizen_nagoya/items/910847f01379903e40c8
basic: プログラムジェネレータジェネレータ。構造屋(architect)としての成功事例3失敗事例６, OESK(74) 
https://qiita.com/kaizen_nagoya/items/117c7a1b6dad97470ae9
AUTOSAR記事一覧, OSEK(75) 
https://qiita.com/kaizen_nagoya/items/89c07961b59a8754c869
AUTOSAR 文書番号, OSEK(76) 
https://qiita.com/kaizen_nagoya/items/8b894228a0b76c2265c7
参考文献の参考文献は参考文献だ。清水吉男「「派生開発」を成功させるプロセス改善の技術と極意」を超えて, OSEK(77) 
https://qiita.com/kaizen_nagoya/items/562a0cf784cf92bc0ebb
ボッシュ自動車handbook(英語)11版(0-1) 課題と記事一覧new, OSEK(78) 
https://qiita.com/kaizen_nagoya/items/a9d2887bf2a7598dc8e5
プログラマの「プログラムが書ける」思い込みは強みだ。３つの理由。仮説（168）統計と確率(17) , OSEK(79) 
https://qiita.com/kaizen_nagoya/items/bc5dd86e414de402ec29
最新規格のコンパイル, OSEK(80) 
https://qiita.com/kaizen_nagoya/items/4e23544a7ee8a8f19b68

＜この記事は個人の過去の経験に基づく個人の感想です。現在所属する組織、業務とは関係がありません。＞
This article is an individual impression based on the individual's experience. It has nothing to do with the organization or business to which I currently belong.
### 文書履歴(document history)
ver. 0.01 初稿 20210205
ver. 0.02 追記 20210206
ver. 0.03 学会追記 20210207
ver. 0.04 日本技術士会　日本計算工学会 追記 20210208
ver. 0.05 ２つ投稿に絞る 20210213
ver. 0.06 2021安全工学シンポジウム 20210704
### 最後までおよみいただきありがとうございました。
いいね　💚、フォローをお願いします。
#### Thank you very much for reading to the last sentence.
Please press the like icon 💚　and follow me for your happy life.
