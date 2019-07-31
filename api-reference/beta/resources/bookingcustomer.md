---
title: bookingCustomer リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 864635014b3e215dabd11896922ca9e73a5e8cb9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974172"
---
# <a name="bookingcustomer-resource-type"></a><span data-ttu-id="3daf9-104">bookingCustomer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3daf9-104">bookingCustomer resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="3daf9-105">[Bookingbusiness](bookingbusiness.md)のお客様を表します。</span><span class="sxs-lookup"><span data-stu-id="3daf9-105">Represents a customer of a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="3daf9-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="3daf9-106">Methods</span></span>

| <span data-ttu-id="3daf9-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="3daf9-107">Method</span></span>           | <span data-ttu-id="3daf9-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3daf9-108">Return Type</span></span>    |<span data-ttu-id="3daf9-109">説明</span><span class="sxs-lookup"><span data-stu-id="3daf9-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3daf9-110">顧客を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="3daf9-110">List customers</span></span>](../api/bookingbusiness-list-customers.md) | <span data-ttu-id="3daf9-111">[Bookingcustomer](bookingcustomer.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3daf9-111">[bookingCustomer](bookingcustomer.md) collection</span></span> | <span data-ttu-id="3daf9-112">**Bookingcustomer**オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="3daf9-112">Get a list of **bookingCustomer** objects.</span></span> |
|[<span data-ttu-id="3daf9-113">BookingCustomer の作成</span><span class="sxs-lookup"><span data-stu-id="3daf9-113">Create bookingCustomer</span></span>](../api/bookingbusiness-post-customers.md) | [<span data-ttu-id="3daf9-114">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="3daf9-114">bookingCustomer</span></span>](bookingcustomer.md) | <span data-ttu-id="3daf9-115">新しい**Bookcustomer**オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3daf9-115">Create a new **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="3daf9-116">BookingCustomer を取得する</span><span class="sxs-lookup"><span data-stu-id="3daf9-116">Get bookingCustomer</span></span>](../api/bookingcustomer-get.md) | [<span data-ttu-id="3daf9-117">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="3daf9-117">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="3daf9-118">**Bookingcustomer**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3daf9-118">Read the properties and relationships of a **bookingCustomer** object.</span></span>|
|[<span data-ttu-id="3daf9-119">Update</span><span class="sxs-lookup"><span data-stu-id="3daf9-119">Update</span></span>](../api/bookingcustomer-update.md) | [<span data-ttu-id="3daf9-120">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="3daf9-120">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="3daf9-121">**Bookingcustomer**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="3daf9-121">Update a **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="3daf9-122">Delete</span><span class="sxs-lookup"><span data-stu-id="3daf9-122">Delete</span></span>](../api/bookingcustomer-delete.md) | <span data-ttu-id="3daf9-123">None</span><span class="sxs-lookup"><span data-stu-id="3daf9-123">None</span></span> |<span data-ttu-id="3daf9-124">**Bookingcustomer**オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="3daf9-124">Delete a **bookingCustomer** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3daf9-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3daf9-125">Properties</span></span>
| <span data-ttu-id="3daf9-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3daf9-126">Property</span></span>     | <span data-ttu-id="3daf9-127">型</span><span class="sxs-lookup"><span data-stu-id="3daf9-127">Type</span></span>   |<span data-ttu-id="3daf9-128">説明</span><span class="sxs-lookup"><span data-stu-id="3daf9-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3daf9-129">displayName</span><span class="sxs-lookup"><span data-stu-id="3daf9-129">displayName</span></span>|<span data-ttu-id="3daf9-130">String</span><span class="sxs-lookup"><span data-stu-id="3daf9-130">String</span></span>|<span data-ttu-id="3daf9-131">顧客の名前。</span><span class="sxs-lookup"><span data-stu-id="3daf9-131">The name of the customer.</span></span>|
|<span data-ttu-id="3daf9-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="3daf9-132">emailAddress</span></span>|<span data-ttu-id="3daf9-133">String</span><span class="sxs-lookup"><span data-stu-id="3daf9-133">String</span></span>|<span data-ttu-id="3daf9-134">顧客の SMTP アドレス。</span><span class="sxs-lookup"><span data-stu-id="3daf9-134">The SMTP address of the customer.</span></span>|
|<span data-ttu-id="3daf9-135">id</span><span class="sxs-lookup"><span data-stu-id="3daf9-135">id</span></span>|<span data-ttu-id="3daf9-136">文字列</span><span class="sxs-lookup"><span data-stu-id="3daf9-136">String</span></span>| <span data-ttu-id="3daf9-137">顧客の ID。</span><span class="sxs-lookup"><span data-stu-id="3daf9-137">The ID of the customer.</span></span> <span data-ttu-id="3daf9-138">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3daf9-138">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3daf9-139">関係</span><span class="sxs-lookup"><span data-stu-id="3daf9-139">Relationships</span></span>
<span data-ttu-id="3daf9-140">なし</span><span class="sxs-lookup"><span data-stu-id="3daf9-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3daf9-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3daf9-141">JSON representation</span></span>

<span data-ttu-id="3daf9-142">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3daf9-142">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
