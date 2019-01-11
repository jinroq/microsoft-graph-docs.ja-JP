---
title: ピボットテーブル リソースの種類
description: Excel のピボットテーブルを表します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: aead84b21117b896f620a0722cf42c2e6c5d1293
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831543"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="421b4-103">ピボットテーブル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="421b4-103">pivotTable resource type</span></span>

> <span data-ttu-id="421b4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="421b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="421b4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="421b4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="421b4-106">Excel のピボットテーブルを表します。</span><span class="sxs-lookup"><span data-stu-id="421b4-106">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="421b4-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="421b4-107">Methods</span></span>

| <span data-ttu-id="421b4-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="421b4-108">Method</span></span>           | <span data-ttu-id="421b4-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="421b4-109">Return Type</span></span>    |<span data-ttu-id="421b4-110">説明</span><span class="sxs-lookup"><span data-stu-id="421b4-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="421b4-111">workbookPivotTable を取得する</span><span class="sxs-lookup"><span data-stu-id="421b4-111">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="421b4-112">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="421b4-112">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="421b4-113">worksheetprotection オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="421b4-113">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="421b4-114">更新</span><span class="sxs-lookup"><span data-stu-id="421b4-114">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="421b4-115">なし</span><span class="sxs-lookup"><span data-stu-id="421b4-115">None</span></span>|<span data-ttu-id="421b4-116">ピボットテーブルを更新します。</span><span class="sxs-lookup"><span data-stu-id="421b4-116">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="421b4-117">Refreshall</span><span class="sxs-lookup"><span data-stu-id="421b4-117">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="421b4-118">なし</span><span class="sxs-lookup"><span data-stu-id="421b4-118">None</span></span>|<span data-ttu-id="421b4-p102">指定したワークシート内のすべてのテーブルを更新します。このアクションは、ピボットテーブルのコレクションでのみ使用できることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="421b4-p102">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="421b4-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="421b4-121">Properties</span></span>
| <span data-ttu-id="421b4-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="421b4-122">Property</span></span>     | <span data-ttu-id="421b4-123">種類</span><span class="sxs-lookup"><span data-stu-id="421b4-123">Type</span></span>   |<span data-ttu-id="421b4-124">説明</span><span class="sxs-lookup"><span data-stu-id="421b4-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="421b4-125">ID</span><span class="sxs-lookup"><span data-stu-id="421b4-125">id</span></span>|<span data-ttu-id="421b4-126">String</span><span class="sxs-lookup"><span data-stu-id="421b4-126">String</span></span>| <span data-ttu-id="421b4-p103">ピボットテーブルの ID。 読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="421b4-p103">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="421b4-129">name</span><span class="sxs-lookup"><span data-stu-id="421b4-129">name</span></span>|<span data-ttu-id="421b4-130">String</span><span class="sxs-lookup"><span data-stu-id="421b4-130">String</span></span>|<span data-ttu-id="421b4-131">ピボットテーブルの名前。</span><span class="sxs-lookup"><span data-stu-id="421b4-131">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="421b4-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="421b4-132">Relationships</span></span>
| <span data-ttu-id="421b4-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="421b4-133">Relationship</span></span> | <span data-ttu-id="421b4-134">型</span><span class="sxs-lookup"><span data-stu-id="421b4-134">Type</span></span>   |<span data-ttu-id="421b4-135">説明</span><span class="sxs-lookup"><span data-stu-id="421b4-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="421b4-136">ワークシート</span><span class="sxs-lookup"><span data-stu-id="421b4-136">worksheet</span></span>|[<span data-ttu-id="421b4-137">worksheet</span><span class="sxs-lookup"><span data-stu-id="421b4-137">worksheet</span></span>](worksheet.md)| <span data-ttu-id="421b4-p104">現在のピボットテーブルを含んでいるワークシート。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="421b4-p104">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="421b4-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="421b4-140">JSON representation</span></span>
<span data-ttu-id="421b4-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="421b4-141">Here is a JSON representation of the resource.</span></span>

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
