---
title: physicalAddress リソースの種類
description: 連絡先やイベントなどのリソースの番地を表します。
ms.openlocfilehash: 819240be3eb9a088fde43390fbb1d1d4af1fd30c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073075"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="2a911-103">physicalAddress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2a911-103">physicalAddress resource type</span></span>

<span data-ttu-id="2a911-104">連絡先やイベントなどのリソースの番地を表します。</span><span class="sxs-lookup"><span data-stu-id="2a911-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="2a911-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2a911-105">Properties</span></span>
| <span data-ttu-id="2a911-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2a911-106">Property</span></span>     | <span data-ttu-id="2a911-107">型</span><span class="sxs-lookup"><span data-stu-id="2a911-107">Type</span></span>   |<span data-ttu-id="2a911-108">説明</span><span class="sxs-lookup"><span data-stu-id="2a911-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a911-109">type</span><span class="sxs-lookup"><span data-stu-id="2a911-109">type</span></span>|<span data-ttu-id="2a911-110">String</span><span class="sxs-lookup"><span data-stu-id="2a911-110">String</span></span>|<span data-ttu-id="2a911-111">アドレスの種類。</span><span class="sxs-lookup"><span data-stu-id="2a911-111">The type of address.</span></span> <span data-ttu-id="2a911-112">可能な値は、`unknown`、`home`、`business`、`other` です。</span><span class="sxs-lookup"><span data-stu-id="2a911-112">Possible values are: `unknown`, `home`, `business`, `other`.</span></span>|
|<span data-ttu-id="2a911-113">postOfficeBox</span><span class="sxs-lookup"><span data-stu-id="2a911-113">postOfficeBox</span></span>|<span data-ttu-id="2a911-114">String</span><span class="sxs-lookup"><span data-stu-id="2a911-114">String</span></span>|<span data-ttu-id="2a911-115">私書箱番号です。</span><span class="sxs-lookup"><span data-stu-id="2a911-115">The post office box number.</span></span>|
|<span data-ttu-id="2a911-116">city</span><span class="sxs-lookup"><span data-stu-id="2a911-116">city</span></span>|<span data-ttu-id="2a911-117">String</span><span class="sxs-lookup"><span data-stu-id="2a911-117">String</span></span>|<span data-ttu-id="2a911-118">市区町村。</span><span class="sxs-lookup"><span data-stu-id="2a911-118">The city.</span></span>|
|<span data-ttu-id="2a911-119">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="2a911-119">countryOrRegion</span></span>|<span data-ttu-id="2a911-120">String</span><span class="sxs-lookup"><span data-stu-id="2a911-120">String</span></span>|<span data-ttu-id="2a911-p102">国または地域。自由形式の文字列値です。例: 「米国」。</span><span class="sxs-lookup"><span data-stu-id="2a911-p102">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="2a911-123">postalCode</span><span class="sxs-lookup"><span data-stu-id="2a911-123">postalCode</span></span>|<span data-ttu-id="2a911-124">String</span><span class="sxs-lookup"><span data-stu-id="2a911-124">String</span></span>|<span data-ttu-id="2a911-125">郵便番号。</span><span class="sxs-lookup"><span data-stu-id="2a911-125">The postal code.</span></span>|
|<span data-ttu-id="2a911-126">state</span><span class="sxs-lookup"><span data-stu-id="2a911-126">state</span></span>|<span data-ttu-id="2a911-127">String</span><span class="sxs-lookup"><span data-stu-id="2a911-127">String</span></span>|<span data-ttu-id="2a911-128">都道府県。</span><span class="sxs-lookup"><span data-stu-id="2a911-128">The state.</span></span>|
|<span data-ttu-id="2a911-129">street</span><span class="sxs-lookup"><span data-stu-id="2a911-129">street</span></span>|<span data-ttu-id="2a911-130">String</span><span class="sxs-lookup"><span data-stu-id="2a911-130">String</span></span>|<span data-ttu-id="2a911-131">番地。</span><span class="sxs-lookup"><span data-stu-id="2a911-131">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2a911-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2a911-132">JSON representation</span></span>

<span data-ttu-id="2a911-133">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="2a911-133">Here is a JSON representation of the resource</span></span>

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
