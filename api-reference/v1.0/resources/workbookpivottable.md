---
title: ピボットテーブル リソースの種類
description: Excel のピボットテーブルを表します。
ms.openlocfilehash: b4ddd0c1bb9e4ee13aaf3d1b4472c4e750e3a755
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020870"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="6e6d5-103">ピボットテーブル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6e6d5-103">pivotTable resource type</span></span>

<span data-ttu-id="6e6d5-104">Excel のピボットテーブルを表します。</span><span class="sxs-lookup"><span data-stu-id="6e6d5-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="6e6d5-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="6e6d5-105">Methods</span></span>

| <span data-ttu-id="6e6d5-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="6e6d5-106">Method</span></span>           | <span data-ttu-id="6e6d5-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6e6d5-107">Return Type</span></span>    |<span data-ttu-id="6e6d5-108">説明</span><span class="sxs-lookup"><span data-stu-id="6e6d5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6e6d5-109">workbookPivotTable を取得する</span><span class="sxs-lookup"><span data-stu-id="6e6d5-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="6e6d5-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="6e6d5-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="6e6d5-111">worksheetprotection オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6e6d5-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="6e6d5-112">更新</span><span class="sxs-lookup"><span data-stu-id="6e6d5-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="6e6d5-113">なし</span><span class="sxs-lookup"><span data-stu-id="6e6d5-113">None</span></span>|<span data-ttu-id="6e6d5-114">ピボットテーブルを更新します。</span><span class="sxs-lookup"><span data-stu-id="6e6d5-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="6e6d5-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="6e6d5-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="6e6d5-116">なし</span><span class="sxs-lookup"><span data-stu-id="6e6d5-116">None</span></span>|<span data-ttu-id="6e6d5-p101">指定したワークシート内のすべてのテーブルを更新します。このアクションは、ピボットテーブルのコレクションでのみ使用できることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="6e6d5-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="6e6d5-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e6d5-119">Properties</span></span>
| <span data-ttu-id="6e6d5-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e6d5-120">Property</span></span>     | <span data-ttu-id="6e6d5-121">型</span><span class="sxs-lookup"><span data-stu-id="6e6d5-121">Type</span></span>   |<span data-ttu-id="6e6d5-122">説明</span><span class="sxs-lookup"><span data-stu-id="6e6d5-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e6d5-123">id</span><span class="sxs-lookup"><span data-stu-id="6e6d5-123">id</span></span>|<span data-ttu-id="6e6d5-124">String</span><span class="sxs-lookup"><span data-stu-id="6e6d5-124">String</span></span>| <span data-ttu-id="6e6d5-p102">ピボットテーブルの ID。 読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6e6d5-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="6e6d5-127">name</span><span class="sxs-lookup"><span data-stu-id="6e6d5-127">name</span></span>|<span data-ttu-id="6e6d5-128">String</span><span class="sxs-lookup"><span data-stu-id="6e6d5-128">String</span></span>|<span data-ttu-id="6e6d5-129">ピボットテーブルの名前。</span><span class="sxs-lookup"><span data-stu-id="6e6d5-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="6e6d5-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6e6d5-130">Relationships</span></span>
| <span data-ttu-id="6e6d5-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6e6d5-131">Relationship</span></span> | <span data-ttu-id="6e6d5-132">型</span><span class="sxs-lookup"><span data-stu-id="6e6d5-132">Type</span></span>   |<span data-ttu-id="6e6d5-133">説明</span><span class="sxs-lookup"><span data-stu-id="6e6d5-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e6d5-134">ワークシート</span><span class="sxs-lookup"><span data-stu-id="6e6d5-134">worksheet</span></span>|[<span data-ttu-id="6e6d5-135">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="6e6d5-135">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="6e6d5-p103">現在のピボットテーブルを含んでいるワークシート。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="6e6d5-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="6e6d5-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6e6d5-138">JSON representation</span></span>
<span data-ttu-id="6e6d5-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6e6d5-139">Here is a JSON representation of the resource.</span></span>

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
