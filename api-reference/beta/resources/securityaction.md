---
title: securityAction リソースの種類
description: Microsoft Graph のセキュリティの securityAction エンティティを使用して、脅威から保護するためのアクションをただちに実行します。 セキュリティ アナリストが、悪意のあるファイル、URL、ドメイン、IP アドレスなどの新しいインジケーターを発見した場合、Microsoft のセキュリティ ソリューションでそれらに対する保護をすぐに有効にできます。 特定のプロバイダーのアクションを呼び出し、実行されるすべての操作を表示し、必要な場合は操作を取り消します。 Windows Defender ATP (近日公開) でセキュリティ アクションを実行し、アラートに表示されるプロパティまたは調査中に特定されるプロパティを使用して Windows のエンドポイントの悪意のあるアクティビティをブロックします。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: d1f8603659d665291576ce804a0bd80c75a853df
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008517"
---
# <a name="securityaction-resource-type"></a>securityAction リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph のセキュリティの securityAction エンティティを使用して、脅威から保護するためのアクションをただちに実行します。 セキュリティ アナリストが、悪意のあるファイル、URL、ドメイン、IP アドレスなどの新しいインジケーターを発見した場合、Microsoft のセキュリティ ソリューションでそれらに対する保護をすぐに有効にできます。 特定のプロバイダーのアクションを呼び出し、実行されるすべての操作を表示し、必要な場合は操作を取り消します。 [Windows Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection) でセキュリティ アクションを実行し、アラートに表示されるプロパティまたは調査中に特定されるプロパティを使用して Windows のエンドポイントの悪意のあるアクティビティをブロックします。

  > **注:** 現在、セキュリティ アクションでサポートされているのは、アプリケーションのアクセス許可のみです。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [セキュリティ アクションを取得する](../api/securityaction-get.md) | [securityAction](securityaction.md) | SecurityAction オブジェクトのプロパティとリレーションシップを読み取ります。 |
| [セキュリティ アクションを作成する](../api/securityactions-post.md) | [securityAction](securityaction.md) | SecurityActions コレクションへの投稿によって新しい securityAction を作成します。 |
| [セキュリティ アクションを一覧表示する](../api/securityactions-list.md) | [securityAction](securityaction.md)コレクション | SecurityAction オブジェクトのコレクションを取得します。 |
|[セキュリティ アクションをキャンセルする](../api/securityaction-cancelsecurityaction.md)|None|セキュリティ操作をキャンセルします。|

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|actionReason|String|このアクションを起動する理由。|
|appId|String|アクションを送信 (POST) した、呼び出し元アプリケーションのアプリケーション ID。 AppId は、認証トークンから抽出され、呼び出し元アプリケーションによって手動で入力されることはありません。|
|azureTenantId|String|エンティティが属しているテナントを判断するエンティティの Azure テナント ID (マルチテナントのサポート)。 AzureTenantId は、認証トークンから抽出され、呼び出し元アプリケーションによって手動で入力されることはありません。|
|CompletedDateTime|DateTimeOffset|アクションが完了したときのタイムスタンプ。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|createdDateTime|DateTimeOffset|アクションが作成されたときのタイムスタンプ。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|errorInfo|[resultInfo](resultinfo.md)| アクションが失敗した場合のエラー情報。|
|id|文字列| アクションが取り込まれたの場合に、システムによって作成されます。 生成された GUID/一意の識別子。 読み取り専用です。|
|lastActionDateTime|DateTimeOffset| このアクションが最後に更新されたときのタイムスタンプ。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|name|String| アクション名。|
|parameters|[keyValuePair](keyvaluepair.md) コレクション| アクションを呼び出すために必要なパラメーター (キーと値のペア) のコレクション (たとえば、ブロックする URL または fileHash など)。 **Required**|
|示し|[Securityactionstate](securityactionstate.md)コレクション|アクションの履歴を保持する securityActionState のコレクション。|
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