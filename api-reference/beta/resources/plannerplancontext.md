---
title: プラン "context/プラン" コンテキストリソースの種類
description: '**plan by コンテキスト**リソースは、Planner の外部のユーザー環境に対するプランの関係を表します。 Planner のプランは、Microsoft Teams などの他のエクスペリエンスで提示して、そのエクスペリエンスのコンテキストで作業を追跡することができます。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 68d9233d2645c2176ad364fbcbfac869976f0586
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344450"
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
|createdDateTime|DateTimeOffset|読み取り専用。 **プラン**が作成された日付と時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。|
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
  "suppressions": []
}
-->
