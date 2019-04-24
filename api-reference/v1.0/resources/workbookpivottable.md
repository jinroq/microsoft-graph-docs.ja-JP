---
title: ピボットテーブル リソースの種類
description: Excel のピボットテーブルを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5f6360ce1eacc313f1bcc8a9f59b44b216a87b84
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456865"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="a54d6-103">ピボットテーブル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a54d6-103">pivotTable resource type</span></span>

<span data-ttu-id="a54d6-104">Excel のピボットテーブルを表します。</span><span class="sxs-lookup"><span data-stu-id="a54d6-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="a54d6-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="a54d6-105">Methods</span></span>

| <span data-ttu-id="a54d6-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="a54d6-106">Method</span></span>           | <span data-ttu-id="a54d6-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a54d6-107">Return Type</span></span>    |<span data-ttu-id="a54d6-108">説明</span><span class="sxs-lookup"><span data-stu-id="a54d6-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a54d6-109">workbookPivotTable を取得する</span><span class="sxs-lookup"><span data-stu-id="a54d6-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="a54d6-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="a54d6-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="a54d6-111">worksheetprotection オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a54d6-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="a54d6-112">更新</span><span class="sxs-lookup"><span data-stu-id="a54d6-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="a54d6-113">None</span><span class="sxs-lookup"><span data-stu-id="a54d6-113">None</span></span>|<span data-ttu-id="a54d6-114">ピボットテーブルを更新します。</span><span class="sxs-lookup"><span data-stu-id="a54d6-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="a54d6-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="a54d6-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="a54d6-116">なし</span><span class="sxs-lookup"><span data-stu-id="a54d6-116">None</span></span>|<span data-ttu-id="a54d6-p101">指定したワークシート内のすべてのテーブルを更新します。このアクションは、ピボットテーブルのコレクションでのみ使用できることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="a54d6-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="a54d6-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a54d6-119">Properties</span></span>
| <span data-ttu-id="a54d6-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a54d6-120">Property</span></span>     | <span data-ttu-id="a54d6-121">型</span><span class="sxs-lookup"><span data-stu-id="a54d6-121">Type</span></span>   |<span data-ttu-id="a54d6-122">説明</span><span class="sxs-lookup"><span data-stu-id="a54d6-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a54d6-123">id</span><span class="sxs-lookup"><span data-stu-id="a54d6-123">id</span></span>|<span data-ttu-id="a54d6-124">String</span><span class="sxs-lookup"><span data-stu-id="a54d6-124">String</span></span>| <span data-ttu-id="a54d6-p102">ピボットテーブルの ID。 読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a54d6-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="a54d6-127">name</span><span class="sxs-lookup"><span data-stu-id="a54d6-127">name</span></span>|<span data-ttu-id="a54d6-128">String</span><span class="sxs-lookup"><span data-stu-id="a54d6-128">String</span></span>|<span data-ttu-id="a54d6-129">ピボットテーブルの名前。</span><span class="sxs-lookup"><span data-stu-id="a54d6-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="a54d6-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a54d6-130">Relationships</span></span>
| <span data-ttu-id="a54d6-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a54d6-131">Relationship</span></span> | <span data-ttu-id="a54d6-132">型</span><span class="sxs-lookup"><span data-stu-id="a54d6-132">Type</span></span>   |<span data-ttu-id="a54d6-133">説明</span><span class="sxs-lookup"><span data-stu-id="a54d6-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a54d6-134">worksheet</span><span class="sxs-lookup"><span data-stu-id="a54d6-134">worksheet</span></span>|[<span data-ttu-id="a54d6-135">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="a54d6-135">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="a54d6-136">現在のピボットテーブルを含んでいるワークシート。</span><span class="sxs-lookup"><span data-stu-id="a54d6-136">The worksheet containing the current PivotTable.</span></span> <span data-ttu-id="a54d6-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a54d6-137">Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="a54d6-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a54d6-138">JSON representation</span></span>
<span data-ttu-id="a54d6-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a54d6-139">Here is a JSON representation of the resource.</span></span>

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
