---
title: physicalOfficeAddress リソースの種類
description: 連絡先、イベントなどのリソースの勤務先住所を表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 8299f72032cfb7910583fcd4dbefe914f054648e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966098"
---
# <a name="physicalofficeaddress-resource-type"></a><span data-ttu-id="0d275-103">physicalOfficeAddress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0d275-103">physicalOfficeAddress resource type</span></span>

<span data-ttu-id="0d275-104">組織の連絡先などのリソースの勤務先住所を表します。</span><span class="sxs-lookup"><span data-stu-id="0d275-104">Represents the business address of a resource such as an organizational contact.</span></span>

## <a name="properties"></a><span data-ttu-id="0d275-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d275-105">Properties</span></span>

| <span data-ttu-id="0d275-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d275-106">Property</span></span>     | <span data-ttu-id="0d275-107">型</span><span class="sxs-lookup"><span data-stu-id="0d275-107">Type</span></span>   |<span data-ttu-id="0d275-108">説明</span><span class="sxs-lookup"><span data-stu-id="0d275-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d275-109">city</span><span class="sxs-lookup"><span data-stu-id="0d275-109">city</span></span>|<span data-ttu-id="0d275-110">String</span><span class="sxs-lookup"><span data-stu-id="0d275-110">String</span></span>|<span data-ttu-id="0d275-111">市区町村。</span><span class="sxs-lookup"><span data-stu-id="0d275-111">The city.</span></span>|
|<span data-ttu-id="0d275-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="0d275-112">countryOrRegion</span></span>|<span data-ttu-id="0d275-113">String</span><span class="sxs-lookup"><span data-stu-id="0d275-113">String</span></span>|<span data-ttu-id="0d275-p101">国または地域。自由形式の文字列値です。例: 「米国」。</span><span class="sxs-lookup"><span data-stu-id="0d275-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="0d275-116">officeLocation</span><span class="sxs-lookup"><span data-stu-id="0d275-116">officeLocation</span></span>  | <span data-ttu-id="0d275-117">String</span><span class="sxs-lookup"><span data-stu-id="0d275-117">String</span></span> | <span data-ttu-id="0d275-118">組織の連絡先の建物やオフィス番号などのオフィスの場所。</span><span class="sxs-lookup"><span data-stu-id="0d275-118">Office location such as building and office number for an organizational contact.</span></span>  |
|<span data-ttu-id="0d275-119">postalCode</span><span class="sxs-lookup"><span data-stu-id="0d275-119">postalCode</span></span>|<span data-ttu-id="0d275-120">String</span><span class="sxs-lookup"><span data-stu-id="0d275-120">String</span></span>|<span data-ttu-id="0d275-121">郵便番号。</span><span class="sxs-lookup"><span data-stu-id="0d275-121">The postal code.</span></span>|
|<span data-ttu-id="0d275-122">state</span><span class="sxs-lookup"><span data-stu-id="0d275-122">state</span></span>|<span data-ttu-id="0d275-123">String</span><span class="sxs-lookup"><span data-stu-id="0d275-123">String</span></span>|<span data-ttu-id="0d275-124">都道府県。</span><span class="sxs-lookup"><span data-stu-id="0d275-124">The state.</span></span>|
|<span data-ttu-id="0d275-125">street</span><span class="sxs-lookup"><span data-stu-id="0d275-125">street</span></span>|<span data-ttu-id="0d275-126">String</span><span class="sxs-lookup"><span data-stu-id="0d275-126">String</span></span>|<span data-ttu-id="0d275-127">番地。</span><span class="sxs-lookup"><span data-stu-id="0d275-127">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0d275-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0d275-128">JSON representation</span></span>

<span data-ttu-id="0d275-129">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="0d275-129">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalOfficeAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "officeLocation": "string",
  "postalCode": "string",
  "state": "string",
  "street": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "physicalOfficeAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
