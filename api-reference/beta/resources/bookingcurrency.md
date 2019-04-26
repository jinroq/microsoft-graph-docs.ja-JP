---
title: bookingcurrency リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 6ab74cff24e1f575166f6672523ecc5d94bc1826
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328236"
---
# <a name="bookingcurrency-resource-type"></a><span data-ttu-id="cdd3f-104">bookingcurrency リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cdd3f-104">bookingCurrency resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="cdd3f-105">[bookingbusiness](bookingbusiness.md)でサポートされている通貨通貨を表します。</span><span class="sxs-lookup"><span data-stu-id="cdd3f-105">Represents a monetary currency supported by a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="cdd3f-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="cdd3f-106">Methods</span></span>

| <span data-ttu-id="cdd3f-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="cdd3f-107">Method</span></span>           | <span data-ttu-id="cdd3f-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cdd3f-108">Return Type</span></span>    |<span data-ttu-id="cdd3f-109">説明</span><span class="sxs-lookup"><span data-stu-id="cdd3f-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cdd3f-110">bookingcurrencies のリスト</span><span class="sxs-lookup"><span data-stu-id="cdd3f-110">List bookingCurrencies</span></span>](../api/bookingcurrency-list.md) | <span data-ttu-id="cdd3f-111">[bookingcurrency](bookingcurrency.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cdd3f-111">[bookingCurrency](bookingcurrency.md) collection</span></span> |<span data-ttu-id="cdd3f-112">Microsoft の予約ビジネスで使用できる**bookingcurrency**オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="cdd3f-112">Get a list of **bookingCurrency** objects available to a Microsoft Bookings business.</span></span>|
|[<span data-ttu-id="cdd3f-113">bookingcurrency の取得</span><span class="sxs-lookup"><span data-stu-id="cdd3f-113">Get bookingCurrency</span></span>](../api/bookingcurrency-get.md) | [<span data-ttu-id="cdd3f-114">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="cdd3f-114">bookingCurrency</span></span>](bookingcurrency.md) |<span data-ttu-id="cdd3f-115">**bookingcurrency**オブジェクトのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="cdd3f-115">Get the properties of a **bookingCurrency** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="cdd3f-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cdd3f-116">Properties</span></span>
| <span data-ttu-id="cdd3f-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cdd3f-117">Property</span></span>     | <span data-ttu-id="cdd3f-118">型</span><span class="sxs-lookup"><span data-stu-id="cdd3f-118">Type</span></span>   |<span data-ttu-id="cdd3f-119">説明</span><span class="sxs-lookup"><span data-stu-id="cdd3f-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cdd3f-120">id</span><span class="sxs-lookup"><span data-stu-id="cdd3f-120">id</span></span>|<span data-ttu-id="cdd3f-121">String</span><span class="sxs-lookup"><span data-stu-id="cdd3f-121">String</span></span>| <span data-ttu-id="cdd3f-122">[ISO 4217](https://www.iso.org/iso-4217-currency-codes.html)に基づく3文字の通貨コード。</span><span class="sxs-lookup"><span data-stu-id="cdd3f-122">A 3-character currency code, based on [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span></span> <span data-ttu-id="cdd3f-123">たとえば、米国ドルの通貨コードは USD で、オーストラリアドルは AUD になります。</span><span class="sxs-lookup"><span data-stu-id="cdd3f-123">For example, the currency code for the US dollar is USD, and for the Australian dollar is AUD.</span></span> <span data-ttu-id="cdd3f-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cdd3f-124">Read-only.</span></span>|
|<span data-ttu-id="cdd3f-125">疑問符</span><span class="sxs-lookup"><span data-stu-id="cdd3f-125">symbol</span></span>|<span data-ttu-id="cdd3f-126">String</span><span class="sxs-lookup"><span data-stu-id="cdd3f-126">String</span></span>| <span data-ttu-id="cdd3f-127">通貨記号。</span><span class="sxs-lookup"><span data-stu-id="cdd3f-127">The currency symbol.</span></span> <span data-ttu-id="cdd3f-128">たとえば、米ドルおよびオーストラリアドルの通貨記号は $ です。</span><span class="sxs-lookup"><span data-stu-id="cdd3f-128">For example, the currency symbol for the US dollar and for the Australian dollar is $.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="cdd3f-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cdd3f-129">Relationships</span></span>
<span data-ttu-id="cdd3f-130">なし</span><span class="sxs-lookup"><span data-stu-id="cdd3f-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="cdd3f-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cdd3f-131">JSON representation</span></span>

<span data-ttu-id="cdd3f-132">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cdd3f-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingCurrency"
}-->

```json
{
  "id": "String (identifier)",
  "symbol": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingCurrency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
