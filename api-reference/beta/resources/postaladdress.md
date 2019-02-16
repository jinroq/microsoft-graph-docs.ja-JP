---
title: "\"postaladdress リソースの種類"
description: 連絡先やイベントなどのリソースの番地を表します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7d168e4f53dbd182e4dbd93d0a5b6342daf3339d
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057395"
---
# <a name="postaladdress-resource-type"></a><span data-ttu-id="56e4c-103">"postaladdress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="56e4c-103">postalAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56e4c-104">場所の住所を表します。</span><span class="sxs-lookup"><span data-stu-id="56e4c-104">Represents the street address of a location.</span></span>


## <a name="properties"></a><span data-ttu-id="56e4c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56e4c-105">Properties</span></span>
| <span data-ttu-id="56e4c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56e4c-106">Property</span></span>     | <span data-ttu-id="56e4c-107">型</span><span class="sxs-lookup"><span data-stu-id="56e4c-107">Type</span></span>   |<span data-ttu-id="56e4c-108">説明</span><span class="sxs-lookup"><span data-stu-id="56e4c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56e4c-109">city</span><span class="sxs-lookup"><span data-stu-id="56e4c-109">city</span></span>|<span data-ttu-id="56e4c-110">String</span><span class="sxs-lookup"><span data-stu-id="56e4c-110">String</span></span>|<span data-ttu-id="56e4c-111">市区町村。</span><span class="sxs-lookup"><span data-stu-id="56e4c-111">The city.</span></span>|
|<span data-ttu-id="56e4c-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="56e4c-112">countryOrRegion</span></span>|<span data-ttu-id="56e4c-113">String</span><span class="sxs-lookup"><span data-stu-id="56e4c-113">String</span></span>|<span data-ttu-id="56e4c-p101">国または地域。自由形式の文字列値です。例: 「米国」。</span><span class="sxs-lookup"><span data-stu-id="56e4c-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="56e4c-116">isinferred</span><span class="sxs-lookup"><span data-stu-id="56e4c-116">isInferred</span></span>|<span data-ttu-id="56e4c-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="56e4c-117">Boolean</span></span>|<span data-ttu-id="56e4c-118">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="56e4c-118">For internal use only.</span></span>|
|<span data-ttu-id="56e4c-119">postalCode</span><span class="sxs-lookup"><span data-stu-id="56e4c-119">postalCode</span></span>|<span data-ttu-id="56e4c-120">String</span><span class="sxs-lookup"><span data-stu-id="56e4c-120">String</span></span>|<span data-ttu-id="56e4c-121">郵便番号。</span><span class="sxs-lookup"><span data-stu-id="56e4c-121">The postal code.</span></span>|
|<span data-ttu-id="56e4c-122">state</span><span class="sxs-lookup"><span data-stu-id="56e4c-122">state</span></span>|<span data-ttu-id="56e4c-123">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="56e4c-123">String</span></span>|<span data-ttu-id="56e4c-124">都道府県。</span><span class="sxs-lookup"><span data-stu-id="56e4c-124">The state.</span></span>|
|<span data-ttu-id="56e4c-125">street</span><span class="sxs-lookup"><span data-stu-id="56e4c-125">street</span></span>|<span data-ttu-id="56e4c-126">String</span><span class="sxs-lookup"><span data-stu-id="56e4c-126">String</span></span>|<span data-ttu-id="56e4c-127">番地。</span><span class="sxs-lookup"><span data-stu-id="56e4c-127">The street.</span></span>|
|<span data-ttu-id="56e4c-128">type</span><span class="sxs-lookup"><span data-stu-id="56e4c-128">type</span></span>|<span data-ttu-id="56e4c-129">addressType</span><span class="sxs-lookup"><span data-stu-id="56e4c-129">addressType</span></span>|<span data-ttu-id="56e4c-130">住所の種類。</span><span class="sxs-lookup"><span data-stu-id="56e4c-130">The type of address.</span></span> <span data-ttu-id="56e4c-131">使用可能な値は`unknown`、 `home`、 `business`、 `other`、です。</span><span class="sxs-lookup"><span data-stu-id="56e4c-131">The possible values are: `unknown`, `home`, `business`, `other`.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="56e4c-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="56e4c-132">JSON representation</span></span>

<span data-ttu-id="56e4c-133">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="56e4c-133">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.postalAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "isInferred": "boolean",
  "postalCode": "string",
  "state": "string",
  "street": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "postaladdress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/postaladdress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}-->
