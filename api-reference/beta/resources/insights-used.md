---
title: 使用されるリソースの種類
description: 特定のユーザーが使用するドキュメントを表す洞察。 insights は、ユーザーが表示またはアクセスした最も関連性のあるドキュメントを返します。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 35698741cd457f4e8d202b13dd9099bb2669b6e1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551292"
---
# <a name="used-resource-type"></a>使用されるリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特定のユーザーが使用するドキュメントを表す洞察。 insights は、ユーザーが表示またはアクセスした最も関連性のあるドキュメントを返します。 これには次のドキュメントが含まれます。

- OneDrive for Business
- SharePoint

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[使用するリスト](../api/insights-list-used.md) |[insights_used](insights-used.md)コレクション| 使用されているファイルの一覧を取得します。|

## <a name="properties"></a>プロパティ

| プロパティ              | 型                      | 説明  |
| -------------         |---------------            | -------------|
| id                    | String                    | リレーションシップの一意識別子。 読み取り専用です。        |
| lastused              | [usageDetails](insights-usagedetails.md)              | ユーザーが最後にアイテムを表示および変更した日時に関する情報。 読み取り専用です。     |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | ユーザーの作業でドキュメントをビジュアル化するために使用できるプロパティ。 読み取り専用      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | ドキュメントの url や種類など、使用されているドキュメントの参照プロパティ。 読み取り専用     |

## <a name="relationships"></a>リレーションシップ

| プロパティ      | 型          | 説明  |
| ------------- |---------------| -------------|
| リソース      | エンティティ        | 使用されたアイテムに移動するために使用されます。 添付ファイルの場合、type は*fileattachment*になります。 リンクされた添付ファイルの場合、種類は [*ドライブ] 項目*です。 |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-used.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
