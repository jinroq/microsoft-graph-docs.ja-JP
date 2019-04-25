---
title: bookingcustomer リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: cd4991b28f1dee0ba647a7f95b70817beffbef95
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543910"
---
# <a name="bookingcustomer-resource-type"></a><span data-ttu-id="db1fb-104">bookingcustomer リソースの種類</span><span class="sxs-lookup"><span data-stu-id="db1fb-104">bookingCustomer resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="db1fb-105">[bookingBsiness](bookingbusiness.md)のお客様を表します。</span><span class="sxs-lookup"><span data-stu-id="db1fb-105">Represents a customer of a [bookingBsiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="db1fb-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="db1fb-106">Methods</span></span>

| <span data-ttu-id="db1fb-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="db1fb-107">Method</span></span>           | <span data-ttu-id="db1fb-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="db1fb-108">Return Type</span></span>    |<span data-ttu-id="db1fb-109">説明</span><span class="sxs-lookup"><span data-stu-id="db1fb-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="db1fb-110">顧客を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="db1fb-110">List customers</span></span>](../api/bookingbusiness-list-customers.md) | <span data-ttu-id="db1fb-111">[bookingcustomer](bookingcustomer.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="db1fb-111">[bookingCustomer](bookingcustomer.md) collection</span></span> | <span data-ttu-id="db1fb-112">**bookingcustomer**オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="db1fb-112">Get a list of **bookingCustomer** objects.</span></span> |
|[<span data-ttu-id="db1fb-113">bookingcustomer の作成</span><span class="sxs-lookup"><span data-stu-id="db1fb-113">Create bookingCustomer</span></span>](../api/bookingbusiness-post-customers.md) | [<span data-ttu-id="db1fb-114">bookingcustomer</span><span class="sxs-lookup"><span data-stu-id="db1fb-114">bookingCustomer</span></span>](bookingcustomer.md) | <span data-ttu-id="db1fb-115">新しい**bookcustomer**オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="db1fb-115">Create a new **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="db1fb-116">bookingcustomer を取得する</span><span class="sxs-lookup"><span data-stu-id="db1fb-116">Get bookingCustomer</span></span>](../api/bookingcustomer-get.md) | [<span data-ttu-id="db1fb-117">bookingcustomer</span><span class="sxs-lookup"><span data-stu-id="db1fb-117">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="db1fb-118">**bookingcustomer**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="db1fb-118">Read the properties and relationships of a **bookingCustomer** object.</span></span>|
|[<span data-ttu-id="db1fb-119">更新</span><span class="sxs-lookup"><span data-stu-id="db1fb-119">Update</span></span>](../api/bookingcustomer-update.md) | [<span data-ttu-id="db1fb-120">bookingcustomer</span><span class="sxs-lookup"><span data-stu-id="db1fb-120">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="db1fb-121">**bookingcustomer**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="db1fb-121">Update a **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="db1fb-122">削除</span><span class="sxs-lookup"><span data-stu-id="db1fb-122">Delete</span></span>](../api/bookingcustomer-delete.md) | <span data-ttu-id="db1fb-123">なし</span><span class="sxs-lookup"><span data-stu-id="db1fb-123">None</span></span> |<span data-ttu-id="db1fb-124">**bookingcustomer**オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="db1fb-124">Delete a **bookingCustomer** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="db1fb-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="db1fb-125">Properties</span></span>
| <span data-ttu-id="db1fb-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="db1fb-126">Property</span></span>     | <span data-ttu-id="db1fb-127">型</span><span class="sxs-lookup"><span data-stu-id="db1fb-127">Type</span></span>   |<span data-ttu-id="db1fb-128">説明</span><span class="sxs-lookup"><span data-stu-id="db1fb-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db1fb-129">displayName</span><span class="sxs-lookup"><span data-stu-id="db1fb-129">displayName</span></span>|<span data-ttu-id="db1fb-130">String</span><span class="sxs-lookup"><span data-stu-id="db1fb-130">String</span></span>|<span data-ttu-id="db1fb-131">顧客の名前。</span><span class="sxs-lookup"><span data-stu-id="db1fb-131">The name of the customer.</span></span>|
|<span data-ttu-id="db1fb-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="db1fb-132">emailAddress</span></span>|<span data-ttu-id="db1fb-133">String</span><span class="sxs-lookup"><span data-stu-id="db1fb-133">String</span></span>|<span data-ttu-id="db1fb-134">顧客の SMTP アドレス。</span><span class="sxs-lookup"><span data-stu-id="db1fb-134">The SMTP address of the customer.</span></span>|
|<span data-ttu-id="db1fb-135">id</span><span class="sxs-lookup"><span data-stu-id="db1fb-135">id</span></span>|<span data-ttu-id="db1fb-136">String</span><span class="sxs-lookup"><span data-stu-id="db1fb-136">String</span></span>| <span data-ttu-id="db1fb-137">顧客の ID。</span><span class="sxs-lookup"><span data-stu-id="db1fb-137">The ID of the customer.</span></span> <span data-ttu-id="db1fb-138">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="db1fb-138">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db1fb-139">関係</span><span class="sxs-lookup"><span data-stu-id="db1fb-139">Relationships</span></span>
<span data-ttu-id="db1fb-140">なし</span><span class="sxs-lookup"><span data-stu-id="db1fb-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="db1fb-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="db1fb-141">JSON representation</span></span>

<span data-ttu-id="db1fb-142">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="db1fb-142">The following is a JSON representation of the resource.</span></span>

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
