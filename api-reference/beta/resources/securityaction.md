---
title: securityAction リソースの種類
description: Microsoft Graph のセキュリティの securityAction エンティティを使用して、脅威から保護するためのアクションをただちに実行します。 セキュリティ アナリストが、悪意のあるファイル、URL、ドメイン、IP アドレスなどの新しいインジケーターを発見した場合、Microsoft のセキュリティ ソリューションでそれらに対する保護をすぐに有効にできます。 特定のプロバイダーのアクションを呼び出し、実行されるすべての操作を表示し、必要な場合は操作を取り消します。 Windows Defender ATP (近日公開) でセキュリティ アクションを実行し、アラートに表示されるプロパティまたは調査中に特定されるプロパティを使用して Windows のエンドポイントの悪意のあるアクティビティをブロックします。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 5aa99119f23baa4cd9450d48ee4955d7ce91f60d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583682"
---
# <a name="securityaction-resource-type"></a>securityAction リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph のセキュリティの securityAction エンティティを使用して、脅威から保護するためのアクションをただちに実行します。 セキュリティ アナリストが、悪意のあるファイル、URL、ドメイン、IP アドレスなどの新しいインジケーターを発見した場合、Microsoft のセキュリティ ソリューションでそれらに対する保護をすぐに有効にできます。 特定のプロバイダーのアクションを呼び出し、実行されるすべての操作を表示し、必要な場合は操作を取り消します。 [windows Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection)を使用してセキュリティアクションを試行し、警告で表示されたプロパティを使用して windows エンドポイント上の悪意のあるアクティビティをブロックするか、調査中に特定します。

  > **注:** 現在、セキュリティアクションはアプリケーションのアクセス許可のみサポートしています。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [セキュリティ アクションを取得する](../api/securityaction-get.md) | [securityAction](securityaction.md) | securityAction オブジェクトのプロパティとリレーションシップを読み取ります。 |
| [セキュリティ アクションを作成する](../api/securityactions-post.md) | [securityAction](securityaction.md) | securityactions コレクションへの投稿によって新しい securityAction を作成します。 |
| [セキュリティ アクションを一覧表示する](../api/securityactions-list.md) | [securityAction](securityaction.md)コレクション | securityAction オブジェクトのコレクションを取得します。 |
|[セキュリティ アクションをキャンセルする](../api/securityaction-cancelsecurityaction.md)|なし|セキュリティ操作をキャンセルします。|

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|actionreason|String|このアクションを起動する理由。|
|appId|String|アクションを送信 (POST) した、呼び出し元アプリケーションのアプリケーション ID。 appId は、認証トークンから抽出され、呼び出し元アプリケーションによって手動で入力されることはありません。|
|azureTenantId|String|エンティティが属しているテナントを判断するエンティティの Azure テナント ID (マルチテナントのサポート)。 azureTenantId は、認証トークンから抽出され、呼び出し元アプリケーションによって手動で入力されることはありません。|
|CompletedDateTime|DateTimeOffset|アクションが完了したときのタイムスタンプ。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|createdDateTime|DateTimeOffset|アクションが作成されたときのタイムスタンプ。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|errorInfo|[resultInfo](resultinfo.md)| アクションが失敗した場合のエラー情報。|
|id|String| アクションが取り込まれたの場合に、システムによって作成されます。 生成された GUID/一意の識別子。 読み取り専用。|
|lastactiondatetime|DateTimeOffset| このアクションが最後に更新されたときのタイムスタンプ。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|name|String| アクション名。|
|parameters|[keyValuePair](keyvaluepair.md) コレクション| アクションを呼び出すために必要なパラメーター (キーと値のペア) のコレクション (たとえば、ブロックする URL または filehash など)。 **必須**|
|示し|[securityactionstate](securityactionstate.md)コレクション|アクションの履歴を保持する securityactionstate のコレクション。|
|status|string| アクションの状態。 使用可能な値は、`NotStarted`、`Running`、`Completed`、`Failed` です。|
|user|String| アクションを送信 (POST) した、サインインしているユーザーのユーザープリンシパル名。 ユーザーは、認証トークンから抽出され、呼び出し元アプリケーションによって手動で入力されることはありません。|
|vendorInformation|[securityVendorInformation](securityvendorinformation.md)|セキュリティ製品/サービスベンダー、プロバイダー、およびサブプロバイダに関する詳細を含む複合型 (ベンダー = Microsoft; provider = Windows Defender ATP; サブプロバイダ = AppLocker)。|

## <a name="relationships"></a>関係

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