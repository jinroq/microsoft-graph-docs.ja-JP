---
title: ピボットテーブル リソースの種類
description: Excel のピボットテーブルを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c5b841495b19a81967ba056f702a88c4cbe74efc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033363"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="23958-103">ピボットテーブル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="23958-103">pivotTable resource type</span></span>

<span data-ttu-id="23958-104">Excel のピボットテーブルを表します。</span><span class="sxs-lookup"><span data-stu-id="23958-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="23958-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="23958-105">Methods</span></span>

| <span data-ttu-id="23958-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="23958-106">Method</span></span>           | <span data-ttu-id="23958-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="23958-107">Return Type</span></span>    |<span data-ttu-id="23958-108">説明</span><span class="sxs-lookup"><span data-stu-id="23958-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="23958-109">workbookPivotTable を取得する</span><span class="sxs-lookup"><span data-stu-id="23958-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="23958-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="23958-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="23958-111">worksheetprotection オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="23958-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="23958-112">更新</span><span class="sxs-lookup"><span data-stu-id="23958-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="23958-113">None</span><span class="sxs-lookup"><span data-stu-id="23958-113">None</span></span>|<span data-ttu-id="23958-114">ピボットテーブルを更新します。</span><span class="sxs-lookup"><span data-stu-id="23958-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="23958-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="23958-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="23958-116">なし</span><span class="sxs-lookup"><span data-stu-id="23958-116">None</span></span>|<span data-ttu-id="23958-p101">指定したワークシート内のすべてのテーブルを更新します。このアクションは、ピボットテーブルのコレクションでのみ使用できることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="23958-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="23958-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23958-119">Properties</span></span>
| <span data-ttu-id="23958-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23958-120">Property</span></span>     | <span data-ttu-id="23958-121">型</span><span class="sxs-lookup"><span data-stu-id="23958-121">Type</span></span>   |<span data-ttu-id="23958-122">説明</span><span class="sxs-lookup"><span data-stu-id="23958-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23958-123">id</span><span class="sxs-lookup"><span data-stu-id="23958-123">id</span></span>|<span data-ttu-id="23958-124">文字列</span><span class="sxs-lookup"><span data-stu-id="23958-124">String</span></span>| <span data-ttu-id="23958-p102">ピボットテーブルの ID。 読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="23958-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="23958-127">name</span><span class="sxs-lookup"><span data-stu-id="23958-127">name</span></span>|<span data-ttu-id="23958-128">String</span><span class="sxs-lookup"><span data-stu-id="23958-128">String</span></span>|<span data-ttu-id="23958-129">ピボットテーブルの名前。</span><span class="sxs-lookup"><span data-stu-id="23958-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="23958-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="23958-130">Relationships</span></span>
| <span data-ttu-id="23958-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="23958-131">Relationship</span></span> | <span data-ttu-id="23958-132">型</span><span class="sxs-lookup"><span data-stu-id="23958-132">Type</span></span>   |<span data-ttu-id="23958-133">説明</span><span class="sxs-lookup"><span data-stu-id="23958-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23958-134">worksheet</span><span class="sxs-lookup"><span data-stu-id="23958-134">worksheet</span></span>|[<span data-ttu-id="23958-135">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="23958-135">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="23958-136">現在のピボットテーブルを含んでいるワークシート。</span><span class="sxs-lookup"><span data-stu-id="23958-136">The worksheet containing the current PivotTable.</span></span> <span data-ttu-id="23958-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="23958-137">Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="23958-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="23958-138">JSON representation</span></span>
<span data-ttu-id="23958-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="23958-139">Here is a JSON representation of the resource.</span></span>

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
