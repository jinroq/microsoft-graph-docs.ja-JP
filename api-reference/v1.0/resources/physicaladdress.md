---
title: physicalAddress リソースの種類
description: 連絡先やイベントなどのリソースの番地を表します。
localization_priority: Normal
ms.openlocfilehash: 2bbfc3f38d4d353d370b9c8ba859b06cc2e4398b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462467"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="cb8cc-103">physicalAddress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cb8cc-103">physicalAddress resource type</span></span>

<span data-ttu-id="cb8cc-104">連絡先やイベントなどのリソースの番地を表します。</span><span class="sxs-lookup"><span data-stu-id="cb8cc-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="cb8cc-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb8cc-105">Properties</span></span>
| <span data-ttu-id="cb8cc-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb8cc-106">Property</span></span>     | <span data-ttu-id="cb8cc-107">型</span><span class="sxs-lookup"><span data-stu-id="cb8cc-107">Type</span></span>   |<span data-ttu-id="cb8cc-108">説明</span><span class="sxs-lookup"><span data-stu-id="cb8cc-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb8cc-109">city</span><span class="sxs-lookup"><span data-stu-id="cb8cc-109">city</span></span>|<span data-ttu-id="cb8cc-110">String</span><span class="sxs-lookup"><span data-stu-id="cb8cc-110">String</span></span>|<span data-ttu-id="cb8cc-111">市区町村。</span><span class="sxs-lookup"><span data-stu-id="cb8cc-111">The city.</span></span>|
|<span data-ttu-id="cb8cc-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="cb8cc-112">countryOrRegion</span></span>|<span data-ttu-id="cb8cc-113">String</span><span class="sxs-lookup"><span data-stu-id="cb8cc-113">String</span></span>|<span data-ttu-id="cb8cc-p101">国または地域。自由形式の文字列値です。例: 「米国」。</span><span class="sxs-lookup"><span data-stu-id="cb8cc-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="cb8cc-116">postalCode</span><span class="sxs-lookup"><span data-stu-id="cb8cc-116">postalCode</span></span>|<span data-ttu-id="cb8cc-117">String</span><span class="sxs-lookup"><span data-stu-id="cb8cc-117">String</span></span>|<span data-ttu-id="cb8cc-118">郵便番号。</span><span class="sxs-lookup"><span data-stu-id="cb8cc-118">The postal code.</span></span>|
|<span data-ttu-id="cb8cc-119">state</span><span class="sxs-lookup"><span data-stu-id="cb8cc-119">state</span></span>|<span data-ttu-id="cb8cc-120">String</span><span class="sxs-lookup"><span data-stu-id="cb8cc-120">String</span></span>|<span data-ttu-id="cb8cc-121">都道府県。</span><span class="sxs-lookup"><span data-stu-id="cb8cc-121">The state.</span></span>|
|<span data-ttu-id="cb8cc-122">street</span><span class="sxs-lookup"><span data-stu-id="cb8cc-122">street</span></span>|<span data-ttu-id="cb8cc-123">String</span><span class="sxs-lookup"><span data-stu-id="cb8cc-123">String</span></span>|<span data-ttu-id="cb8cc-124">番地。</span><span class="sxs-lookup"><span data-stu-id="cb8cc-124">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb8cc-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cb8cc-125">JSON representation</span></span>

<span data-ttu-id="cb8cc-126">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="cb8cc-126">Here is a JSON representation of the resource</span></span>

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
