---
title: ピボットテーブル リソースの種類
description: Excel のピボットテーブルを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 91035b607d8c44f2d1515e9c004abd4c2235c0ec
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950859"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="0964b-103">ピボットテーブル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0964b-103">pivotTable resource type</span></span>

> <span data-ttu-id="0964b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0964b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0964b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0964b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0964b-106">Excel のピボットテーブルを表します。</span><span class="sxs-lookup"><span data-stu-id="0964b-106">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="0964b-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0964b-107">Methods</span></span>

| <span data-ttu-id="0964b-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0964b-108">Method</span></span>           | <span data-ttu-id="0964b-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0964b-109">Return Type</span></span>    |<span data-ttu-id="0964b-110">説明</span><span class="sxs-lookup"><span data-stu-id="0964b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0964b-111">workbookPivotTable を取得する</span><span class="sxs-lookup"><span data-stu-id="0964b-111">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="0964b-112">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="0964b-112">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="0964b-113">worksheetprotection オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0964b-113">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="0964b-114">更新</span><span class="sxs-lookup"><span data-stu-id="0964b-114">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="0964b-115">なし</span><span class="sxs-lookup"><span data-stu-id="0964b-115">None</span></span>|<span data-ttu-id="0964b-116">ピボットテーブルを更新します。</span><span class="sxs-lookup"><span data-stu-id="0964b-116">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="0964b-117">Refreshall</span><span class="sxs-lookup"><span data-stu-id="0964b-117">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="0964b-118">なし</span><span class="sxs-lookup"><span data-stu-id="0964b-118">None</span></span>|<span data-ttu-id="0964b-p102">指定したワークシート内のすべてのテーブルを更新します。このアクションは、ピボットテーブルのコレクションでのみ使用できることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="0964b-p102">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="0964b-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0964b-121">Properties</span></span>
| <span data-ttu-id="0964b-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0964b-122">Property</span></span>     | <span data-ttu-id="0964b-123">種類</span><span class="sxs-lookup"><span data-stu-id="0964b-123">Type</span></span>   |<span data-ttu-id="0964b-124">説明</span><span class="sxs-lookup"><span data-stu-id="0964b-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0964b-125">ID</span><span class="sxs-lookup"><span data-stu-id="0964b-125">id</span></span>|<span data-ttu-id="0964b-126">String</span><span class="sxs-lookup"><span data-stu-id="0964b-126">String</span></span>| <span data-ttu-id="0964b-p103">ピボットテーブルの ID。 読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0964b-p103">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="0964b-129">name</span><span class="sxs-lookup"><span data-stu-id="0964b-129">name</span></span>|<span data-ttu-id="0964b-130">String</span><span class="sxs-lookup"><span data-stu-id="0964b-130">String</span></span>|<span data-ttu-id="0964b-131">ピボットテーブルの名前。</span><span class="sxs-lookup"><span data-stu-id="0964b-131">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="0964b-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0964b-132">Relationships</span></span>
| <span data-ttu-id="0964b-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0964b-133">Relationship</span></span> | <span data-ttu-id="0964b-134">型</span><span class="sxs-lookup"><span data-stu-id="0964b-134">Type</span></span>   |<span data-ttu-id="0964b-135">説明</span><span class="sxs-lookup"><span data-stu-id="0964b-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0964b-136">ワークシート</span><span class="sxs-lookup"><span data-stu-id="0964b-136">worksheet</span></span>|[<span data-ttu-id="0964b-137">worksheet</span><span class="sxs-lookup"><span data-stu-id="0964b-137">worksheet</span></span>](worksheet.md)| <span data-ttu-id="0964b-p104">現在のピボットテーブルを含んでいるワークシート。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0964b-p104">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="0964b-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0964b-140">JSON representation</span></span>
<span data-ttu-id="0964b-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0964b-141">Here is a JSON representation of the resource.</span></span>

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
