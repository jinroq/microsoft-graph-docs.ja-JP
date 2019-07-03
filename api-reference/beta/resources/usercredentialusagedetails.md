---
title: Usercredential使い方の詳細リソースの種類
description: 指定したテナントのセルフサービスによるパスワードのリセットの使用法を表します。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: bb92f3bfc91e8fa418d6a33ad6a77a5fddbf9f10
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527631"
---
# <a name="usercredentialusagedetails-resource-type"></a>Usercredential使い方の詳細リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定したテナントのセルフサービスによるパスワードのリセットの使用法を表します。 詳細には、ユーザー情報、リセットの状態、およびエラーの理由が含まれます。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [Usercredentialの詳細を一覧表示する](../api/reportroot-list-usercredentialusagedetails.md) | Usercredentialの詳細 | Usercredentialの詳細オブジェクトのプロパティとリレーションシップを読み取ります。 |

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
| authMethod | string | ユーザーが使用した認証方法を表します。 可能な値は`email`、 `mobileSMS` `mobileCall`、、 `officePhone`、 `securityQuestion` 、(セルフサービスのパスワードのリセットにのみ使用`appNotification`) `appCode`、、 `alternateMobileCall` 、および (登録でのみサポートされます) です。 |
| eventDateTime | DateTimeOffset | Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` |
| failureReason | String | 対応するリセットまたは登録ワークフローのエラーの理由を示します。 |
| 特徴 | string | 可能な値は`registration` 、 `reset`とです。 |
| id | String | 読み取り専用です。 アクティビティの一意識別子。 読み取り専用です。|
| この | Boolean | ワークフローの成功または失敗を示します。 |
| userDisplayName | String | リセットまたは登録ワークフローを実行するユーザーのユーザー名。 |
| userPrincipalName | String | リセットまたは登録ワークフローを実行するユーザーのユーザープリンシパル名。 |

## <a name="relationships"></a>リレーションシップ

なし。

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userCredentialUsageDetails",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "feature":"string",
  "userPrincipalName":"String",
  "userDisplayName": "String",
  "isSuccess" : true,
  "authMethod": "string",
  "failureReason": "String",
  "eventDateTime" : "DateTimeOffset"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userCredentialUsageDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->