---
title: workbookPivotTable リソースの種類
description: Excel のピボットテーブルを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: d8df88699fde1e4d5562db6299cd12665512c03b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963994"
---
# <a name="workbookpivottable-resource-type"></a><span data-ttu-id="1de79-103">workbookPivotTable リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1de79-103">workbookPivotTable resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1de79-104">Excel のピボットテーブルを表します。</span><span class="sxs-lookup"><span data-stu-id="1de79-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="1de79-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="1de79-105">Methods</span></span>

| <span data-ttu-id="1de79-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="1de79-106">Method</span></span>           | <span data-ttu-id="1de79-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1de79-107">Return Type</span></span>    |<span data-ttu-id="1de79-108">説明</span><span class="sxs-lookup"><span data-stu-id="1de79-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1de79-109">workbookPivotTable を取得する</span><span class="sxs-lookup"><span data-stu-id="1de79-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="1de79-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="1de79-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="1de79-111">worksheetprotection オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1de79-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="1de79-112">更新</span><span class="sxs-lookup"><span data-stu-id="1de79-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="1de79-113">None</span><span class="sxs-lookup"><span data-stu-id="1de79-113">None</span></span>|<span data-ttu-id="1de79-114">ピボットテーブルを更新します。</span><span class="sxs-lookup"><span data-stu-id="1de79-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="1de79-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="1de79-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="1de79-116">なし</span><span class="sxs-lookup"><span data-stu-id="1de79-116">None</span></span>|<span data-ttu-id="1de79-p101">指定したワークシート内のすべてのテーブルを更新します。このアクションは、ピボットテーブルのコレクションでのみ使用できることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="1de79-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="1de79-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1de79-119">Properties</span></span>
| <span data-ttu-id="1de79-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1de79-120">Property</span></span>     | <span data-ttu-id="1de79-121">型</span><span class="sxs-lookup"><span data-stu-id="1de79-121">Type</span></span>   |<span data-ttu-id="1de79-122">説明</span><span class="sxs-lookup"><span data-stu-id="1de79-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1de79-123">id</span><span class="sxs-lookup"><span data-stu-id="1de79-123">id</span></span>|<span data-ttu-id="1de79-124">文字列</span><span class="sxs-lookup"><span data-stu-id="1de79-124">String</span></span>| <span data-ttu-id="1de79-p102">ピボットテーブルの ID。 読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1de79-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="1de79-127">name</span><span class="sxs-lookup"><span data-stu-id="1de79-127">name</span></span>|<span data-ttu-id="1de79-128">String</span><span class="sxs-lookup"><span data-stu-id="1de79-128">String</span></span>|<span data-ttu-id="1de79-129">ピボットテーブルの名前。</span><span class="sxs-lookup"><span data-stu-id="1de79-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="1de79-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1de79-130">Relationships</span></span>
| <span data-ttu-id="1de79-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1de79-131">Relationship</span></span> | <span data-ttu-id="1de79-132">型</span><span class="sxs-lookup"><span data-stu-id="1de79-132">Type</span></span>   |<span data-ttu-id="1de79-133">説明</span><span class="sxs-lookup"><span data-stu-id="1de79-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1de79-134">ワークシート</span><span class="sxs-lookup"><span data-stu-id="1de79-134">worksheet</span></span>|[<span data-ttu-id="1de79-135">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="1de79-135">workbookWorksheet</span></span>](workbookworksheet.md)| <span data-ttu-id="1de79-136">現在のピボットテーブルを含んでいるワークシート。</span><span class="sxs-lookup"><span data-stu-id="1de79-136">The worksheet containing the current PivotTable.</span></span> <span data-ttu-id="1de79-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1de79-137">Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="1de79-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1de79-138">JSON representation</span></span>
<span data-ttu-id="1de79-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1de79-139">Here is a JSON representation of the resource.</span></span>

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
