---
title: publishedResource リソースの種類
description: publishedResource リソースの種類。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 54a2b1b610f30ec3ce7d9853916aad345142cbf0
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841361"
---
# <a name="publishedresource-resource-type"></a>publishedResource リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

オンプレミスで発行されたリソースを表します。 テナント管理者は、テナント管理者によってインストールされたエンタープライズアプリケーション、ドメインコントローラー、サーバー、その他の[オンプレミスエージェント](onpremisesagent.md)を、さまざまな種類のオンプレミスのリソースに公開することができます。発行された特定のリソース。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [PublishedResources のリスト](../api/publishedresource-list.md) | [Publishedresource](publishedresource.md) objects コレクション | **Publishedresources**オブジェクトコレクションを取得します。 |
| [PublishedResource の取得](../api/publishedresource-get.md) | [publishedResource](publishedresource.md) | **Publishedresource**オブジェクトのプロパティとリレーションシップを読み取ります。 |
| [PublishedResource の作成](../api/publishedresource-post.md) |  [publishedResource](publishedresource.md)  | 新しい**Publishedresource**を作成します。 |
| [PublishedResource の更新](../api/publishedresource-update.md) | [publishedResource](publishedresource.md) | **Publishedresource**オブジェクトを更新します。 |
| [PublishedResource の削除](../api/publishedresource-delete.md) | None | **Publishedresource**オブジェクトを削除します。 |
| [PublishedResource を onPremisesAgentGroup に割り当てます。](../api/publishedresource-post-agentgroups.md) | None | **Publishedresource**オブジェクトを**onPremisesAgentGroup**に割り当てます。 |
| [OnPremisesAgentGroup から publishedResource を削除する](../api/publishedresource-delete-agentgroups.md) | None |  **OnPremisesAgentGroup**から**publishedresource**オブジェクトを削除します。|

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|displayName|String| PublishedResource の表示名。|
|id|文字列| PublishedResource のオブジェクト id。 読み取り専用です。|
|発行の種類|string| 可能な値は、`appProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration` です。|
|resourceName|String|PublishedResource の名前。|

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型        | 説明 |
|:-------------|:------------|:------------|
|agentGroups|[onPremisesAgentGroup](onpremisesagentgroup.md)コレクション| **Publishedresource**が割り当てられている**onPremisesAgentGroups**のリスト。 読み取り専用です。 Null 許容型。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.publishedResource",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "publishingType": "string",
  "resourceName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "publishedResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
