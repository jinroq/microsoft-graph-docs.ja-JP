---
title: tiindicator リソースの種類
description: 脅威インテリジェンス (TI) インジケーターは、悪意のあるアクティビティを識別するために使用されるデータを表します。 組織が脅威指標を使用する場合 (独自の情報を生成する、オープンソースフィードから取得する、パートナー組織またはコミュニティとの共有、またはデータのフィードを購入するなど)、多くの場合、これらの指標をさまざまなセキュリティで使用することが望まれます。ログデータと照合するためのツール。 Graph Security tiindicators エンティティを使用すると、許可、ブロック、または警告のアクションについて、脅威インジケーターを Microsoft セキュリティツールにアップロードできます。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: f85883394f7218a08f923b29304d2ad22432bb86
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342028"
---
# <a name="tiindicator-resource-type"></a>tiindicator リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

脅威インテリジェンス (TI) インジケーターは、悪意のあるアクティビティを識別するために使用されるデータを表します。 組織が脅威指標を使用する場合 (独自のものを生成する、オープンソースフィードから情報を取得する、パートナー組織またはコミュニティと共有する、データのフィードを購入するなど)、さまざまなセキュリティでこれらの指標を使用することをお勧めします。ログデータと照合するためのツール。 microsoft Graph セキュリティ API の**tiindicators**エンティティを使用すると、許可、ブロック、または警告のアクションについて、脅威インジケーターを microsoft セキュリティツールにアップロードすることができます。

tiindicators によっ**** てアップロードされた脅威指標は、組織に合わせてカスタマイズされたセキュリティソリューションを提供するために、Microsoft の脅威インテリジェンスと組み合わせて使用されます。 tiindicators エンティティ**** を使用する場合は、 **targetproduct**プロパティを使用してインジケーターを使用する Microsoft セキュリティソリューションを指定し、セキュリティソリューションが必要とするアクション (許可、ブロック、または警告) を指定します。**アクション**プロパティを使用して、インジケーターを適用します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [Get tiIndicator](../api/tiindicator-get.md) | [tiindicator](tiindicator.md) | tiindicator オブジェクトのプロパティとリレーションシップを読み取ります。 |
| [Create tiIndicator](../api/tiindicators-post.md) | [tiindicator](tiindicator.md) | tiindicator コレクションへの投稿によって、新しい tiindicator を作成します。 |
| [List tiIndicators](../api/tiindicators-list.md) | [tiindicator](tiindicator.md)コレクション | tiindicator オブジェクトのコレクションを取得します。 |
| [更新する](../api/tiindicator-update.md) | [tiindicator](tiindicator.md) | tiindicator オブジェクトを更新します。 |
| [削除](../api/tiindicator-delete.md) | なし | tiindicator オブジェクトを削除します。 |
|[deleteTiIndicators](../api/tiindicator-deletetiindicators.md)|なし| 複数の tiindicator オブジェクトを削除します。|
|[deleteTiIndicatorsByExternalId](../api/tiindicator-deletetiindicatorsbyexternalid.md)|なし| `externalId`プロパティによって複数の tiindicator オブジェクトを削除します。|
|[submitTiIndicators](../api/tiindicator-submittiindicators.md)|[tiindicator](tiindicator.md)コレクション|tiindicators コレクションを投稿して、新しい tiindicators を作成します。|
|[updateTiIndicators](../api/tiindicator-updatetiindicators.md)|[tiindicator](tiindicator.md)コレクション| 複数の tiindicator オブジェクトを更新します。|

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|action|string| インジケーターが targetproduct セキュリティツール内から一致した場合に適用するアクション。 使用可能な値は、`unknown`、`allow`、`block`、`alert` です。 **必須です。**|
|activitygroupnames|String collection|脅威指標でカバーされる悪意のあるアクティビティを担当する、その当事者のためのサイバー脅威インテリジェンス名。|
|additionalinformation|String|他の tiindicator プロパティでカバーされていない特別なデータが配置される可能性がある catchall 領域。 通常、additionalinformation に配置されるデータは、targetproduct セキュリティツールでは使用されません。|
|azureTenantId|String| インジケーターが取り込まれたのときに、システムによってスタンプされます。 送信クライアントの Azure Active Directory テナント id。 **必須です。**|
|confidence|Int32|インジケーター内のデータが悪意のある動作を正確に特定していることを表す整数。 指定できる値は 0 ~ 100 で、100は最高です。|
|description|String| インジケーターで表される脅威の簡単な説明 (100 文字以内)。 **必須です。**|
|diamondModel|[diamondModel](#diamondmodel-values)|このインジケーターが存在する菱形モデルの領域。 可能な値は、`unknown`、`adversary`、`capability`、`infrastructure`、`victim` です。|
|expirationDateTime|DateTimeOffset| インジケーターがいつ期限切れになるかを示す DateTime 文字列。 システム内の古いインジケーターが保持されないようにするには、すべてのインジケーターに有効期限が設定されている必要があります。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。 **必須です。**|
|externalId|String| インジケーターをインジケータープロバイダーのシステム (例: 外部キー) に結びつける識別番号。 |
|id|String|インジケーターが取り込まれたの場合に、システムによって作成されます。 生成された GUID/一意の識別子。 読み取り専用です。|
|ingestedDateTime|DateTimeOffset| インジケーターが取り込まれたのときに、システムによってスタンプされます。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|isActive|Boolean| システム内のインジケーターを非アクティブ化するために使用されます。 既定では、送信されたインジケーターはすべてアクティブとして設定されます。 ただし、プロバイダーは、この設定を使用した既存のインジケーターを ' False ' に送信して、システム内のインジケーターを非アクティブ化することができます。|
|"出てきたチェイン"|[](#killchain-values)指定したコレクション|このインジケーターが対象とする、キルチェーン上の点または点を表す文字列の JSON 配列。 正確な値については、以下の「次を参照してください」を参照してください。 |
|knownfalse 陽性|String|インジケーターが誤検知を引き起こす可能性があるシナリオ。 これは、人間が判読できるテキストである必要があります。|
|lastReportedDateTime|DateTimeOffset|最後にインジケーターが表示された時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|悪意のある refrefamilynames|String collection|インジケーターに関連付けられたマルウェアファミリ名 (存在する場合)。 microsoft では、Windows Defender セキュリティインテリジェンスの[脅威の百科事典](https://www.microsoft.com/wdsi/threats)を使用して検出できる場合は、microsoft マルウェアファミリ名を推奨しています。|
|「いいえ veonly」|Boolean |エンドユーザーに表示されるイベントをインジケーターがトリガーするかどうかを決定します。 [true] に設定されている場合、セキュリティツールは、' hit ' が発生したことをエンドユーザーに通知しません。 これは、通常、一致が発生したが、その操作は実行されないことをログに記録するセキュリティ製品によって、監査またはサイレントモードとして扱われます。 既定値は False です。 |
|重大度|Int32| インジケーター内のデータによって識別される、悪意のある動作の重要度を表す整数。 指定可能な値は0–5で、5は最も深刻であり、0はまったく重要ではありません。 既定値は3です。 |
|tags|String コレクション|任意のタグ/キーワードを格納する文字列の JSON 配列。 |
|targetproduct|String|インジケーターを適用する1つのセキュリティ製品を表す文字列型 (string) の値を指定します。 指定できる値は`Azure Sentinel`次のとおりです。 **必須**|
|threatType|[threatType](#threattype-values)| 各インジケーターには、有効なインジケーターの脅威の種類が含まれている必要があります。 使用可能な値は、`Botnet`、`C2`、`CryptoMining`、`Darknet`、`DDoS`、`MaliciousUrl`、`Malware`、`Phishing`、`Proxy`、`PUA`、`WatchList` です。 **必須です。** |
|tlpLevel|[tlpLevel](#tlplevel-values)| インジケーターのトラフィックライトプロトコルの値。 可能な値は、`unknown`、`white`、`green`、`amber`、`red` です。 **必須です。**|

### <a name="indicator-observables---email"></a>インジケーター Observables-電子メール

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|emailencoding|String|電子メールで使用されるテキストエンコードの種類。|
|emaillanguage|String|電子メールの言語。|
|emailrecipient|String|受信者の電子メールアドレス。|
|emailSenderAddress|String|attacker& # 124; 犠牲者の電子メールアドレス。|
|emailsendername|String|attacker& # 124; 犠牲者の表示名。|
|emailsourcedomain|String|電子メールで使用されるドメイン。|
|emailSourceIpAddress|String|電子メールの送信元 IP アドレス。|
|emailSubject|String|電子メールの件名。|
|emailxmailer|String|電子メールで使用される X メーラの値。|

### <a name="indicator-observables---file"></a>インジケーター Observables-ファイル

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|fileCompileDateTime|DateTimeOffset|ファイルがコンパイルされた日時。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|fileCreatedDateTime|DateTimeOffset| ファイルが作成された日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|fileHashType|string| filehashvalue に格納されているハッシュの種類。 可能な値は、`unknown`、`sha1`、`sha256`、`md5`、`authenticodeHash256`、`lsHash`、`ctph` です。|
|filehashvalue|String| ファイルハッシュ値。|
|filemutexname|String| ファイルベースの検出で使用されるミューテックス名。|
|fileName|String|マークがファイルベースの場合は、ファイルの名前。 複数のファイル名をコンマで区切ることができます。 |
|filepacker|String|対象のファイルをビルドするために使用される packer。|
|パス|String|危険を示しているファイルのパス。 Windows または * nix スタイルパスの場合があります。|
|fileSize|Int64|ファイルのサイズ (バイト単位)。|
|fileType|String| ファイルの種類の説明テキスト。 たとえば、「Word 文書」や「バイナリ」などです。|

### <a name="indicator-observables---network"></a>インジケーター Observables-ネットワーク

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|domainName|String|このインジケーターに関連付けられているドメイン名。 topleveldomain の形式にする必要があります (たとえば、baddomain.domain.net)。|
|networkCidrBlock|String| このインジケーターで参照されているネットワークの CIDR ブロック表記表現。 送信元と送信先を識別できない場合にのみ使用します。 |
|networkdestinationasn|Int32|インジケーターで参照されているネットワークの宛先自律システム識別子。|
|networkDestinationCidrBlock|String|このインジケーターに含まれる、宛先ネットワークの CIDR ブロック表記表現。|
|networkDestinationIPv4|String|IPv4 IP アドレスの宛先。|
|networkDestinationIPv6|String|IPv6 IP アドレスの宛先。|
|networkdestinationport|Int32|TCP ポートの宛先。|
|networkIPv4|String| IPv4 IP アドレス。 送信元と送信先を識別できない場合にのみ使用します。 |
|networkIPv6|String| IPv6 IP アドレス。 送信元と送信先を識別できない場合にのみ使用します。 |
|networkport|Int32| TCP ポート。 送信元と送信先を識別できない場合にのみ使用します。 |
|networkprotocol|Int32|IPv4 ヘッダーの protocol フィールドの10進表現。|
|networksourceasn|Int32|インジケーターで参照されているネットワークの送信元の自律システム識別子。|
|networksourc要素 drblock|String|このインジケーターに表示されるソースネットワークの CIDR ブロック表記|
|networkSourceIPv4|String|IPv4 IP アドレスソース。|
|networkSourceIPv6|String|IPv6 IP アドレスソース。|
|networksourceport|Int32|TCP ポートのソース。|
|url|String|Uniform resource Locator。 この URL は、RFC 1738 に準拠している必要があります。|
|userAgent|String|危険を示している可能性がある web 要求のユーザーエージェント文字列。|

### <a name="diamondmodel-values"></a>diamondModel の値

このモデルの詳細については、[ダイヤモンドモデル](http://diamondmodel.org)を参照してください。

| メンバー | 値 | 説明 |
|:-------|:----- |:------------|
| 不明 |  .0    | |
| 攻撃 |  1-d    |このマークは、敵対について説明します。|
| capability |  pbm-2   |インジケーターは敵対機の機能です。|
| 構築 | 1/3 |このインジケーターは、敵対のインフラストラクチャを示しています。|
| 犠牲 | 2/4 |インジケーターは、敵対者の被害者を示します。|
| unknownfuturevalue という | 127 | |

### <a name="killchain-values"></a>指定した値の継承

| メンバー | 説明 |
|:-------|:------------|
|アクション|セキュリティ侵害されたシステムを悪用して、分散型のサービス拒否攻撃などの操作を実行していることを、攻撃者が示しています。|
|基準|侵害されたシステムの操作によって制御されるチャネルを表します。|
|Delivery|悪用コードを (例: USB、電子メール、web サイトなどの) 被害に分配するプロセス。|
|活用|脆弱性を利用するエクスプロイトコード (例: コードの実行)。|
|インストール|脆弱性が悪用された後にマルウェアをインストールする。|
|予備|マークは、今後の攻撃で使用されるアクティビティグループの情報の証拠です。|
|Weaponization|脆弱性を悪用コードに変える (たとえば、マルウェア)。|

### <a name="threattype-values"></a>threatType の値

| メンバー | 説明 |
|:-------|:------------|
|ます| インジケーターは、ます node/member の詳細を示しています。|
|基準|インジケーターは、ますのコマンド & Control ノードの詳細を示しています。|
|cryptomining|このネットワークアドレスまたは URL を含むトラフィックは、CyrptoMining/リソースの乱用を示しています。|
|Darknet|インジケーターは、Darknet ノード/ネットワークのものです。
|DDoS|アクティブまたは今後の DDoS キャンペーンに関連する指標。|
|MaliciousUrl|マルウェアに対して提供されている URL。|
|マルウェア|悪意のあるファイルやファイルを説明するインジケーター。|
|フィッシング|フィッシングキャンペーンに関連するインジケーター。|
|プロキシ|インジケーターは、プロキシサービスのことです。|
|私用|望ましくない可能性があるアプリケーション。|
|WatchList|これは、脅威が正確であるかどうか、または手動での解釈が必要な場合に、インジケーターが配置される一般的なバケットです。 これは通常、システムにデータを送信するパートナーによって使用されることはありません。|

### <a name="tlplevel-values"></a>tlpLevel の値

また、すべてのインジケーターに、送信時にトラフィック信号プロトコルの値が含まれている必要があります。 この値は、特定のインジケーターの感度と共有の範囲を表します。

| メンバー | 説明 |
|:-------|:------------|
|ホワイト| 共有スコープ: 無制限。 インジケーターは無制限に共有できます。制限はありません。|
|緑| 共有スコープ: コミュニティ。 インジケーターはセキュリティコミュニティと共有できます。|
|黄色い| 共有スコープ: 制限されています。 これは、インジケーターの既定の設定であり、システムの動作がインジケーターと一致することを示す、脅威インテリジェンス2を実装するサービスおよびサービスオペレーターに対してのみ、共有を制限します。|
|赤| 共有スコープ: Personal。 これらのインジケーターは、本人でのみ直接共有されるようになっています。 通常は、指定された制限によって tlp 赤のインジケーターは取り込まれたされません。 tlp 赤のインジケーターが送信された場合は、"" "の表示の`True`設定のみ" プロパティをに設定する必要があります。 |

## <a name="relationships"></a>リレーションシップ

なし。

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tiIndicator",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "action": "string",
  "activityGroupNames": ["String"],
  "additionalInformation": "String",
  "azureTenantId": "String",
  "confidence": 1024,
  "description": "String",
  "diamondModel": "string",
  "domainName": "String",
  "emailEncoding": "String",
  "emailLanguage": "String",
  "emailRecipient": "String",
  "emailSenderAddress": "String",
  "emailSenderName": "String",
  "emailSourceDomain": "String",
  "emailSourceIpAddress": "String",
  "emailSubject": "String",
  "emailXMailer": "String",
  "expirationDateTime": "String (timestamp)",
  "externalId": "String",
  "fileCompileDateTime": "String (timestamp)",
  "fileCreatedDateTime": "String (timestamp)",
  "fileHashType": "string",
  "fileHashValue": "String",
  "fileMutexName": "String",
  "fileName": "String",
  "filePacker": "String",
  "filePath": "String",
  "fileSize": 1024,
  "fileType": "String",
  "id": "String (identifier)",
  "ingestedDateTime": "String (timestamp)",
  "isActive": true,
  "killChain": ["String"],
  "knownFalsePositives": "String",
  "lastReportedDateTime": "String (timestamp)",
  "malwareFamilyNames": ["String"],
  "networkCidrBlock": "String",
  "networkDestinationAsn": 1024,
  "networkDestinationCidrBlock": "String",
  "networkDestinationIPv4": "String",
  "networkDestinationIPv6": "String",
  "networkDestinationPort": 1024,
  "networkIPv4": "String",
  "networkIPv6": "String",
  "networkPort": 1024,
  "networkProtocol": 1024,
  "networkSourceAsn": 1024,
  "networkSourceCidrBlock": "String",
  "networkSourceIPv4": "String",
  "networkSourceIPv6": "String",
  "networkSourcePort": 1024,
  "passiveOnly": true,
  "severity": 1024,
  "tags": ["String"],
  "targetProduct": "String",
  "threatType": "String",
  "tlpLevel": "string",
  "url": "String",
  "userAgent": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
