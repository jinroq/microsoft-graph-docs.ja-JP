---
title: プラン "context/プラン" コンテキストリソースの種類
description: '**plan by コンテキスト**リソースは、Planner の外部のユーザー環境に対するプランの関係を表します。 Planner のプランは、Microsoft Teams などの他のエクスペリエンスで提示して、そのエクスペリエンスのコンテキストで作業を追跡することができます。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 76260b51bc6f77acf6fac22e80bd676edd8b8e11
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522161"
---
# <a name="plannerplancontext-resource-type"></a>プラン "context/プラン" コンテキストリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**plan by コンテキスト**リソースは、Planner の外部のユーザー環境に対する[プラン](plannerplan.md)の関係を表します。 Planner のプランは、Microsoft Teams などの他のエクスペリエンスで提示して、そのエクスペリエンスのコンテキストで作業を追跡することができます。
**プランのコンテキスト**エントリ再生機能は、 **ownerappid**プロパティに基づいて識別できます。
 - 5e3ce6c0-2b1f-4285-8d4b-75ee78787346: コンテキストエントリは Microsoft Teams に属しています。
 - 00000003-0000-0ff1-ce00-000000000000: コンテキストエントリは SharePoint に属しています。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|associationType|String|Null 許容型。 アプリケーションで定義された、[プラン](plannerplan.md)とアプリの間の関連付けの種類。 アプリはこの情報を使用して、同じ[プラン](plannerplan.md)の異なる種類のリレーションシップを追跡できます。|
|createdDateTime|DateTimeOffset|読み取り専用。 **プラン**が作成された日付と時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|displaynamesegments|String collection|外部環境の名前のセグメント。 セグメントは、他のアプリがリレーションシップを表示できる階層構造を表します。|
|ownerappid|String|読み取り専用です。 **プランのコンテキスト**を作成したアプリの ID です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContext"
}-->

```json
{
  "associationType": "Board",
  "createdDateTime": "2015-10-14T00:57:28.4698344Z",
  "displayNameSegments": [
    "Finance Team",
    "Budget Plans"
  ],
  "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContext resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplancontext.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
