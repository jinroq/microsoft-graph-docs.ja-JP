---
title: onPremisesProvisioningError リソースの種類
description: オンプレミスのディレクトリを Azure Active Directory と同期するときの、ユーザー、グループ、または組織の連絡先エンティティのディレクトリ同期エラーを表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 240b7f100a01c37b6b778d3b18b0297739ada66b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966372"
---
# <a name="onpremisesprovisioningerror-resource-type"></a>onPremisesProvisioningError リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

オンプレミスのディレクトリを Azure Active Directory と同期するときの、[ユーザー](user.md)、[グループ](group.md)、または[組織の連絡先](orgcontact.md)エンティティのディレクトリ同期エラーを表します。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|category|String| プロビジョニングエラーのカテゴリ。 注: 現時点では、可能な値は1つだけです。 可能な値: *Propertyconflict* -プロパティ値が一意ではないことを示します。 その他のオブジェクトには、プロパティと同じ値が含まれています。 |
|occurredDateTime|DateTimeOffset| エラーが発生した日付と時刻。 |
|Propertycain Error|String| エラーを引き起こしたディレクトリプロパティの名前。 現在使用可能な値: *UserPrincipalName*または*ProxyAddress* |
|value|文字列型 (String)| エラーが発生したプロパティの値。 |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesProvisioningError"
}-->

```json
{
  "category": "String",
  "occurredDateTime": "String (timestamp)",
  "propertyCausingError": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
