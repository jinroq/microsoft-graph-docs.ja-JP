---
title: physicalAddress リソースの種類
description: 連絡先やイベントなどのリソースの番地を表します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 35826dabd9052023abdc9d8c83ac9640ef550061
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966120"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="70a8f-103">physicalAddress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="70a8f-103">physicalAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70a8f-104">連絡先やイベントなどのリソースの番地を表します。</span><span class="sxs-lookup"><span data-stu-id="70a8f-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="70a8f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="70a8f-105">Properties</span></span>
| <span data-ttu-id="70a8f-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="70a8f-106">Property</span></span>     | <span data-ttu-id="70a8f-107">型</span><span class="sxs-lookup"><span data-stu-id="70a8f-107">Type</span></span>   |<span data-ttu-id="70a8f-108">説明</span><span class="sxs-lookup"><span data-stu-id="70a8f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70a8f-109">city</span><span class="sxs-lookup"><span data-stu-id="70a8f-109">city</span></span>|<span data-ttu-id="70a8f-110">String</span><span class="sxs-lookup"><span data-stu-id="70a8f-110">String</span></span>|<span data-ttu-id="70a8f-111">市区町村。</span><span class="sxs-lookup"><span data-stu-id="70a8f-111">The city.</span></span>|
|<span data-ttu-id="70a8f-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="70a8f-112">countryOrRegion</span></span>|<span data-ttu-id="70a8f-113">String</span><span class="sxs-lookup"><span data-stu-id="70a8f-113">String</span></span>|<span data-ttu-id="70a8f-p101">国または地域。自由形式の文字列値です。例: 「米国」。</span><span class="sxs-lookup"><span data-stu-id="70a8f-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="70a8f-116">postalCode</span><span class="sxs-lookup"><span data-stu-id="70a8f-116">postalCode</span></span>|<span data-ttu-id="70a8f-117">String</span><span class="sxs-lookup"><span data-stu-id="70a8f-117">String</span></span>|<span data-ttu-id="70a8f-118">郵便番号。</span><span class="sxs-lookup"><span data-stu-id="70a8f-118">The postal code.</span></span>|
|<span data-ttu-id="70a8f-119">Postofficebox が</span><span class="sxs-lookup"><span data-stu-id="70a8f-119">postOfficeBox</span></span>|<span data-ttu-id="70a8f-120">String</span><span class="sxs-lookup"><span data-stu-id="70a8f-120">String</span></span>|<span data-ttu-id="70a8f-121">郵便局の私書箱番号。</span><span class="sxs-lookup"><span data-stu-id="70a8f-121">The post office box number.</span></span>|
|<span data-ttu-id="70a8f-122">state</span><span class="sxs-lookup"><span data-stu-id="70a8f-122">state</span></span>|<span data-ttu-id="70a8f-123">String</span><span class="sxs-lookup"><span data-stu-id="70a8f-123">String</span></span>|<span data-ttu-id="70a8f-124">都道府県。</span><span class="sxs-lookup"><span data-stu-id="70a8f-124">The state.</span></span>|
|<span data-ttu-id="70a8f-125">street</span><span class="sxs-lookup"><span data-stu-id="70a8f-125">street</span></span>|<span data-ttu-id="70a8f-126">String</span><span class="sxs-lookup"><span data-stu-id="70a8f-126">String</span></span>|<span data-ttu-id="70a8f-127">番地。</span><span class="sxs-lookup"><span data-stu-id="70a8f-127">The street.</span></span>|
|<span data-ttu-id="70a8f-128">type</span><span class="sxs-lookup"><span data-stu-id="70a8f-128">type</span></span>|<span data-ttu-id="70a8f-129">physicalAddressType</span><span class="sxs-lookup"><span data-stu-id="70a8f-129">physicalAddressType</span></span>|<span data-ttu-id="70a8f-130">住所の種類。</span><span class="sxs-lookup"><span data-stu-id="70a8f-130">The type of address.</span></span> <span data-ttu-id="70a8f-131">使用可能な値は、`unknown`、`home`、`business`、`other` です。</span><span class="sxs-lookup"><span data-stu-id="70a8f-131">Possible values are: `unknown`, `home`, `business`, `other`.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="70a8f-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="70a8f-132">JSON representation</span></span>

<span data-ttu-id="70a8f-133">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="70a8f-133">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "postalCode": "string",
  "postOfficeBox": "string",
  "state": "string",
  "street": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "physicalAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
