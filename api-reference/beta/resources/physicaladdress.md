---
title: physicalAddress リソースの種類
description: 連絡先やイベントなどのリソースの番地を表します。
localization_priority: Normal
ms.openlocfilehash: 3a656046cc23394fc8cff9100eb5ad2289050b25
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823584"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="d206f-103">physicalAddress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d206f-103">physicalAddress resource type</span></span>

<span data-ttu-id="d206f-104">連絡先やイベントなどのリソースの番地を表します。</span><span class="sxs-lookup"><span data-stu-id="d206f-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="d206f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d206f-105">Properties</span></span>
| <span data-ttu-id="d206f-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d206f-106">Property</span></span>     | <span data-ttu-id="d206f-107">種類</span><span class="sxs-lookup"><span data-stu-id="d206f-107">Type</span></span>   |<span data-ttu-id="d206f-108">説明</span><span class="sxs-lookup"><span data-stu-id="d206f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d206f-109">type</span><span class="sxs-lookup"><span data-stu-id="d206f-109">type</span></span>|<span data-ttu-id="d206f-110">String</span><span class="sxs-lookup"><span data-stu-id="d206f-110">String</span></span>|<span data-ttu-id="d206f-111">アドレスの種類。</span><span class="sxs-lookup"><span data-stu-id="d206f-111">The type of address.</span></span> <span data-ttu-id="d206f-112">可能な値は、`unknown`、`home`、`business`、`other` です。</span><span class="sxs-lookup"><span data-stu-id="d206f-112">Possible values are: `unknown`, `home`, `business`, `other`.</span></span>|
|<span data-ttu-id="d206f-113">postOfficeBox</span><span class="sxs-lookup"><span data-stu-id="d206f-113">postOfficeBox</span></span>|<span data-ttu-id="d206f-114">String</span><span class="sxs-lookup"><span data-stu-id="d206f-114">String</span></span>|<span data-ttu-id="d206f-115">私書箱番号です。</span><span class="sxs-lookup"><span data-stu-id="d206f-115">The post office box number.</span></span>|
|<span data-ttu-id="d206f-116">city</span><span class="sxs-lookup"><span data-stu-id="d206f-116">city</span></span>|<span data-ttu-id="d206f-117">String</span><span class="sxs-lookup"><span data-stu-id="d206f-117">String</span></span>|<span data-ttu-id="d206f-118">市区町村。</span><span class="sxs-lookup"><span data-stu-id="d206f-118">The city.</span></span>|
|<span data-ttu-id="d206f-119">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="d206f-119">countryOrRegion</span></span>|<span data-ttu-id="d206f-120">String</span><span class="sxs-lookup"><span data-stu-id="d206f-120">String</span></span>|<span data-ttu-id="d206f-p102">国または地域。自由形式の文字列値です。例: 「米国」。</span><span class="sxs-lookup"><span data-stu-id="d206f-p102">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="d206f-123">postalCode</span><span class="sxs-lookup"><span data-stu-id="d206f-123">postalCode</span></span>|<span data-ttu-id="d206f-124">String</span><span class="sxs-lookup"><span data-stu-id="d206f-124">String</span></span>|<span data-ttu-id="d206f-125">郵便番号。</span><span class="sxs-lookup"><span data-stu-id="d206f-125">The postal code.</span></span>|
|<span data-ttu-id="d206f-126">state</span><span class="sxs-lookup"><span data-stu-id="d206f-126">state</span></span>|<span data-ttu-id="d206f-127">String</span><span class="sxs-lookup"><span data-stu-id="d206f-127">String</span></span>|<span data-ttu-id="d206f-128">都道府県。</span><span class="sxs-lookup"><span data-stu-id="d206f-128">The state.</span></span>|
|<span data-ttu-id="d206f-129">street</span><span class="sxs-lookup"><span data-stu-id="d206f-129">street</span></span>|<span data-ttu-id="d206f-130">String</span><span class="sxs-lookup"><span data-stu-id="d206f-130">String</span></span>|<span data-ttu-id="d206f-131">番地。</span><span class="sxs-lookup"><span data-stu-id="d206f-131">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d206f-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d206f-132">JSON representation</span></span>

<span data-ttu-id="d206f-133">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="d206f-133">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalAddress"
}-->

```json
{
  "type": "string",
  "postOfficeBox": "string",
  "city": "string",
  "countryOrRegion": "string",
  "postalCode": "string",
  "state": "string",
  "street": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "physicalAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
