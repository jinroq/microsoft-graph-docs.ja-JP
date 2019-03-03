---
title: securityAction リソースの種類
description: Microsoft Graph Security securityAction エンティティを使用して脅威から防御するために、直ちにアクションを実行します。 セキュリティアナリストが、悪意のあるファイル、URL、ドメイン、または IP アドレスなどの新しい指標を見つけた場合、保護を Microsoft セキュリティソリューションですぐに有効にすることができます。 特定のプロバイダーに対してアクションを起動し、実行されたすべてのアクションを表示し、必要に応じて操作をキャンセルします。 windows Defender ATP (近日中) と共にセキュリティアクションを試行して、警告で表示されたプロパティまたは調査中に識別されたプロパティを使用して、windows エンドポイント上の悪意のあるアクティビティをブロックします。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 405f12c2cf484651f8bcefc791c9dd24dae410bd
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366988"
---
# <a name="securityaction-resource-type"></a>securityAction リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph Security securityAction エンティティを使用して脅威から防御するために、直ちにアクションを実行します。 セキュリティアナリストが、悪意のあるファイル、URL、ドメイン、または IP アドレスなどの新しい指標を見つけた場合、保護を Microsoft セキュリティソリューションですぐに有効にすることができます。 特定のプロバイダーに対してアクションを起動し、実行されたすべてのアクションを表示し、必要に応じて操作をキャンセルします。 [windows Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection) (近日中) と共にセキュリティアクションを試行して、警告で表示されたプロパティまたは調査中に識別されたプロパティを使用して、windows エンドポイント上の悪意のあるアクティビティをブロックします。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [securityAction を取得する](../api/securityaction-get.md) | [securityAction](securityaction.md) | securityAction オブジェクトのプロパティとリレーションシップを読み取ります。 |
| [securityAction を作成する](../api/securityactions-post.md) | [securityAction](securityaction.md) | securityactions コレクションへの投稿によって新しい securityAction を作成します。 |
| [セキュリティアクションを一覧表示する](../api/securityactions-list.md) | [securityAction](securityaction.md)コレクション | securityAction オブジェクトのコレクションを取得します。 |
|[securityAction のキャンセル](../api/securityaction-cancelsecurityaction.md)|なし|セキュリティ操作をキャンセルします。|

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|actionreason|String|このアクションを起動する理由。|
|appId|String|アクションを送信 (POST) した、呼び出し元アプリケーションのアプリケーション ID。 appId は、認証トークンから抽出され、呼び出し元アプリケーションによって手動で入力されることはありません。|
|azureTenantId|String|エンティティが属しているテナントを判断するエンティティの Azure テナント ID (マルチテナントのサポート)。 azureTenantId は、認証トークンから抽出され、呼び出し元アプリケーションによって手動で入力されることはありません。|
|CompletedDateTime|DateTimeOffset|アクションが完了したときのタイムスタンプ。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|createdDateTime|DateTimeOffset|アクションが作成されたときのタイムスタンプ。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|errorInfo|[resultInfo](resultinfo.md)| アクションが失敗した場合のエラー情報。|
|id|String| アクションが取り込まれたの場合に、システムによって作成されます。 生成された GUID/一意の識別子。 読み取り専用です。|
|lastActionDateTime|DateTimeOffset| このアクションが最後に更新されたときのタイムスタンプ。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|name|String| アクション名。|
|parameters|[keyValuePair](keyvaluepair.md) コレクション| アクションを呼び出すために必要なパラメーター (キーと値のペア) のコレクション (たとえば、ブロックする URL または filehash など)。 **Required**|
|示し|[securityactionstate](securityactionstate.md)コレクション|アクションの履歴を保持する securityactionstate のコレクション。|
|status|string| アクションの状態。 使用可能な値は、`NotStarted`、`Running`、`Completed`、`Failed` です。|
|user|String| アクションを送信 (POST) した、サインインしているユーザーのユーザープリンシパル名。 ユーザーは、認証トークンから抽出され、呼び出し元アプリケーションによって手動で入力されることはありません。|
|vendorInformation|[securityVendorInformation](securityvendorinformation.md)|セキュリティ製品/サービスベンダー、プロバイダー、およびサブプロバイダに関する詳細を含む複合型 (ベンダー = Microsoft; provider = Windows Defender ATP; サブプロバイダ = AppLocker)。|

## <a name="relationships"></a>リレーションシップ

なし

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityAction",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "actionReason": "String",
  "appId": "String",
  "azureTenantId": "String",
  "clientContext": "String",
  "completedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "errorInfo": {"@odata.type": "microsoft.graph.resultInfo"},
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "name": "String",
  "parameters": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "states": [{"@odata.type": "microsoft.graph.securityActionState"}],
  "status": "string",
  "user": "String",
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->