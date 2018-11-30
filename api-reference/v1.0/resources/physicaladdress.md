---
title: physicalAddress リソースの種類
description: 連絡先やイベントなどのリソースの番地を表します。
ms.openlocfilehash: eb2c1ea6a73d7f6eb5d3d43b877f50dc39a2b17e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022085"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="56736-103">physicalAddress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="56736-103">physicalAddress resource type</span></span>

<span data-ttu-id="56736-104">連絡先やイベントなどのリソースの番地を表します。</span><span class="sxs-lookup"><span data-stu-id="56736-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="56736-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56736-105">Properties</span></span>
| <span data-ttu-id="56736-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56736-106">Property</span></span>     | <span data-ttu-id="56736-107">型</span><span class="sxs-lookup"><span data-stu-id="56736-107">Type</span></span>   |<span data-ttu-id="56736-108">説明</span><span class="sxs-lookup"><span data-stu-id="56736-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56736-109">city</span><span class="sxs-lookup"><span data-stu-id="56736-109">city</span></span>|<span data-ttu-id="56736-110">String</span><span class="sxs-lookup"><span data-stu-id="56736-110">String</span></span>|<span data-ttu-id="56736-111">市区町村。</span><span class="sxs-lookup"><span data-stu-id="56736-111">The city.</span></span>|
|<span data-ttu-id="56736-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="56736-112">countryOrRegion</span></span>|<span data-ttu-id="56736-113">String</span><span class="sxs-lookup"><span data-stu-id="56736-113">String</span></span>|<span data-ttu-id="56736-p101">国または地域。自由形式の文字列値です。例: 「米国」。</span><span class="sxs-lookup"><span data-stu-id="56736-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="56736-116">postalCode</span><span class="sxs-lookup"><span data-stu-id="56736-116">postalCode</span></span>|<span data-ttu-id="56736-117">String</span><span class="sxs-lookup"><span data-stu-id="56736-117">String</span></span>|<span data-ttu-id="56736-118">郵便番号。</span><span class="sxs-lookup"><span data-stu-id="56736-118">The postal code.</span></span>|
|<span data-ttu-id="56736-119">state</span><span class="sxs-lookup"><span data-stu-id="56736-119">state</span></span>|<span data-ttu-id="56736-120">String</span><span class="sxs-lookup"><span data-stu-id="56736-120">String</span></span>|<span data-ttu-id="56736-121">都道府県。</span><span class="sxs-lookup"><span data-stu-id="56736-121">The state.</span></span>|
|<span data-ttu-id="56736-122">street</span><span class="sxs-lookup"><span data-stu-id="56736-122">street</span></span>|<span data-ttu-id="56736-123">String</span><span class="sxs-lookup"><span data-stu-id="56736-123">String</span></span>|<span data-ttu-id="56736-124">番地。</span><span class="sxs-lookup"><span data-stu-id="56736-124">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="56736-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="56736-125">JSON representation</span></span>

<span data-ttu-id="56736-126">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="56736-126">Here is a JSON representation of the resource</span></span>

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
