---
title: physicalOfficeAddress リソースの種類
description: 連絡先やイベントなどのリソースの会社の住所を表します。
ms.openlocfilehash: 472e4dfd03670f5fd4ff6b5c5c53342fff5c391a
ms.sourcegitcommit: f3d479edf03935d0edbbc7668a65f7cde2a56c92
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2018
ms.locfileid: "27284099"
---
# <a name="physicalofficeaddress-resource-type"></a><span data-ttu-id="0a7b7-103">physicalOfficeAddress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0a7b7-103">physicalOfficeAddress resource type</span></span>

<span data-ttu-id="0a7b7-104">リソース、組織の連絡先などの会社の住所を表します。</span><span class="sxs-lookup"><span data-stu-id="0a7b7-104">Represents the business address of a resource such as an organizational contact.</span></span>

## <a name="properties"></a><span data-ttu-id="0a7b7-105">Properties</span><span class="sxs-lookup"><span data-stu-id="0a7b7-105">Properties</span></span>

| <span data-ttu-id="0a7b7-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a7b7-106">Property</span></span>     | <span data-ttu-id="0a7b7-107">種類</span><span class="sxs-lookup"><span data-stu-id="0a7b7-107">Type</span></span>   |<span data-ttu-id="0a7b7-108">説明</span><span class="sxs-lookup"><span data-stu-id="0a7b7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a7b7-109">city</span><span class="sxs-lookup"><span data-stu-id="0a7b7-109">city</span></span>|<span data-ttu-id="0a7b7-110">String</span><span class="sxs-lookup"><span data-stu-id="0a7b7-110">String</span></span>|<span data-ttu-id="0a7b7-111">市区町村。</span><span class="sxs-lookup"><span data-stu-id="0a7b7-111">The city.</span></span>|
|<span data-ttu-id="0a7b7-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="0a7b7-112">countryOrRegion</span></span>|<span data-ttu-id="0a7b7-113">String</span><span class="sxs-lookup"><span data-stu-id="0a7b7-113">String</span></span>|<span data-ttu-id="0a7b7-p101">国または地域。自由形式の文字列値です。例: 「米国」。</span><span class="sxs-lookup"><span data-stu-id="0a7b7-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="0a7b7-116">officeLocation</span><span class="sxs-lookup"><span data-stu-id="0a7b7-116">officeLocation</span></span>  | <span data-ttu-id="0a7b7-117">String</span><span class="sxs-lookup"><span data-stu-id="0a7b7-117">String</span></span> | <span data-ttu-id="0a7b7-118">組織の連絡先の数の建物や事務所などの場所を Office です。</span><span class="sxs-lookup"><span data-stu-id="0a7b7-118">Office location such as building and office number for an organizational contact.</span></span>  |
|<span data-ttu-id="0a7b7-119">postalCode</span><span class="sxs-lookup"><span data-stu-id="0a7b7-119">postalCode</span></span>|<span data-ttu-id="0a7b7-120">String</span><span class="sxs-lookup"><span data-stu-id="0a7b7-120">String</span></span>|<span data-ttu-id="0a7b7-121">郵便番号。</span><span class="sxs-lookup"><span data-stu-id="0a7b7-121">The postal code.</span></span>|
|<span data-ttu-id="0a7b7-122">state</span><span class="sxs-lookup"><span data-stu-id="0a7b7-122">state</span></span>|<span data-ttu-id="0a7b7-123">String</span><span class="sxs-lookup"><span data-stu-id="0a7b7-123">String</span></span>|<span data-ttu-id="0a7b7-124">都道府県。</span><span class="sxs-lookup"><span data-stu-id="0a7b7-124">The state.</span></span>|
|<span data-ttu-id="0a7b7-125">street</span><span class="sxs-lookup"><span data-stu-id="0a7b7-125">street</span></span>|<span data-ttu-id="0a7b7-126">String</span><span class="sxs-lookup"><span data-stu-id="0a7b7-126">String</span></span>|<span data-ttu-id="0a7b7-127">番地。</span><span class="sxs-lookup"><span data-stu-id="0a7b7-127">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0a7b7-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0a7b7-128">JSON representation</span></span>

<span data-ttu-id="0a7b7-129">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="0a7b7-129">Here is a JSON representation of the resource</span></span>

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
