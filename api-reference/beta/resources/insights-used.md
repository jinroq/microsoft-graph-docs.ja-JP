---
title: Used リソースの種類
description: 特定のユーザーが使用するドキュメントを表す洞察。 Insights は、ユーザーが表示またはアクセスした最も関連性のあるドキュメントを返します。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 2b6e7a7c4df94e9ffbcb34ef200457b4a903eb24
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005689"
---
# <a name="usedinsight-resource-type"></a>Used リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特定のユーザーが使用するドキュメントを表す洞察。 Insights は、ユーザーが表示またはアクセスした最も関連性のあるドキュメントを返します。 これには次のドキュメントが含まれます。

- OneDrive for Business
- SharePoint

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[使用するリスト](../api/insights-list-used.md) |[usedInsight](insights-used.md) コレクション| 使用されているファイルの一覧を取得します。|

## <a name="properties"></a>プロパティ

| プロパティ              | 型                      | 説明  |
| -------------         |---------------            | -------------|
| id                    | String                    | リレーションシップの一意識別子。 読み取り専用です。        |
| lastUsed              | [usageDetails](insights-usagedetails.md)              | ユーザーが最後にアイテムを表示および変更した日時に関する情報。 読み取り専用です。     |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | ユーザーの作業でドキュメントをビジュアル化するために使用できるプロパティ。 読み取り専用      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | ドキュメントの url や種類など、使用されているドキュメントの参照プロパティ。 読み取り専用     |

## <a name="relationships"></a>リレーションシップ

| プロパティ      | 型          | 説明  |
| ------------- |---------------| -------------|
| リソース      | [entity](entity.md)コレクション    | 使用されたアイテムに移動するために使用されます。 添付ファイルの場合、type は*Fileattachment*になります。 リンクされた添付ファイルの場合、種類は [*ドライブ] 項目*です。 |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
    "resource"
  ],
  "@odata.type": "microsoft.graph.usedInsight"
}-->

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": { "@odata.type": "microsoft.graph.resourceVisualization" },
  "resourceReference": { "@odata.type": "microsoft.graph.resourceReference" }
}
```
