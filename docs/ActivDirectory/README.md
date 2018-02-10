## Active Directoryとは
> Active Directory (アクティブディレクトリ) とはマイクロソフトによって開発されたオンプレミスにおけるディレクトリ・サービス・システムであり、Windows 2000 Serverから導入された、ユーザとコンピュータリソースを管理するコンポーネント群の総称である。なお、クラウドコンピューティングにおけるディレクトリ・サービス・システムであるAzure Active Directoryと区別する場合、オンプレミス Active Directoryと表記することもある。
>> [Wikipediaより](https://ja.wikipedia.org/wiki/Active_Directory)

### ActiveDirectoryの５つのサービス
---
- ActiveDirectoryドメインサービス(AD DS)
	- 最も重要なサービスIDの集約や認証を担当する
- ActiveDirectoryライトディレクトリサービス(AD LDS)
	- LDAP(Lightweight Directory Access Protocol)機能に特化したサービス
- ActiveDirectory証明書サービス(AD FS)
	- 証明書の発行管理をおこなう
- ActiveDirectoryフェデレーションサービス(AD FS)
	- 組織を超えた異なる認証基盤での連携をおこなう
- ActiveDirectoryRightsManagementサービス(AD RMS)
	- デジタルコンテンツの保護をおこなう

### Active Directoryを使用するメリット
---
- 認証/承認によるセキュリティの強化
	- 管理者の認めた正規の利用者のみシステムを利用できる
- シングルサインオンによる業務効率の向上
	- １回の認証で全てのリソースを利用できる
- グループポリシーの利用 ←**ここがActiveDirectoryのキモ**
	- セキュリティの強化に結びつく共通ルールを設定し守らせることができる
- セキュリティ更新プログラムの配布
	- WSUS(Windows Server Update Servies)とグループポリシーを利用することでクライアントコンピューターに対する更新プログラムの一元管理ができる
- 統制関連情報の集中化による内部統制対応の効率化
	- 監査機能を利用してログの記録、検査をおこなう

### ワークグループとドメイン
---
![図](URL"タイトル")

#### ワークグループ
- メリット
	- クライアントPCのみでOK
	- 管理者を置かなくてOK
- デメリット
	- 別PCにログインするためにはそこにアカウントが必要になり管理が大変
	 10人が10台のPCにログインするには100個アカウントが必要

#### ドメイン
- デメリット
	- サーバーが必要になる

### フォレストとドメイン
---
![図](URL"タイトル")

