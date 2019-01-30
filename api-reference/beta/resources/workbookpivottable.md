---
title: ピボットテーブル リソースの種類
description: Excel のピボットテーブルを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: fc43bf160e93e354ff58b2f960e8ec38d252287f
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641107"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="aff73-103">ピボットテーブル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aff73-103">pivotTable resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aff73-104">Excel のピボットテーブルを表します。</span><span class="sxs-lookup"><span data-stu-id="aff73-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="aff73-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="aff73-105">Methods</span></span>

| <span data-ttu-id="aff73-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="aff73-106">Method</span></span>           | <span data-ttu-id="aff73-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="aff73-107">Return Type</span></span>    |<span data-ttu-id="aff73-108">説明</span><span class="sxs-lookup"><span data-stu-id="aff73-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aff73-109">workbookPivotTable を取得する</span><span class="sxs-lookup"><span data-stu-id="aff73-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="aff73-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="aff73-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="aff73-111">worksheetprotection オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="aff73-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="aff73-112">更新</span><span class="sxs-lookup"><span data-stu-id="aff73-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="aff73-113">なし</span><span class="sxs-lookup"><span data-stu-id="aff73-113">None</span></span>|<span data-ttu-id="aff73-114">ピボットテーブルを更新します。</span><span class="sxs-lookup"><span data-stu-id="aff73-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="aff73-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="aff73-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="aff73-116">なし</span><span class="sxs-lookup"><span data-stu-id="aff73-116">None</span></span>|<span data-ttu-id="aff73-p101">指定したワークシート内のすべてのテーブルを更新します。このアクションは、ピボットテーブルのコレクションでのみ使用できることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="aff73-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="aff73-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aff73-119">Properties</span></span>
| <span data-ttu-id="aff73-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aff73-120">Property</span></span>     | <span data-ttu-id="aff73-121">型</span><span class="sxs-lookup"><span data-stu-id="aff73-121">Type</span></span>   |<span data-ttu-id="aff73-122">説明</span><span class="sxs-lookup"><span data-stu-id="aff73-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aff73-123">id</span><span class="sxs-lookup"><span data-stu-id="aff73-123">id</span></span>|<span data-ttu-id="aff73-124">String</span><span class="sxs-lookup"><span data-stu-id="aff73-124">String</span></span>| <span data-ttu-id="aff73-p102">ピボットテーブルの ID。 読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="aff73-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="aff73-127">name</span><span class="sxs-lookup"><span data-stu-id="aff73-127">name</span></span>|<span data-ttu-id="aff73-128">String</span><span class="sxs-lookup"><span data-stu-id="aff73-128">String</span></span>|<span data-ttu-id="aff73-129">ピボットテーブルの名前。</span><span class="sxs-lookup"><span data-stu-id="aff73-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="aff73-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aff73-130">Relationships</span></span>
| <span data-ttu-id="aff73-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aff73-131">Relationship</span></span> | <span data-ttu-id="aff73-132">型</span><span class="sxs-lookup"><span data-stu-id="aff73-132">Type</span></span>   |<span data-ttu-id="aff73-133">説明</span><span class="sxs-lookup"><span data-stu-id="aff73-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aff73-134">ワークシート</span><span class="sxs-lookup"><span data-stu-id="aff73-134">worksheet</span></span>|[<span data-ttu-id="aff73-135">worksheet</span><span class="sxs-lookup"><span data-stu-id="aff73-135">worksheet</span></span>](worksheet.md)| <span data-ttu-id="aff73-p103">現在のピボットテーブルを含んでいるワークシート。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="aff73-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="aff73-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aff73-138">JSON representation</span></span>
<span data-ttu-id="aff73-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="aff73-139">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookPivotTable"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/workbookpivottable.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
