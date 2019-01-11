---
title: bookingPerson リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: 606e0e0d1d851fac16b25310b278ca524124eb00
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845578"
---
# <a name="bookingperson-resource-type"></a><span data-ttu-id="1a1a8-104">bookingPerson リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1a1a8-104">bookingPerson resource type</span></span>

 > <span data-ttu-id="1a1a8-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1a1a8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a1a8-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a1a8-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="1a1a8-107">これは、 [bookingCustomer](bookingcustomer.md)または[bookingStaffMember](bookingstaffmember.md)であることができます、Microsoft の予約のビジネス ユーザーの基本型です。</span><span class="sxs-lookup"><span data-stu-id="1a1a8-107">This is a base type for a person in a Microsoft Bookings business, which can be a [bookingCustomer](bookingcustomer.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1a1a8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a1a8-108">Properties</span></span>
| <span data-ttu-id="1a1a8-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a1a8-109">Property</span></span>     | <span data-ttu-id="1a1a8-110">種類</span><span class="sxs-lookup"><span data-stu-id="1a1a8-110">Type</span></span>   |<span data-ttu-id="1a1a8-111">説明</span><span class="sxs-lookup"><span data-stu-id="1a1a8-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a1a8-112">displayName</span><span class="sxs-lookup"><span data-stu-id="1a1a8-112">displayName</span></span>|<span data-ttu-id="1a1a8-113">String</span><span class="sxs-lookup"><span data-stu-id="1a1a8-113">String</span></span>|<span data-ttu-id="1a1a8-114">派生のエンティティは、顧客とのインターフェイスの名前です。</span><span class="sxs-lookup"><span data-stu-id="1a1a8-114">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="1a1a8-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="1a1a8-115">emailAddress</span></span>|<span data-ttu-id="1a1a8-116">String</span><span class="sxs-lookup"><span data-stu-id="1a1a8-116">String</span></span>|<span data-ttu-id="1a1a8-117">ユーザーの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="1a1a8-117">The email address of the person.</span></span>|
|<span data-ttu-id="1a1a8-118">id</span><span class="sxs-lookup"><span data-stu-id="1a1a8-118">id</span></span>|<span data-ttu-id="1a1a8-119">String</span><span class="sxs-lookup"><span data-stu-id="1a1a8-119">String</span></span>| <span data-ttu-id="1a1a8-120">派生エンティティの ID です。</span><span class="sxs-lookup"><span data-stu-id="1a1a8-120">The ID for the derived entity.</span></span> <span data-ttu-id="1a1a8-121">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1a1a8-121">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a1a8-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1a1a8-122">Relationships</span></span>
<span data-ttu-id="1a1a8-123">なし</span><span class="sxs-lookup"><span data-stu-id="1a1a8-123">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1a1a8-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1a1a8-124">JSON representation</span></span>

<span data-ttu-id="1a1a8-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1a1a8-125">The following is a JSON representation of the resource.</span></span>

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
