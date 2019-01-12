---
title: bookingPerson リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: e39fbbf12909e7a4d29c95e22896df081522a7d2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990111"
---
# <a name="bookingperson-resource-type"></a><span data-ttu-id="cc5be-104">bookingPerson リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cc5be-104">bookingPerson resource type</span></span>

 > <span data-ttu-id="cc5be-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cc5be-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc5be-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc5be-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="cc5be-107">これは、 [bookingCustomer](bookingcustomer.md)または[bookingStaffMember](bookingstaffmember.md)であることができます、Microsoft の予約のビジネス ユーザーの基本型です。</span><span class="sxs-lookup"><span data-stu-id="cc5be-107">This is a base type for a person in a Microsoft Bookings business, which can be a [bookingCustomer](bookingcustomer.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cc5be-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc5be-108">Properties</span></span>
| <span data-ttu-id="cc5be-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc5be-109">Property</span></span>     | <span data-ttu-id="cc5be-110">種類</span><span class="sxs-lookup"><span data-stu-id="cc5be-110">Type</span></span>   |<span data-ttu-id="cc5be-111">説明</span><span class="sxs-lookup"><span data-stu-id="cc5be-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc5be-112">displayName</span><span class="sxs-lookup"><span data-stu-id="cc5be-112">displayName</span></span>|<span data-ttu-id="cc5be-113">String</span><span class="sxs-lookup"><span data-stu-id="cc5be-113">String</span></span>|<span data-ttu-id="cc5be-114">派生のエンティティは、顧客とのインターフェイスの名前です。</span><span class="sxs-lookup"><span data-stu-id="cc5be-114">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="cc5be-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="cc5be-115">emailAddress</span></span>|<span data-ttu-id="cc5be-116">String</span><span class="sxs-lookup"><span data-stu-id="cc5be-116">String</span></span>|<span data-ttu-id="cc5be-117">ユーザーの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="cc5be-117">The email address of the person.</span></span>|
|<span data-ttu-id="cc5be-118">id</span><span class="sxs-lookup"><span data-stu-id="cc5be-118">id</span></span>|<span data-ttu-id="cc5be-119">String</span><span class="sxs-lookup"><span data-stu-id="cc5be-119">String</span></span>| <span data-ttu-id="cc5be-120">派生エンティティの ID です。</span><span class="sxs-lookup"><span data-stu-id="cc5be-120">The ID for the derived entity.</span></span> <span data-ttu-id="cc5be-121">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cc5be-121">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc5be-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cc5be-122">Relationships</span></span>
<span data-ttu-id="cc5be-123">なし</span><span class="sxs-lookup"><span data-stu-id="cc5be-123">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="cc5be-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cc5be-124">JSON representation</span></span>

<span data-ttu-id="cc5be-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cc5be-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingPerson"
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
  "description": "bookingPerson resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
