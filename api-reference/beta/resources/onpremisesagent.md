---
title: onPremisesAgent リソースの種類
description: onPremisesAgent リソースの種類。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1bcff659cf30b946654f14190b2cf5f693d27bc4
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841263"
---
# <a name="onpremisesagent-resource-type"></a>onPremisesAgent リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

オンプレミスのエージェントを表します。 テナント管理者によってインストールされた社内エージェントは、発行された特定の[リソース](publishedresource.md)への要求にアクセスしたり、処理したりするように構成できます。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [リスト onPremisesAgents](../api/onpremisesagent-list.md) | [onPremisesAgent](onpremisesagent.md)コレクション | **OnPremisesAgents**オブジェクトのコレクションを取得します。 |
| [OnPremisesAgent を取得する](../api/onpremisesagent-get.md) | [onPremisesAgent](onpremisesagent.md) | **OnPremisesAgent**オブジェクトのプロパティとリレーションシップを読み取ります。 |
| [OnPremisesAgent を onPremisesAgentGroup に割り当てる](../api/onpremisesagent-post-agentgroups.md) | None | **OnPremisesAgent**を**onPremisesAgentGroup**に割り当てます。|
| [OnPremisesAgentGroup から onpremisesAgent を削除する](../api/onpremisesagent-delete-agentgroups.md) | None | **OnPremisesAgentGroup**から**onPremisesAgent**を削除します。 |

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|externalIp|String|エージェントコンピューターのサービスによって検出された外部 IP アドレス。 読み取り専用|
|id|文字列| OnPremisesAgent のオブジェクト id。 読み取り専用です。|
|マシン|String|Aggent が実行されているコンピューターの名前。 読み取り専用|
|status|string| 可能な値は、`active`、`inactive` です。|
|発行の種類|string| 可能な値は、`appProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration` です。|

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型        | 説明 |
|:-------------|:------------|:------------|
|agentGroups|[onPremisesAgentGroup](onpremisesagentgroup.md)コレクション| **OnPremisesAgent**が割り当てられている**onPremisesAgentGroups**のリスト。 読み取り専用。 Null 許容型。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesAgent",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "externalIp": "String",
  "id": "String (identifier)",
  "machineName": "String",
  "status": "string",
  "supportedPublishingTypes": ["string"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesAgent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
