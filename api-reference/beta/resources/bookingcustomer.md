---
title: bookingCustomer リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: b213e4026ee33886c0e56db9790efff09fd8c522
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925106"
---
# <a name="bookingcustomer-resource-type"></a><span data-ttu-id="9d684-104">bookingCustomer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9d684-104">bookingCustomer resource type</span></span>

 > <span data-ttu-id="9d684-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9d684-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d684-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d684-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="9d684-107">の[bookingBsiness](bookingbusiness.md)の顧客を表します。</span><span class="sxs-lookup"><span data-stu-id="9d684-107">Represents a customer of a [bookingBsiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="9d684-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="9d684-108">Methods</span></span>

| <span data-ttu-id="9d684-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="9d684-109">Method</span></span>           | <span data-ttu-id="9d684-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9d684-110">Return Type</span></span>    |<span data-ttu-id="9d684-111">説明</span><span class="sxs-lookup"><span data-stu-id="9d684-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9d684-112">顧客のリスト</span><span class="sxs-lookup"><span data-stu-id="9d684-112">List customers</span></span>](../api/bookingbusiness-list-customers.md) | <span data-ttu-id="9d684-113">[bookingCustomer](bookingcustomer.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9d684-113">[bookingCustomer](bookingcustomer.md) collection</span></span> | <span data-ttu-id="9d684-114">**BookingCustomer**オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="9d684-114">Get a list of **bookingCustomer** objects.</span></span> |
|[<span data-ttu-id="9d684-115">BookingCustomer を作成します。</span><span class="sxs-lookup"><span data-stu-id="9d684-115">Create bookingCustomer</span></span>](../api/bookingbusiness-post-customers.md) | [<span data-ttu-id="9d684-116">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="9d684-116">bookingCustomer</span></span>](bookingcustomer.md) | <span data-ttu-id="9d684-117">新しい**bookingCustomer**オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9d684-117">Create a new **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="9d684-118">BookingCustomer を取得します。</span><span class="sxs-lookup"><span data-stu-id="9d684-118">Get bookingCustomer</span></span>](../api/bookingcustomer-get.md) | [<span data-ttu-id="9d684-119">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="9d684-119">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="9d684-120">プロパティと、 **bookingCustomer**オブジェクトの関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9d684-120">Read the properties and relationships of a **bookingCustomer** object.</span></span>|
|[<span data-ttu-id="9d684-121">Update</span><span class="sxs-lookup"><span data-stu-id="9d684-121">Update</span></span>](../api/bookingcustomer-update.md) | [<span data-ttu-id="9d684-122">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="9d684-122">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="9d684-123">**BookingCustomer**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="9d684-123">Update a **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="9d684-124">Delete</span><span class="sxs-lookup"><span data-stu-id="9d684-124">Delete</span></span>](../api/bookingcustomer-delete.md) | <span data-ttu-id="9d684-125">なし</span><span class="sxs-lookup"><span data-stu-id="9d684-125">None</span></span> |<span data-ttu-id="9d684-126">**BookingCustomer**オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="9d684-126">Delete a **bookingCustomer** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9d684-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d684-127">Properties</span></span>
| <span data-ttu-id="9d684-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d684-128">Property</span></span>     | <span data-ttu-id="9d684-129">種類</span><span class="sxs-lookup"><span data-stu-id="9d684-129">Type</span></span>   |<span data-ttu-id="9d684-130">説明</span><span class="sxs-lookup"><span data-stu-id="9d684-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d684-131">displayName</span><span class="sxs-lookup"><span data-stu-id="9d684-131">displayName</span></span>|<span data-ttu-id="9d684-132">String</span><span class="sxs-lookup"><span data-stu-id="9d684-132">String</span></span>|<span data-ttu-id="9d684-133">顧客の名前。</span><span class="sxs-lookup"><span data-stu-id="9d684-133">The name of the customer.</span></span>|
|<span data-ttu-id="9d684-134">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9d684-134">emailAddress</span></span>|<span data-ttu-id="9d684-135">String</span><span class="sxs-lookup"><span data-stu-id="9d684-135">String</span></span>|<span data-ttu-id="9d684-136">お客様の SMTP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="9d684-136">The SMTP address of the customer.</span></span>|
|<span data-ttu-id="9d684-137">id</span><span class="sxs-lookup"><span data-stu-id="9d684-137">id</span></span>|<span data-ttu-id="9d684-138">String</span><span class="sxs-lookup"><span data-stu-id="9d684-138">String</span></span>| <span data-ttu-id="9d684-139">顧客の ID です。</span><span class="sxs-lookup"><span data-stu-id="9d684-139">The ID of the customer.</span></span> <span data-ttu-id="9d684-140">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9d684-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d684-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9d684-141">Relationships</span></span>
<span data-ttu-id="9d684-142">なし</span><span class="sxs-lookup"><span data-stu-id="9d684-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9d684-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9d684-143">JSON representation</span></span>

<span data-ttu-id="9d684-144">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9d684-144">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingCustomer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
