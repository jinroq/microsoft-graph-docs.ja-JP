---
title: FormatProtection リソースの種類
description: 範囲オブジェクトの書式保護を表します。
localization_priority: Normal
ms.openlocfilehash: 7bc27060567136386ef1f08e6fe46e95980788a9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509190"
---
# <a name="formatprotection-resource-type"></a><span data-ttu-id="4504b-103">FormatProtection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4504b-103">FormatProtection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4504b-104">範囲オブジェクトの書式保護を表します。</span><span class="sxs-lookup"><span data-stu-id="4504b-104">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="4504b-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="4504b-105">Methods</span></span>

| <span data-ttu-id="4504b-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="4504b-106">Method</span></span>           | <span data-ttu-id="4504b-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4504b-107">Return Type</span></span>    |<span data-ttu-id="4504b-108">説明</span><span class="sxs-lookup"><span data-stu-id="4504b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4504b-109">FormatProtection を取得する</span><span class="sxs-lookup"><span data-stu-id="4504b-109">[Get FormatProtection](../api/formatprotection-get.md)</span></span> | [<span data-ttu-id="4504b-110">formatProtection</span><span class="sxs-lookup"><span data-stu-id="4504b-110">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="4504b-111">formatProtection オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4504b-111">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="4504b-112">Update</span><span class="sxs-lookup"><span data-stu-id="4504b-112">Update</span></span>](../api/formatprotection-update.md) | <span data-ttu-id="4504b-113">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="4504b-113">[FormatProtection](formatprotection.md)</span></span>  |<span data-ttu-id="4504b-114">FormatProtection オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="4504b-114">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4504b-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4504b-115">Properties</span></span>
| <span data-ttu-id="4504b-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4504b-116">Property</span></span>     | <span data-ttu-id="4504b-117">型</span><span class="sxs-lookup"><span data-stu-id="4504b-117">Type</span></span>   |<span data-ttu-id="4504b-118">説明</span><span class="sxs-lookup"><span data-stu-id="4504b-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4504b-119">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="4504b-119">formulaHidden</span></span>|<span data-ttu-id="4504b-120">boolean</span><span class="sxs-lookup"><span data-stu-id="4504b-120">boolean</span></span>|<span data-ttu-id="4504b-p101">Excel が範囲内のセルの数式を非表示にするかどうかを示します。null 値は、範囲全体に一様な数式非表示設定がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="4504b-p101">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="4504b-123">locked</span><span class="sxs-lookup"><span data-stu-id="4504b-123">locked</span></span>|<span data-ttu-id="4504b-124">ブール値</span><span class="sxs-lookup"><span data-stu-id="4504b-124">boolean</span></span>|<span data-ttu-id="4504b-p102">Excel がオブジェクト内のセルをロックするかどうかを示します。null 値は、範囲全体に一様なロック設定がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="4504b-p102">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4504b-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4504b-127">Relationships</span></span>
<span data-ttu-id="4504b-128">なし</span><span class="sxs-lookup"><span data-stu-id="4504b-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4504b-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4504b-129">JSON representation</span></span>

<span data-ttu-id="4504b-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4504b-130">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "FormatProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/formatprotection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
