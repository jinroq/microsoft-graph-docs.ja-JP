---
title: bookingcustomer リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: f97f3d36599fe088f28176d001fecc701bb5e3ab
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339072"
---
# <a name="bookingcustomer-resource-type"></a><span data-ttu-id="4b5cf-104">bookingcustomer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4b5cf-104">bookingCustomer resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="4b5cf-105">[bookingBsiness](bookingbusiness.md)のお客様を表します。</span><span class="sxs-lookup"><span data-stu-id="4b5cf-105">Represents a customer of a [bookingBsiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="4b5cf-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="4b5cf-106">Methods</span></span>

| <span data-ttu-id="4b5cf-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="4b5cf-107">Method</span></span>           | <span data-ttu-id="4b5cf-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4b5cf-108">Return Type</span></span>    |<span data-ttu-id="4b5cf-109">説明</span><span class="sxs-lookup"><span data-stu-id="4b5cf-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4b5cf-110">顧客を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="4b5cf-110">List customers</span></span>](../api/bookingbusiness-list-customers.md) | <span data-ttu-id="4b5cf-111">[bookingcustomer](bookingcustomer.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4b5cf-111">[bookingCustomer](bookingcustomer.md) collection</span></span> | <span data-ttu-id="4b5cf-112">**bookingcustomer**オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="4b5cf-112">Get a list of **bookingCustomer** objects.</span></span> |
|[<span data-ttu-id="4b5cf-113">bookingcustomer の作成</span><span class="sxs-lookup"><span data-stu-id="4b5cf-113">Create bookingCustomer</span></span>](../api/bookingbusiness-post-customers.md) | [<span data-ttu-id="4b5cf-114">bookingcustomer</span><span class="sxs-lookup"><span data-stu-id="4b5cf-114">bookingCustomer</span></span>](bookingcustomer.md) | <span data-ttu-id="4b5cf-115">新しい**bookcustomer**オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4b5cf-115">Create a new **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="4b5cf-116">bookingcustomer を取得する</span><span class="sxs-lookup"><span data-stu-id="4b5cf-116">Get bookingCustomer</span></span>](../api/bookingcustomer-get.md) | [<span data-ttu-id="4b5cf-117">bookingcustomer</span><span class="sxs-lookup"><span data-stu-id="4b5cf-117">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="4b5cf-118">**bookingcustomer**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4b5cf-118">Read the properties and relationships of a **bookingCustomer** object.</span></span>|
|[<span data-ttu-id="4b5cf-119">更新する</span><span class="sxs-lookup"><span data-stu-id="4b5cf-119">Update</span></span>](../api/bookingcustomer-update.md) | [<span data-ttu-id="4b5cf-120">bookingcustomer</span><span class="sxs-lookup"><span data-stu-id="4b5cf-120">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="4b5cf-121">**bookingcustomer**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="4b5cf-121">Update a **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="4b5cf-122">削除</span><span class="sxs-lookup"><span data-stu-id="4b5cf-122">Delete</span></span>](../api/bookingcustomer-delete.md) | <span data-ttu-id="4b5cf-123">なし</span><span class="sxs-lookup"><span data-stu-id="4b5cf-123">None</span></span> |<span data-ttu-id="4b5cf-124">**bookingcustomer**オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="4b5cf-124">Delete a **bookingCustomer** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4b5cf-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b5cf-125">Properties</span></span>
| <span data-ttu-id="4b5cf-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b5cf-126">Property</span></span>     | <span data-ttu-id="4b5cf-127">型</span><span class="sxs-lookup"><span data-stu-id="4b5cf-127">Type</span></span>   |<span data-ttu-id="4b5cf-128">説明</span><span class="sxs-lookup"><span data-stu-id="4b5cf-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b5cf-129">displayName</span><span class="sxs-lookup"><span data-stu-id="4b5cf-129">displayName</span></span>|<span data-ttu-id="4b5cf-130">String</span><span class="sxs-lookup"><span data-stu-id="4b5cf-130">String</span></span>|<span data-ttu-id="4b5cf-131">顧客の名前。</span><span class="sxs-lookup"><span data-stu-id="4b5cf-131">The name of the customer.</span></span>|
|<span data-ttu-id="4b5cf-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="4b5cf-132">emailAddress</span></span>|<span data-ttu-id="4b5cf-133">String</span><span class="sxs-lookup"><span data-stu-id="4b5cf-133">String</span></span>|<span data-ttu-id="4b5cf-134">顧客の SMTP アドレス。</span><span class="sxs-lookup"><span data-stu-id="4b5cf-134">The SMTP address of the customer.</span></span>|
|<span data-ttu-id="4b5cf-135">id</span><span class="sxs-lookup"><span data-stu-id="4b5cf-135">id</span></span>|<span data-ttu-id="4b5cf-136">String</span><span class="sxs-lookup"><span data-stu-id="4b5cf-136">String</span></span>| <span data-ttu-id="4b5cf-137">顧客の ID。</span><span class="sxs-lookup"><span data-stu-id="4b5cf-137">The ID of the customer.</span></span> <span data-ttu-id="4b5cf-138">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4b5cf-138">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b5cf-139">関係</span><span class="sxs-lookup"><span data-stu-id="4b5cf-139">Relationships</span></span>
<span data-ttu-id="4b5cf-140">なし</span><span class="sxs-lookup"><span data-stu-id="4b5cf-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4b5cf-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4b5cf-141">JSON representation</span></span>

<span data-ttu-id="4b5cf-142">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4b5cf-142">The following is a JSON representation of the resource.</span></span>

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
