---
title: physicalAddress リソースの種類
description: 連絡先やイベントなどのリソースの番地を表します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: d6081f21069cef6014c8a028898f11ea9a3f4f3c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345005"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="41cfa-103">physicalAddress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="41cfa-103">physicalAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41cfa-104">連絡先やイベントなどのリソースの番地を表します。</span><span class="sxs-lookup"><span data-stu-id="41cfa-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="41cfa-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41cfa-105">Properties</span></span>
| <span data-ttu-id="41cfa-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41cfa-106">Property</span></span>     | <span data-ttu-id="41cfa-107">型</span><span class="sxs-lookup"><span data-stu-id="41cfa-107">Type</span></span>   |<span data-ttu-id="41cfa-108">説明</span><span class="sxs-lookup"><span data-stu-id="41cfa-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41cfa-109">city</span><span class="sxs-lookup"><span data-stu-id="41cfa-109">city</span></span>|<span data-ttu-id="41cfa-110">String</span><span class="sxs-lookup"><span data-stu-id="41cfa-110">String</span></span>|<span data-ttu-id="41cfa-111">市区町村。</span><span class="sxs-lookup"><span data-stu-id="41cfa-111">The city.</span></span>|
|<span data-ttu-id="41cfa-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="41cfa-112">countryOrRegion</span></span>|<span data-ttu-id="41cfa-113">String</span><span class="sxs-lookup"><span data-stu-id="41cfa-113">String</span></span>|<span data-ttu-id="41cfa-p101">国または地域。自由形式の文字列値です。例: 「米国」。</span><span class="sxs-lookup"><span data-stu-id="41cfa-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="41cfa-116">postalCode</span><span class="sxs-lookup"><span data-stu-id="41cfa-116">postalCode</span></span>|<span data-ttu-id="41cfa-117">String</span><span class="sxs-lookup"><span data-stu-id="41cfa-117">String</span></span>|<span data-ttu-id="41cfa-118">郵便番号。</span><span class="sxs-lookup"><span data-stu-id="41cfa-118">The postal code.</span></span>|
|<span data-ttu-id="41cfa-119">postofficebox が</span><span class="sxs-lookup"><span data-stu-id="41cfa-119">postOfficeBox</span></span>|<span data-ttu-id="41cfa-120">String</span><span class="sxs-lookup"><span data-stu-id="41cfa-120">String</span></span>|<span data-ttu-id="41cfa-121">郵便局の私書箱番号。</span><span class="sxs-lookup"><span data-stu-id="41cfa-121">The post office box number.</span></span>|
|<span data-ttu-id="41cfa-122">state</span><span class="sxs-lookup"><span data-stu-id="41cfa-122">state</span></span>|<span data-ttu-id="41cfa-123">String</span><span class="sxs-lookup"><span data-stu-id="41cfa-123">String</span></span>|<span data-ttu-id="41cfa-124">都道府県。</span><span class="sxs-lookup"><span data-stu-id="41cfa-124">The state.</span></span>|
|<span data-ttu-id="41cfa-125">street</span><span class="sxs-lookup"><span data-stu-id="41cfa-125">street</span></span>|<span data-ttu-id="41cfa-126">String</span><span class="sxs-lookup"><span data-stu-id="41cfa-126">String</span></span>|<span data-ttu-id="41cfa-127">番地。</span><span class="sxs-lookup"><span data-stu-id="41cfa-127">The street.</span></span>|
|<span data-ttu-id="41cfa-128">type</span><span class="sxs-lookup"><span data-stu-id="41cfa-128">type</span></span>|<span data-ttu-id="41cfa-129">physicalAddressType</span><span class="sxs-lookup"><span data-stu-id="41cfa-129">physicalAddressType</span></span>|<span data-ttu-id="41cfa-130">住所の種類。</span><span class="sxs-lookup"><span data-stu-id="41cfa-130">The type of address.</span></span> <span data-ttu-id="41cfa-131">使用可能な値は、`unknown`、`home`、`business`、`other` です。</span><span class="sxs-lookup"><span data-stu-id="41cfa-131">Possible values are: `unknown`, `home`, `business`, `other`.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="41cfa-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="41cfa-132">JSON representation</span></span>

<span data-ttu-id="41cfa-133">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="41cfa-133">Here is a JSON representation of the resource</span></span>

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
