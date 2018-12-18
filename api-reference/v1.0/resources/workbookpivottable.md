---
title: ピボットテーブル リソースの種類
description: Excel のピボットテーブルを表します。
author: lumine2008
ms.openlocfilehash: 68075aebeac9c0846e48739daf65e5bf97e4d6f5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334112"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="189b8-103">ピボットテーブル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="189b8-103">pivotTable resource type</span></span>

<span data-ttu-id="189b8-104">Excel のピボットテーブルを表します。</span><span class="sxs-lookup"><span data-stu-id="189b8-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="189b8-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="189b8-105">Methods</span></span>

| <span data-ttu-id="189b8-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="189b8-106">Method</span></span>           | <span data-ttu-id="189b8-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="189b8-107">Return Type</span></span>    |<span data-ttu-id="189b8-108">説明</span><span class="sxs-lookup"><span data-stu-id="189b8-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="189b8-109">workbookPivotTable を取得する</span><span class="sxs-lookup"><span data-stu-id="189b8-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="189b8-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="189b8-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="189b8-111">worksheetprotection オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="189b8-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="189b8-112">更新</span><span class="sxs-lookup"><span data-stu-id="189b8-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="189b8-113">なし</span><span class="sxs-lookup"><span data-stu-id="189b8-113">None</span></span>|<span data-ttu-id="189b8-114">ピボットテーブルを更新します。</span><span class="sxs-lookup"><span data-stu-id="189b8-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="189b8-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="189b8-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="189b8-116">なし</span><span class="sxs-lookup"><span data-stu-id="189b8-116">None</span></span>|<span data-ttu-id="189b8-p101">指定したワークシート内のすべてのテーブルを更新します。このアクションは、ピボットテーブルのコレクションでのみ使用できることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="189b8-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="189b8-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="189b8-119">Properties</span></span>
| <span data-ttu-id="189b8-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="189b8-120">Property</span></span>     | <span data-ttu-id="189b8-121">種類</span><span class="sxs-lookup"><span data-stu-id="189b8-121">Type</span></span>   |<span data-ttu-id="189b8-122">説明</span><span class="sxs-lookup"><span data-stu-id="189b8-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="189b8-123">ID</span><span class="sxs-lookup"><span data-stu-id="189b8-123">id</span></span>|<span data-ttu-id="189b8-124">String</span><span class="sxs-lookup"><span data-stu-id="189b8-124">String</span></span>| <span data-ttu-id="189b8-p102">ピボットテーブルの ID。 読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="189b8-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="189b8-127">name</span><span class="sxs-lookup"><span data-stu-id="189b8-127">name</span></span>|<span data-ttu-id="189b8-128">String</span><span class="sxs-lookup"><span data-stu-id="189b8-128">String</span></span>|<span data-ttu-id="189b8-129">ピボットテーブルの名前。</span><span class="sxs-lookup"><span data-stu-id="189b8-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="189b8-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="189b8-130">Relationships</span></span>
| <span data-ttu-id="189b8-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="189b8-131">Relationship</span></span> | <span data-ttu-id="189b8-132">型</span><span class="sxs-lookup"><span data-stu-id="189b8-132">Type</span></span>   |<span data-ttu-id="189b8-133">説明</span><span class="sxs-lookup"><span data-stu-id="189b8-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="189b8-134">ワークシート</span><span class="sxs-lookup"><span data-stu-id="189b8-134">worksheet</span></span>|[<span data-ttu-id="189b8-135">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="189b8-135">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="189b8-p103">現在のピボットテーブルを含んでいるワークシート。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="189b8-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="189b8-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="189b8-138">JSON representation</span></span>
<span data-ttu-id="189b8-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="189b8-139">Here is a JSON representation of the resource.</span></span>

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
