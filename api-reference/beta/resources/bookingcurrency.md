---
title: bookingcurrency リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 9d4feac66e72c756173113101a88bf8bbe35563a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535460"
---
# <a name="bookingcurrency-resource-type"></a><span data-ttu-id="85732-104">bookingcurrency リソースの種類</span><span class="sxs-lookup"><span data-stu-id="85732-104">bookingCurrency resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="85732-105">[bookingbusiness](bookingbusiness.md)でサポートされている通貨通貨を表します。</span><span class="sxs-lookup"><span data-stu-id="85732-105">Represents a monetary currency supported by a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="85732-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="85732-106">Methods</span></span>

| <span data-ttu-id="85732-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="85732-107">Method</span></span>           | <span data-ttu-id="85732-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="85732-108">Return Type</span></span>    |<span data-ttu-id="85732-109">説明</span><span class="sxs-lookup"><span data-stu-id="85732-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="85732-110">bookingcurrencies のリスト</span><span class="sxs-lookup"><span data-stu-id="85732-110">List bookingCurrencies</span></span>](../api/bookingcurrency-list.md) | <span data-ttu-id="85732-111">[bookingcurrency](bookingcurrency.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="85732-111">[bookingCurrency](bookingcurrency.md) collection</span></span> |<span data-ttu-id="85732-112">Microsoft の予約ビジネスで使用できる**bookingcurrency**オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="85732-112">Get a list of **bookingCurrency** objects available to a Microsoft Bookings business.</span></span>|
|[<span data-ttu-id="85732-113">bookingcurrency の取得</span><span class="sxs-lookup"><span data-stu-id="85732-113">Get bookingCurrency</span></span>](../api/bookingcurrency-get.md) | [<span data-ttu-id="85732-114">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="85732-114">bookingCurrency</span></span>](bookingcurrency.md) |<span data-ttu-id="85732-115">**bookingcurrency**オブジェクトのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="85732-115">Get the properties of a **bookingCurrency** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="85732-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="85732-116">Properties</span></span>
| <span data-ttu-id="85732-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="85732-117">Property</span></span>     | <span data-ttu-id="85732-118">型</span><span class="sxs-lookup"><span data-stu-id="85732-118">Type</span></span>   |<span data-ttu-id="85732-119">説明</span><span class="sxs-lookup"><span data-stu-id="85732-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85732-120">id</span><span class="sxs-lookup"><span data-stu-id="85732-120">id</span></span>|<span data-ttu-id="85732-121">String</span><span class="sxs-lookup"><span data-stu-id="85732-121">String</span></span>| <span data-ttu-id="85732-122">[ISO 4217](https://www.iso.org/iso-4217-currency-codes.html)に基づく3文字の通貨コード。</span><span class="sxs-lookup"><span data-stu-id="85732-122">A 3-character currency code, based on [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span></span> <span data-ttu-id="85732-123">たとえば、米国ドルの通貨コードは USD で、オーストラリアドルは AUD になります。</span><span class="sxs-lookup"><span data-stu-id="85732-123">For example, the currency code for the US dollar is USD, and for the Australian dollar is AUD.</span></span> <span data-ttu-id="85732-124">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="85732-124">Read-only.</span></span>|
|<span data-ttu-id="85732-125">疑問符</span><span class="sxs-lookup"><span data-stu-id="85732-125">symbol</span></span>|<span data-ttu-id="85732-126">String</span><span class="sxs-lookup"><span data-stu-id="85732-126">String</span></span>| <span data-ttu-id="85732-127">通貨記号。</span><span class="sxs-lookup"><span data-stu-id="85732-127">The currency symbol.</span></span> <span data-ttu-id="85732-128">たとえば、米ドルおよびオーストラリアドルの通貨記号は $ です。</span><span class="sxs-lookup"><span data-stu-id="85732-128">For example, the currency symbol for the US dollar and for the Australian dollar is $.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="85732-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="85732-129">Relationships</span></span>
<span data-ttu-id="85732-130">なし</span><span class="sxs-lookup"><span data-stu-id="85732-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="85732-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="85732-131">JSON representation</span></span>

<span data-ttu-id="85732-132">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="85732-132">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingcurrency.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
