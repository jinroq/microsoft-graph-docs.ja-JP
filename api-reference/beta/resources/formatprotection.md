---
title: FormatProtection リソースの種類
description: 範囲オブジェクトの書式保護を表します。
localization_priority: Normal
ms.openlocfilehash: 0b4add2e30a1e475adcb162903f771ce760f9285
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805622"
---
# <a name="formatprotection-resource-type"></a><span data-ttu-id="ecf65-103">FormatProtection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ecf65-103">FormatProtection resource type</span></span>

> <span data-ttu-id="ecf65-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ecf65-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ecf65-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ecf65-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ecf65-106">範囲オブジェクトの書式保護を表します。</span><span class="sxs-lookup"><span data-stu-id="ecf65-106">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="ecf65-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ecf65-107">Methods</span></span>

| <span data-ttu-id="ecf65-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ecf65-108">Method</span></span>           | <span data-ttu-id="ecf65-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ecf65-109">Return Type</span></span>    |<span data-ttu-id="ecf65-110">説明</span><span class="sxs-lookup"><span data-stu-id="ecf65-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ecf65-111">FormatProtection を取得する</span><span class="sxs-lookup"><span data-stu-id="ecf65-111">Get FormatProtection</span></span>](../api/formatprotection-get.md) | [<span data-ttu-id="ecf65-112">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="ecf65-112">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="ecf65-113">formatProtection オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ecf65-113">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="ecf65-114">Update</span><span class="sxs-lookup"><span data-stu-id="ecf65-114">Update</span></span>](../api/formatprotection-update.md) | [<span data-ttu-id="ecf65-115">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="ecf65-115">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="ecf65-116">FormatProtection オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="ecf65-116">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ecf65-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ecf65-117">Properties</span></span>
| <span data-ttu-id="ecf65-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ecf65-118">Property</span></span>     | <span data-ttu-id="ecf65-119">種類</span><span class="sxs-lookup"><span data-stu-id="ecf65-119">Type</span></span>   |<span data-ttu-id="ecf65-120">説明</span><span class="sxs-lookup"><span data-stu-id="ecf65-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ecf65-121">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="ecf65-121">formulaHidden</span></span>|<span data-ttu-id="ecf65-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="ecf65-122">boolean</span></span>|<span data-ttu-id="ecf65-p102">Excel が範囲内のセルの数式を非表示にするかどうかを示します。null 値は、範囲全体に一様な数式非表示設定がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="ecf65-p102">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="ecf65-125">locked</span><span class="sxs-lookup"><span data-stu-id="ecf65-125">locked</span></span>|<span data-ttu-id="ecf65-126">ブール値</span><span class="sxs-lookup"><span data-stu-id="ecf65-126">boolean</span></span>|<span data-ttu-id="ecf65-p103">Excel がオブジェクト内のセルをロックするかどうかを示します。null 値は、範囲全体に一様なロック設定がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="ecf65-p103">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ecf65-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ecf65-129">Relationships</span></span>
<span data-ttu-id="ecf65-130">なし</span><span class="sxs-lookup"><span data-stu-id="ecf65-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ecf65-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ecf65-131">JSON representation</span></span>

<span data-ttu-id="ecf65-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ecf65-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.formatProtection"
}-->

```json
{
  "formulaHidden": true,
  "locked": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FormatProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
