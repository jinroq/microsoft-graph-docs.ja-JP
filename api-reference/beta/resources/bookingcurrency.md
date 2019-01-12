---
title: bookingCurrency リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 7e2289bfa6c6aac62f12d7321d06caaafbc41f8c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956004"
---
# <a name="bookingcurrency-resource-type"></a><span data-ttu-id="d110a-104">bookingCurrency リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d110a-104">bookingCurrency resource type</span></span>

 > <span data-ttu-id="d110a-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d110a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d110a-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d110a-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="d110a-107">[BookingBusiness](bookingbusiness.md)でサポートされている通貨の通貨を表します。</span><span class="sxs-lookup"><span data-stu-id="d110a-107">Represents a monetary currency supported by a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="d110a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d110a-108">Methods</span></span>

| <span data-ttu-id="d110a-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="d110a-109">Method</span></span>           | <span data-ttu-id="d110a-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d110a-110">Return Type</span></span>    |<span data-ttu-id="d110a-111">説明</span><span class="sxs-lookup"><span data-stu-id="d110a-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d110a-112">リスト bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="d110a-112">List bookingCurrencies</span></span>](../api/bookingcurrency-list.md) | <span data-ttu-id="d110a-113">[bookingCurrency](bookingcurrency.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d110a-113">[bookingCurrency](bookingcurrency.md) collection</span></span> |<span data-ttu-id="d110a-114">Microsoft 予約業務に利用可能な**bookingCurrency**のオブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="d110a-114">Get a list of **bookingCurrency** objects available to a Microsoft Bookings business.</span></span>|
|[<span data-ttu-id="d110a-115">BookingCurrency を取得します。</span><span class="sxs-lookup"><span data-stu-id="d110a-115">Get bookingCurrency</span></span>](../api/bookingcurrency-get.md) | [<span data-ttu-id="d110a-116">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="d110a-116">bookingCurrency</span></span>](bookingcurrency.md) |<span data-ttu-id="d110a-117">**BookingCurrency**オブジェクトのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="d110a-117">Get the properties of a **bookingCurrency** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="d110a-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d110a-118">Properties</span></span>
| <span data-ttu-id="d110a-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d110a-119">Property</span></span>     | <span data-ttu-id="d110a-120">種類</span><span class="sxs-lookup"><span data-stu-id="d110a-120">Type</span></span>   |<span data-ttu-id="d110a-121">説明</span><span class="sxs-lookup"><span data-stu-id="d110a-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d110a-122">ID</span><span class="sxs-lookup"><span data-stu-id="d110a-122">id</span></span>|<span data-ttu-id="d110a-123">String</span><span class="sxs-lookup"><span data-stu-id="d110a-123">String</span></span>| <span data-ttu-id="d110a-124">[ISO 4217](https://www.iso.org/iso-4217-currency-codes.html)の 3 文字の通貨コード。</span><span class="sxs-lookup"><span data-stu-id="d110a-124">A 3-character currency code, based on [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span></span> <span data-ttu-id="d110a-125">たとえば、米ドルの通貨コードは米ドル、オーストラリアの AUD.</span><span class="sxs-lookup"><span data-stu-id="d110a-125">For example, the currency code for the US dollar is USD, and for the Australian dollar is AUD.</span></span> <span data-ttu-id="d110a-126">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d110a-126">Read-only.</span></span>|
|<span data-ttu-id="d110a-127">シンボル</span><span class="sxs-lookup"><span data-stu-id="d110a-127">symbol</span></span>|<span data-ttu-id="d110a-128">String</span><span class="sxs-lookup"><span data-stu-id="d110a-128">String</span></span>| <span data-ttu-id="d110a-129">通貨記号。</span><span class="sxs-lookup"><span data-stu-id="d110a-129">The currency symbol.</span></span> <span data-ttu-id="d110a-130">米ドルとオーストラリア ドルの通貨記号は $ です。</span><span class="sxs-lookup"><span data-stu-id="d110a-130">For example, the currency symbol for the US dollar and for the Australian dollar is $.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="d110a-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d110a-131">Relationships</span></span>
<span data-ttu-id="d110a-132">なし</span><span class="sxs-lookup"><span data-stu-id="d110a-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d110a-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d110a-133">JSON representation</span></span>

<span data-ttu-id="d110a-134">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d110a-134">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingCurrency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
