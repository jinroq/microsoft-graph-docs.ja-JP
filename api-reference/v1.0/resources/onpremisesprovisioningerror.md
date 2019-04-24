---
title: onPremisesProvisioningError リソースの種類
description: オンプレミスのディレクトリを Azure Active directory と同期するときに、ユーザーエンティティおよびグループエンティティのディレクトリ同期エラーを表します。
localization_priority: Normal
ms.openlocfilehash: c8989a78dfb60a6c7c25a66a9f1e619dcbdca15d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462684"
---
# <a name="onpremisesprovisioningerror-resource-type"></a>onPremisesProvisioningError リソースの種類

オンプレミスのディレクトリを Azure Active directory と同期するときに、[ユーザー](user.md)エンティティおよび[グループ](group.md)エンティティのディレクトリ同期エラーを表します。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|category|String| プロビジョニングエラーのカテゴリ。 注: 現時点では、可能な値は1つだけです。 可能な値: *propertyconflict* -プロパティ値が一意ではないことを示します。 その他のオブジェクトには、プロパティと同じ値が含まれています。 |
|occurredDateTime|DateTimeOffset| エラーが発生した日付と時刻。 |
|propertycain error|String| エラーを引き起こしたディレクトリプロパティの名前。 現在使用可能な値: *UserPrincipalName*または*ProxyAddress* |
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
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
