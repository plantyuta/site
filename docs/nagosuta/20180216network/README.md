### 初心者のためのネットワーク入門
#### インターネット≠ネットワーク
---
- ネットワークとネットワークとの繋がり=インターネット

#### 繋ぐために
---
- 機器　ONU(建物まで光ファイバーで届いた光の信号を電気信号に変換する装置) ルータ?　ハブ？　ロードバランサ？
- それらを繋ぐケーブル LAN UTP? STP? 同軸? 無線LANと有線は同レイヤー
- 目に見えない範囲　ネットワークプロトコル 共通のルール

#### レイヤーの概念
---
- OSI参照モデル　”物でねーとせっかくのプレゼントはありえねぞ”
- レイヤー2 MACアドレス 各機器に割り当てられる
- レイヤー3 IPアドレス RT,GWから割り当てられる　静的？　動的?

#### プロトコル
---
- DNS Domain Name Serves
- ICMP Internet Control Message Protocol
- DHCP Dynamic Host Configuration Protocol

- NAT Network Address Tracerater

#### こぼれ話
---
- IPv4アドレスの枯渇 2進数？(2進数で32桁分)　最大いくつ？(2^32 約43億個)
↑そもそも足りるはずがないのでサブネットマスク、VLSM、CIDR、プライベートIPアドレス、NATなど少ないIPアドレスを有効活用するための対策が施されたいた
- IPv6アドレスで解決　IPv4とは相互性なし 16bit単位でコロン(:)で区切り16進数 　最大いくつ？(2^128 約340澗=3.4\*10^38)
- MACアドレスは枯渇しないの？(48bit6バイト 2^48 約70兆) 上位3bitがOUIと呼ばれ残り3バイトは各ベンダーにおいて製品ごとに重複しないように管理する番号

#### ルーティング
---
- Networkの経路を作る
- 静的経路
- 動的経路 Rynamic Routing

#### TCPとUDP
- TCP 信頼性を優先　
- UDP 即時性を優先　ストリーミング

#### 通信速度問題
---
1Gのデータを10分以内に転送したい、速度を計算
1024\*8/600

#### こぼれ話
---
IPアドレスを取得できなかった時に割り当てられるIPアドレス
[169.hoge.hoge.hoge] 404エラーみたいに共通なの？

#### 書籍やサイト
---
#### 書籍
- 徹底攻略MTAネットワーク問題集　Micorsoft
- １週間でCCNAの基礎が学べる本　cisco
- １週間で LPICの基礎が学べる本 Linux
- マスタリングTCP/IP
- オライリーの”イーサネット” タコ本
- 絶対わかる！コマンド&パケットキャプチャー超入門 WireShark とても良いらしい

#### サイト
- https://www.pasonatech.co.jp/techlab/internet  古いけどGeekなぺーじの人に書いてもらったらしい
- ネットワークエンジニアとして http://www.infraeye.com/
- ITporのネットワークコマンド解説ページ
http://tech.nikkeibp.co.jp/it/article/COLUMN/20060125/227900/
http://tech.nikkeibp.co.jp/it/article/COLUMN/20060224/230618/
