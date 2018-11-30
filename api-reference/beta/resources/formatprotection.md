---
title: FormatProtection リソースの種類
description: 範囲オブジェクトの書式保護を表します。
ms.openlocfilehash: 5f2a4968b018a952b24bb18a75a4f6d5aff55b00
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071077"
---
# <a name="formatprotection-resource-type"></a><span data-ttu-id="f437a-103">FormatProtection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f437a-103">FormatProtection resource type</span></span>

> <span data-ttu-id="f437a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f437a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f437a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f437a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f437a-106">範囲オブジェクトの書式保護を表します。</span><span class="sxs-lookup"><span data-stu-id="f437a-106">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="f437a-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="f437a-107">Methods</span></span>

| <span data-ttu-id="f437a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="f437a-108">Method</span></span>           | <span data-ttu-id="f437a-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f437a-109">Return Type</span></span>    |<span data-ttu-id="f437a-110">説明</span><span class="sxs-lookup"><span data-stu-id="f437a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f437a-111">FormatProtection を取得する</span><span class="sxs-lookup"><span data-stu-id="f437a-111">Get FormatProtection</span></span>](../api/formatprotection-get.md) | [<span data-ttu-id="f437a-112">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="f437a-112">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="f437a-113">formatProtection オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f437a-113">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="f437a-114">Update</span><span class="sxs-lookup"><span data-stu-id="f437a-114">Update</span></span>](../api/formatprotection-update.md) | [<span data-ttu-id="f437a-115">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="f437a-115">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="f437a-116">FormatProtection オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="f437a-116">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f437a-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f437a-117">Properties</span></span>
| <span data-ttu-id="f437a-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f437a-118">Property</span></span>     | <span data-ttu-id="f437a-119">型</span><span class="sxs-lookup"><span data-stu-id="f437a-119">Type</span></span>   |<span data-ttu-id="f437a-120">説明</span><span class="sxs-lookup"><span data-stu-id="f437a-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f437a-121">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="f437a-121">formulaHidden</span></span>|<span data-ttu-id="f437a-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="f437a-122">boolean</span></span>|<span data-ttu-id="f437a-p102">Excel が範囲内のセルの数式を非表示にするかどうかを示します。null 値は、範囲全体に一様な数式非表示設定がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="f437a-p102">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="f437a-125">locked</span><span class="sxs-lookup"><span data-stu-id="f437a-125">locked</span></span>|<span data-ttu-id="f437a-126">ブール値</span><span class="sxs-lookup"><span data-stu-id="f437a-126">boolean</span></span>|<span data-ttu-id="f437a-p103">Excel がオブジェクト内のセルをロックするかどうかを示します。null 値は、範囲全体に一様なロック設定がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="f437a-p103">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f437a-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f437a-129">Relationships</span></span>
<span data-ttu-id="f437a-130">なし</span><span class="sxs-lookup"><span data-stu-id="f437a-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f437a-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f437a-131">JSON representation</span></span>

<span data-ttu-id="f437a-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f437a-132">Here is a JSON representation of the resource.</span></span>

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