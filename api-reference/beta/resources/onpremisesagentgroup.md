---
title: onPremisesAgentGroup リソースの種類
description: onPremisesAgentGroup リソースの種類。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9e74a49a9a8c4b57232ed90cef232fa8b7feb998
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841319"
---
# <a name="onpremisesagentgroup-resource-type"></a>onPremisesAgentGroup リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

オンプレミスのエージェントグループを表します。 エージェントグループを使用すると、テナント管理者は特定の[エージェント](onpremisesagent.md)を割り当てて、発行された特定[の社内リソース](publishedresource.md)を提供できます。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [リスト onPremisesAgentGroups](../api/onpremisesagentgroup-list.md) | onPremisesAgentGroups コレクション | **OnPremisesAgentGroup** objects コレクションを取得します。 |
| [OnPremisesAgentGroup を取得する](../api/onpremisesagentgroup-get.md) | [onPremisesAgentGroup](onpremisesagentgroup.md) | **OnPremisesAgentGroup**オブジェクトのプロパティとリレーションシップを読み取ります。 |
| [OnPremisesAgentGroup を作成する](../api/onpremisesagentgroup-post.md)  | [onPremisesAgentGroup](onpremisesagentgroup.md) | 新しい**onPremisesAgentGroup**を作成します。 |
| [OnPremisesAgentGroup の更新](../api/onpremisesagentgroup-update.md) | [onPremisesAgentGroup](onpremisesagentgroup.md) | **OnPremisesAgentGroup**オブジェクトを更新します。 |
| [OnPremisesAgentGroup の削除](../api/onpremisesagentgroup-delete.md) | None | **OnPremisesAgentGroup**オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|displayName|String|**OnPremisesAgentGroup**の表示名。|
|id|文字列| **OnPremisesAgentGroup**のオブジェクト ID。 読み取り専用です。|
|isDefault|ブール型 (Boolean)|**OnPremisesAgentGroup**が既定のエージェントグループであるかどうかを示します。 既定の**onPremisesAgentGroup**にすることができ、システムによって設定されるのは、1つのエージェントグループのみです。|
|発行の種類|string| 可能な値は、`appProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration` です。|

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型        | 説明 |
|:-------------|:------------|:------------|
|エージェント|[onPremisesAgent](onpremisesagent.md)コレクション| **OnPremisesAgentGroup**に割り当てられている**onPremisesAgent**のリスト。 読み取り専用です。 Null 許容型。|
|publishedResources|[Publishedresource](publishedresource.md)コレクション| **OnPremisesAgentGroup**に割り当てられている**publishedresource**のリスト。 読み取り専用です。 Null 許容型。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesAgentGroup",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "isDefault": true,
  "publishingType": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesAgentGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
