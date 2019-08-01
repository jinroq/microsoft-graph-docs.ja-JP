---
title: FormatProtection リソースの種類
description: 範囲オブジェクトの書式保護を表します。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: babd1192e216179c59b40d78175f24b0e8366d71
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032439"
---
# <a name="formatprotection-resource-type"></a><span data-ttu-id="deb02-103">FormatProtection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="deb02-103">FormatProtection resource type</span></span>

<span data-ttu-id="deb02-104">範囲オブジェクトの書式保護を表します。</span><span class="sxs-lookup"><span data-stu-id="deb02-104">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="deb02-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="deb02-105">Methods</span></span>

| <span data-ttu-id="deb02-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="deb02-106">Method</span></span>           | <span data-ttu-id="deb02-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="deb02-107">Return Type</span></span>    |<span data-ttu-id="deb02-108">説明</span><span class="sxs-lookup"><span data-stu-id="deb02-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="deb02-109">FormatProtection を取得する</span><span class="sxs-lookup"><span data-stu-id="deb02-109">Get FormatProtection</span></span>](../api/formatprotection-get.md) | [<span data-ttu-id="deb02-110">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="deb02-110">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="deb02-111">formatProtection オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="deb02-111">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="deb02-112">Update</span><span class="sxs-lookup"><span data-stu-id="deb02-112">Update</span></span>](../api/formatprotection-update.md) | [<span data-ttu-id="deb02-113">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="deb02-113">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="deb02-114">FormatProtection オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="deb02-114">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="deb02-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="deb02-115">Properties</span></span>
| <span data-ttu-id="deb02-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="deb02-116">Property</span></span>     | <span data-ttu-id="deb02-117">型</span><span class="sxs-lookup"><span data-stu-id="deb02-117">Type</span></span>   |<span data-ttu-id="deb02-118">説明</span><span class="sxs-lookup"><span data-stu-id="deb02-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="deb02-119">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="deb02-119">formulaHidden</span></span>|<span data-ttu-id="deb02-120">boolean</span><span class="sxs-lookup"><span data-stu-id="deb02-120">boolean</span></span>|<span data-ttu-id="deb02-p101">Excel が範囲内のセルの数式を非表示にするかどうかを示します。null 値は、範囲全体に一様な数式非表示設定がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="deb02-p101">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="deb02-123">locked</span><span class="sxs-lookup"><span data-stu-id="deb02-123">locked</span></span>|<span data-ttu-id="deb02-124">ブール値</span><span class="sxs-lookup"><span data-stu-id="deb02-124">boolean</span></span>|<span data-ttu-id="deb02-p102">Excel がオブジェクト内のセルをロックするかどうかを示します。null 値は、範囲全体に一様なロック設定がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="deb02-p102">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="deb02-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="deb02-127">Relationships</span></span>
<span data-ttu-id="deb02-128">なし</span><span class="sxs-lookup"><span data-stu-id="deb02-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="deb02-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="deb02-129">JSON representation</span></span>

<span data-ttu-id="deb02-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="deb02-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFormatProtection"
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
