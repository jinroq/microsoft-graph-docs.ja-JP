---
title: physicalAddress リソースの種類
description: 連絡先やイベントなどのリソースの番地を表します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: eb7bf1ee21a40517704f20176f5fbcf9ea2b276a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573782"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="c8559-103">physicalAddress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c8559-103">physicalAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8559-104">連絡先やイベントなどのリソースの番地を表します。</span><span class="sxs-lookup"><span data-stu-id="c8559-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="c8559-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8559-105">Properties</span></span>
| <span data-ttu-id="c8559-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8559-106">Property</span></span>     | <span data-ttu-id="c8559-107">型</span><span class="sxs-lookup"><span data-stu-id="c8559-107">Type</span></span>   |<span data-ttu-id="c8559-108">説明</span><span class="sxs-lookup"><span data-stu-id="c8559-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8559-109">city</span><span class="sxs-lookup"><span data-stu-id="c8559-109">city</span></span>|<span data-ttu-id="c8559-110">String</span><span class="sxs-lookup"><span data-stu-id="c8559-110">String</span></span>|<span data-ttu-id="c8559-111">市区町村。</span><span class="sxs-lookup"><span data-stu-id="c8559-111">The city.</span></span>|
|<span data-ttu-id="c8559-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="c8559-112">countryOrRegion</span></span>|<span data-ttu-id="c8559-113">String</span><span class="sxs-lookup"><span data-stu-id="c8559-113">String</span></span>|<span data-ttu-id="c8559-p101">国または地域。自由形式の文字列値です。例: 「米国」。</span><span class="sxs-lookup"><span data-stu-id="c8559-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="c8559-116">postalCode</span><span class="sxs-lookup"><span data-stu-id="c8559-116">postalCode</span></span>|<span data-ttu-id="c8559-117">String</span><span class="sxs-lookup"><span data-stu-id="c8559-117">String</span></span>|<span data-ttu-id="c8559-118">郵便番号。</span><span class="sxs-lookup"><span data-stu-id="c8559-118">The postal code.</span></span>|
|<span data-ttu-id="c8559-119">postofficebox が</span><span class="sxs-lookup"><span data-stu-id="c8559-119">postOfficeBox</span></span>|<span data-ttu-id="c8559-120">String</span><span class="sxs-lookup"><span data-stu-id="c8559-120">String</span></span>|<span data-ttu-id="c8559-121">郵便局の私書箱番号。</span><span class="sxs-lookup"><span data-stu-id="c8559-121">The post office box number.</span></span>|
|<span data-ttu-id="c8559-122">state</span><span class="sxs-lookup"><span data-stu-id="c8559-122">state</span></span>|<span data-ttu-id="c8559-123">String</span><span class="sxs-lookup"><span data-stu-id="c8559-123">String</span></span>|<span data-ttu-id="c8559-124">都道府県。</span><span class="sxs-lookup"><span data-stu-id="c8559-124">The state.</span></span>|
|<span data-ttu-id="c8559-125">street</span><span class="sxs-lookup"><span data-stu-id="c8559-125">street</span></span>|<span data-ttu-id="c8559-126">String</span><span class="sxs-lookup"><span data-stu-id="c8559-126">String</span></span>|<span data-ttu-id="c8559-127">番地。</span><span class="sxs-lookup"><span data-stu-id="c8559-127">The street.</span></span>|
|<span data-ttu-id="c8559-128">type</span><span class="sxs-lookup"><span data-stu-id="c8559-128">type</span></span>|<span data-ttu-id="c8559-129">physicalAddressType</span><span class="sxs-lookup"><span data-stu-id="c8559-129">physicalAddressType</span></span>|<span data-ttu-id="c8559-130">住所の種類。</span><span class="sxs-lookup"><span data-stu-id="c8559-130">The type of address.</span></span> <span data-ttu-id="c8559-131">使用可能な値は、`unknown`、`home`、`business`、`other` です。</span><span class="sxs-lookup"><span data-stu-id="c8559-131">Possible values are: `unknown`, `home`, `business`, `other`.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c8559-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c8559-132">JSON representation</span></span>

<span data-ttu-id="c8559-133">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="c8559-133">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "physicalAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/physicaladdress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}-->
