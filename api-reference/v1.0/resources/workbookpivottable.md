---
title: ピボットテーブル リソースの種類
description: Excel のピボットテーブルを表します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: d500d4bc88608b032262cfae505385bf7ed3f072
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889209"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="69270-103">ピボットテーブル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="69270-103">pivotTable resource type</span></span>

<span data-ttu-id="69270-104">Excel のピボットテーブルを表します。</span><span class="sxs-lookup"><span data-stu-id="69270-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="69270-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="69270-105">Methods</span></span>

| <span data-ttu-id="69270-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="69270-106">Method</span></span>           | <span data-ttu-id="69270-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="69270-107">Return Type</span></span>    |<span data-ttu-id="69270-108">説明</span><span class="sxs-lookup"><span data-stu-id="69270-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="69270-109">workbookPivotTable を取得する</span><span class="sxs-lookup"><span data-stu-id="69270-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="69270-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="69270-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="69270-111">worksheetprotection オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="69270-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="69270-112">更新</span><span class="sxs-lookup"><span data-stu-id="69270-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="69270-113">なし</span><span class="sxs-lookup"><span data-stu-id="69270-113">None</span></span>|<span data-ttu-id="69270-114">ピボットテーブルを更新します。</span><span class="sxs-lookup"><span data-stu-id="69270-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="69270-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="69270-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="69270-116">なし</span><span class="sxs-lookup"><span data-stu-id="69270-116">None</span></span>|<span data-ttu-id="69270-p101">指定したワークシート内のすべてのテーブルを更新します。このアクションは、ピボットテーブルのコレクションでのみ使用できることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="69270-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="69270-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69270-119">Properties</span></span>
| <span data-ttu-id="69270-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69270-120">Property</span></span>     | <span data-ttu-id="69270-121">種類</span><span class="sxs-lookup"><span data-stu-id="69270-121">Type</span></span>   |<span data-ttu-id="69270-122">説明</span><span class="sxs-lookup"><span data-stu-id="69270-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69270-123">ID</span><span class="sxs-lookup"><span data-stu-id="69270-123">id</span></span>|<span data-ttu-id="69270-124">String</span><span class="sxs-lookup"><span data-stu-id="69270-124">String</span></span>| <span data-ttu-id="69270-p102">ピボットテーブルの ID。 読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="69270-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="69270-127">name</span><span class="sxs-lookup"><span data-stu-id="69270-127">name</span></span>|<span data-ttu-id="69270-128">String</span><span class="sxs-lookup"><span data-stu-id="69270-128">String</span></span>|<span data-ttu-id="69270-129">ピボットテーブルの名前。</span><span class="sxs-lookup"><span data-stu-id="69270-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="69270-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="69270-130">Relationships</span></span>
| <span data-ttu-id="69270-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="69270-131">Relationship</span></span> | <span data-ttu-id="69270-132">型</span><span class="sxs-lookup"><span data-stu-id="69270-132">Type</span></span>   |<span data-ttu-id="69270-133">説明</span><span class="sxs-lookup"><span data-stu-id="69270-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69270-134">ワークシート</span><span class="sxs-lookup"><span data-stu-id="69270-134">worksheet</span></span>|[<span data-ttu-id="69270-135">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="69270-135">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="69270-p103">現在のピボットテーブルを含んでいるワークシート。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="69270-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="69270-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="69270-138">JSON representation</span></span>
<span data-ttu-id="69270-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="69270-139">Here is a JSON representation of the resource.</span></span>

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
