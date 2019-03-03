---
title: tiindicator の更新
description: tiindicator オブジェクトのプロパティを更新します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 3c7ec883be4d84efa028362438660ade38e23689
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30367086"
---
# <a name="update-tiindicator"></a>tiindicator の更新

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[tiindicator](../resources/tiindicator.md)オブジェクトのプロパティを更新します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
|:---------------------------------------|:--------------------------------------------|
| 委任 (職場または学校のアカウント)     | ThreatIndicators application.readwrite.ownedby |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。 |
| アプリケーション                            | ThreatIndicators application.readwrite.ownedby |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/tiIndicators/{id}
```

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 説明|
|:-----------|:-----------|
| Authorization | ベアラー {コード} が**必要です** |
|Prefer | 戻り値 = 表現 |

## <a name="request-body"></a>要求本文

要求本文で、更新する関連フィールドの値を指定します。 要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。 最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|action|string| インジケーターが targetproduct セキュリティツール内から一致した場合に適用するアクション。 使用可能な値は、`unknown`、`allow`、`block`、`alert` です。|
|activitygroupnames|String コレクション|脅威指標でカバーされる悪意のあるアクティビティを担当する、その当事者のためのサイバー脅威インテリジェンス名。|
|additionalinformation|String|他の tiindicator プロパティでカバーされていない特別なデータが配置される可能性がある catchall 領域。 通常、additionalinformation に配置されるデータは、targetproduct セキュリティツールでは使用されません。|
|confidence|Int32|インジケーター内のデータが悪意のある動作を正確に特定していることを表す整数。 指定できる値は 0 ~ 100 で、100は最高です。|
|説明|String|インジケーターで表される脅威の簡単な説明 (100 文字以内)。|
|diamondModel|string|このインジケーターが存在する菱形モデルの領域。 可能な値は、`unknown`、`adversary`、`capability`、`infrastructure`、`victim` です。|
|expirationDateTime|DateTimeOffset| インジケーターがいつ期限切れになるかを示す DateTime 文字列。 システム内の古いインジケーターが保持されないようにするには、すべてのインジケーターに有効期限が設定されている必要があります。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`2014-01-01T00:00:00Z`|
|externalId|String|インジケーターをインジケータープロバイダーのシステム (例: 外部キー) に結びつける識別番号。|
|isActive|Boolean|システム内のインジケーターを非アクティブ化するために使用されます。 既定では、送信されたインジケーターはすべてアクティブとして設定されます。 ただし、プロバイダーは、この設定を使用した既存のインジケーターを ' False ' に送信して、システム内のインジケーターを非アクティブ化することができます。|
|"出てきたチェイン"|String コレクション|このインジケーターが対象とする、キルチェーン上の点または点を表す文字列の JSON 配列。 正確な値については、以下の「"" を参照」の値」を参照してください。|
|knownfalse 陽性|String|インジケーターが誤検知を引き起こす可能性があるシナリオ。 これは、人間が判読できるテキストである必要があります。|
|lastReportedDateTime|DateTimeOffset|最後にインジケーターが表示された時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`2014-01-01T00:00:00Z`|
|悪意のある refrefamilynames|String コレクション|インジケーターに関連付けられたマルウェアファミリ名 (存在する場合)。 microsoft では、Windows Defender セキュリティインテリジェンスの[脅威の百科事典](https://www.microsoft.com/wdsi/threats)を使用して検出できる場合は、microsoft マルウェアファミリ名を推奨しています。|
|「いいえ veonly」|Boolean|エンドユーザーに表示されるイベントをインジケーターがトリガーするかどうかを決定します。 [true] に設定されている場合、セキュリティツールは、' hit ' が発生したことをエンドユーザーに通知しません。 これは、通常、一致が発生したが、その操作は実行されないことをログに記録するセキュリティ製品によって、監査またはサイレントモードとして扱われます。 既定値は false です。|
|重大度|Int32|インジケーター内のデータによって識別される、悪意のある動作の重要度を表す整数。 指定可能な値は0–5で、5は最も深刻であり、0はまったく重要ではありません。 既定値は3です。|
|tags|String コレクション|任意のタグ/キーワードを格納する文字列の JSON 配列。|
|tlpLevel|string| インジケーターのトラフィックライトプロトコルの値。 可能な値は、`unknown`、`white`、`green`、`amber`、`red` です。|

### <a name="diamondmodel-values"></a>diamondModel の値

このモデルの詳細については、[ダイヤモンドモデル](http://diamondmodel.org)を参照してください。

| 値 | 説明 |
|:-------|:------------|
|攻撃|このマークは、敵対について説明します。|
|capability|マークは敵対機の機能です。|
|構築|このインジケーターは、敵対のインフラストラクチャを示しています。|
|犠牲|インジケーターは、敵対者の被害者を示します。|

### <a name="killchain-values"></a>指定した値の継承

| 値 | 説明 |
|:-------|:------------|
|アクション|"目的に対するアクション" を表します。 攻撃者が侵害されたシステムを活用して、分散型サービス拒否攻撃などの処理を実行している。|
|基準|侵害されたシステムの操作によって制御されるチャネルを表します。|
|配信|悪用コードを (例: USB、電子メール、web サイトなどの) 被害に分配するプロセス。|
|活用|脆弱性を利用するエクスプロイトコード (例: コードの実行)。|
|インストール|脆弱性が悪用された後にマルウェアをインストールする。|
|予備|マークは、今後の攻撃で使用されるアクティビティグループの情報の証拠です。|
|Weaponization|脆弱性を悪用コードに変える (たとえば、マルウェア)。|

### <a name="tlplevel-values"></a>tlpLevel の値

各インジケーターには、送信時にトラフィックライトプロトコル (tlp) 値が必要です。 この値は、特定のインジケーターの感度と共有の範囲を表します。

| 値 | 説明 |
|:-------|:------------|
|白| 共有スコープ: 無制限。 インジケーターは無制限に共有できます。制限はありません。|
|緑| 共有スコープ: コミュニティ。 インジケーターはセキュリティコミュニティと共有できます。|
|黄色い| 共有スコープ: 制限されています。 これは、インジケーターの既定の設定であり、共有を脅威インテリジェンスを実装するサービスとサービスオペレーターだけに限定し、共有を制限します。2) システムの動作がインジケーターと同じであるお客様。|
|赤| 共有スコープ: Personal。 これらのインジケーターは、本人でのみ直接共有されるようになっています。 通常は、指定された制限によって tlp 赤のインジケーターは取り込まれたされません。 tlp 赤のインジケーターが送信され**** た場合は、"いいえ" の`True`プロパティをに設定する必要があります。 |

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。

省略可能な`200 OK`要求ヘッダーが使用されている場合、メソッドは応答コードと、応答本文で更新された[tiindicator](../resources/tiIndicator.md)オブジェクトを返します。

## <a name="examples"></a>例

### <a name="example-1-request-without-prefer-header"></a>例 1: 希望するヘッダーのない要求

### <a name="request"></a>要求

ヘッダーの`Prefer`ない要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "update_tiIndicator"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json

{
  "description": "description-updated",
}
```

### <a name="response"></a>応答

応答の例を次に示します。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a>例 2: 要求ヘッダーを使用した要求

### <a name="request"></a>要求

`Prefer`ヘッダーを含む要求の例を次に示します。

<!-- {
  "blockType": "request",
  "name": "update_tiIndicator"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json
Prefer: return=representation

{
  "additionalInformation": "additionalInformation-after-update",
  "confidence": 42,
  "description": "description-after-update",
}
```

### <a name="response"></a>応答

応答の例を次に示します。

> [!NOTE]
> ここに示す response オブジェクトは読みやすいように短縮される場合があります。 実際の呼び出しではすべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Security/tiIndicators/$entity",
    "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
    "azureTenantId": "XXXXXXXXXXXXXXXXXXXXXXXXX",
    "action": null,
    "additionalInformation": "additionalInformation-after-update",
    "activityGroupNames": [],
    "confidence": 42,
    "description": "description-after-update",
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
