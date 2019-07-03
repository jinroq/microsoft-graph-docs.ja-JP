---
title: credentialUsageSummary リソースの種類
description: 組織内のユーザーのうち、セルフサービスのパスワードのリセット機能を使用しているユーザー数の現在の状態を表します。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 46fc3f90b7a7f286d61a324e7b5f439d467a4978
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527086"
---
# <a name="credentialusagesummary-resource-type"></a>credentialUsageSummary リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

組織内のユーザーのうち、セルフサービスのパスワードのリセット機能を使用しているユーザー数の現在の状態を表します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [getCredentialUsageSummary](../api/reportroot-getcredentialusagesummary.md) | credentialUsageSummary | CredentialUsageSummary オブジェクトのプロパティとリレーションシップを読み取ります。 |

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
| authMethod | string | ユーザーが使用した認証方法を表します。 可能な値は`email`、 `mobileSMS` `mobileCall`、、 `officePhone`、 `securityQuestion` 、(セルフサービスのパスワードのリセットにのみ使用`appNotification`さ`appCode`れます`alternateMobileCall` )、、、および (登録に対してのみサポートされています)。 |
| failureActivityCount | Int64 | 失敗したリセットまたは登録データのカウントを提供します。 |
| 特徴 | string | レポートする機能を定義します。 可能な値は`registration` 、 `reset`とです。 |
| id | String | アクティビティの一意識別子。 読み取り専用です。 |
| successfulActivityCount | Int64 | 成功した登録またはリセットの数を提供します。 |

## <a name="relationships"></a>リレーションシップ

なし。

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUsageSummary",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "feature":"string",
  "successfulActivityCount":"Int64",
  "failureActivityCount": "Int64",
  "authMethod": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credentialUsageSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->