---
title: bookingCustomer リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: cd4991b28f1dee0ba647a7f95b70817beffbef95
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522218"
---
# <a name="bookingcustomer-resource-type"></a><span data-ttu-id="4ffaa-104">bookingCustomer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4ffaa-104">bookingCustomer resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="4ffaa-105">の[bookingBsiness](bookingbusiness.md)の顧客を表します。</span><span class="sxs-lookup"><span data-stu-id="4ffaa-105">Represents a customer of a [bookingBsiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="4ffaa-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="4ffaa-106">Methods</span></span>

| <span data-ttu-id="4ffaa-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="4ffaa-107">Method</span></span>           | <span data-ttu-id="4ffaa-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4ffaa-108">Return Type</span></span>    |<span data-ttu-id="4ffaa-109">説明</span><span class="sxs-lookup"><span data-stu-id="4ffaa-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4ffaa-110">顧客のリスト</span><span class="sxs-lookup"><span data-stu-id="4ffaa-110">List customers</span></span>](../api/bookingbusiness-list-customers.md) | <span data-ttu-id="4ffaa-111">[bookingCustomer](bookingcustomer.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4ffaa-111">[bookingCustomer](bookingcustomer.md) collection</span></span> | <span data-ttu-id="4ffaa-112">**BookingCustomer**オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="4ffaa-112">Get a list of **bookingCustomer** objects.</span></span> |
|[<span data-ttu-id="4ffaa-113">BookingCustomer を作成します。</span><span class="sxs-lookup"><span data-stu-id="4ffaa-113">Create bookingCustomer</span></span>](../api/bookingbusiness-post-customers.md) | [<span data-ttu-id="4ffaa-114">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="4ffaa-114">bookingCustomer</span></span>](bookingcustomer.md) | <span data-ttu-id="4ffaa-115">新しい**bookingCustomer**オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4ffaa-115">Create a new **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="4ffaa-116">BookingCustomer を取得します。</span><span class="sxs-lookup"><span data-stu-id="4ffaa-116">Get bookingCustomer</span></span>](../api/bookingcustomer-get.md) | [<span data-ttu-id="4ffaa-117">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="4ffaa-117">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="4ffaa-118">プロパティと、 **bookingCustomer**オブジェクトの関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4ffaa-118">Read the properties and relationships of a **bookingCustomer** object.</span></span>|
|[<span data-ttu-id="4ffaa-119">Update</span><span class="sxs-lookup"><span data-stu-id="4ffaa-119">Update</span></span>](../api/bookingcustomer-update.md) | [<span data-ttu-id="4ffaa-120">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="4ffaa-120">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="4ffaa-121">**BookingCustomer**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="4ffaa-121">Update a **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="4ffaa-122">Delete</span><span class="sxs-lookup"><span data-stu-id="4ffaa-122">Delete</span></span>](../api/bookingcustomer-delete.md) | <span data-ttu-id="4ffaa-123">なし</span><span class="sxs-lookup"><span data-stu-id="4ffaa-123">None</span></span> |<span data-ttu-id="4ffaa-124">**BookingCustomer**オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="4ffaa-124">Delete a **bookingCustomer** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4ffaa-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4ffaa-125">Properties</span></span>
| <span data-ttu-id="4ffaa-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4ffaa-126">Property</span></span>     | <span data-ttu-id="4ffaa-127">型</span><span class="sxs-lookup"><span data-stu-id="4ffaa-127">Type</span></span>   |<span data-ttu-id="4ffaa-128">説明</span><span class="sxs-lookup"><span data-stu-id="4ffaa-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ffaa-129">displayName</span><span class="sxs-lookup"><span data-stu-id="4ffaa-129">displayName</span></span>|<span data-ttu-id="4ffaa-130">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4ffaa-130">String</span></span>|<span data-ttu-id="4ffaa-131">顧客の名前。</span><span class="sxs-lookup"><span data-stu-id="4ffaa-131">The name of the customer.</span></span>|
|<span data-ttu-id="4ffaa-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="4ffaa-132">emailAddress</span></span>|<span data-ttu-id="4ffaa-133">String</span><span class="sxs-lookup"><span data-stu-id="4ffaa-133">String</span></span>|<span data-ttu-id="4ffaa-134">お客様の SMTP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="4ffaa-134">The SMTP address of the customer.</span></span>|
|<span data-ttu-id="4ffaa-135">id</span><span class="sxs-lookup"><span data-stu-id="4ffaa-135">id</span></span>|<span data-ttu-id="4ffaa-136">文字列</span><span class="sxs-lookup"><span data-stu-id="4ffaa-136">String</span></span>| <span data-ttu-id="4ffaa-137">顧客の ID です。</span><span class="sxs-lookup"><span data-stu-id="4ffaa-137">The ID of the customer.</span></span> <span data-ttu-id="4ffaa-138">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4ffaa-138">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ffaa-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4ffaa-139">Relationships</span></span>
<span data-ttu-id="4ffaa-140">なし</span><span class="sxs-lookup"><span data-stu-id="4ffaa-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4ffaa-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4ffaa-141">JSON representation</span></span>

<span data-ttu-id="4ffaa-142">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4ffaa-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingCustomer"
}-->

```json
{
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingCustomer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingcustomer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
