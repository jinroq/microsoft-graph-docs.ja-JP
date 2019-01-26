---
title: ピボットテーブル リソースの種類
description: Excel のピボットテーブルを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 774c407022d700bc5856dc780eff3a6dafa6bc4e
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577460"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="091e6-103">ピボットテーブル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="091e6-103">pivotTable resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="091e6-104">Excel のピボットテーブルを表します。</span><span class="sxs-lookup"><span data-stu-id="091e6-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="091e6-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="091e6-105">Methods</span></span>

| <span data-ttu-id="091e6-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="091e6-106">Method</span></span>           | <span data-ttu-id="091e6-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="091e6-107">Return Type</span></span>    |<span data-ttu-id="091e6-108">説明</span><span class="sxs-lookup"><span data-stu-id="091e6-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="091e6-109">workbookPivotTable を取得する</span><span class="sxs-lookup"><span data-stu-id="091e6-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="091e6-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="091e6-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="091e6-111">worksheetprotection オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="091e6-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="091e6-112">更新</span><span class="sxs-lookup"><span data-stu-id="091e6-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="091e6-113">なし</span><span class="sxs-lookup"><span data-stu-id="091e6-113">None</span></span>|<span data-ttu-id="091e6-114">ピボットテーブルを更新します。</span><span class="sxs-lookup"><span data-stu-id="091e6-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="091e6-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="091e6-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="091e6-116">なし</span><span class="sxs-lookup"><span data-stu-id="091e6-116">None</span></span>|<span data-ttu-id="091e6-p101">指定したワークシート内のすべてのテーブルを更新します。このアクションは、ピボットテーブルのコレクションでのみ使用できることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="091e6-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="091e6-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="091e6-119">Properties</span></span>
| <span data-ttu-id="091e6-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="091e6-120">Property</span></span>     | <span data-ttu-id="091e6-121">型</span><span class="sxs-lookup"><span data-stu-id="091e6-121">Type</span></span>   |<span data-ttu-id="091e6-122">説明</span><span class="sxs-lookup"><span data-stu-id="091e6-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="091e6-123">id</span><span class="sxs-lookup"><span data-stu-id="091e6-123">id</span></span>|<span data-ttu-id="091e6-124">String</span><span class="sxs-lookup"><span data-stu-id="091e6-124">String</span></span>| <span data-ttu-id="091e6-p102">ピボットテーブルの ID。 読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="091e6-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="091e6-127">name</span><span class="sxs-lookup"><span data-stu-id="091e6-127">name</span></span>|<span data-ttu-id="091e6-128">String</span><span class="sxs-lookup"><span data-stu-id="091e6-128">String</span></span>|<span data-ttu-id="091e6-129">ピボットテーブルの名前。</span><span class="sxs-lookup"><span data-stu-id="091e6-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="091e6-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="091e6-130">Relationships</span></span>
| <span data-ttu-id="091e6-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="091e6-131">Relationship</span></span> | <span data-ttu-id="091e6-132">型</span><span class="sxs-lookup"><span data-stu-id="091e6-132">Type</span></span>   |<span data-ttu-id="091e6-133">説明</span><span class="sxs-lookup"><span data-stu-id="091e6-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="091e6-134">worksheet</span><span class="sxs-lookup"><span data-stu-id="091e6-134">worksheet</span></span>|[<span data-ttu-id="091e6-135">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="091e6-135">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="091e6-p103">現在のピボットテーブルを含んでいるワークシート。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="091e6-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="091e6-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="091e6-138">JSON representation</span></span>
<span data-ttu-id="091e6-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="091e6-139">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
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
