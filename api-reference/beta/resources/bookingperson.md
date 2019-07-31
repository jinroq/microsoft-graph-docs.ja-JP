---
title: bookingPerson リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 3c8db7aca957878247193207e00e969d8ddfc98e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974166"
---
# <a name="bookingperson-resource-type"></a><span data-ttu-id="a9785-104">bookingPerson リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a9785-104">bookingPerson resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="a9785-105">これは、Microsoft の予約ビジネスにおける個人の基本型です。これは、 [Bookingcustomer](bookingcustomer.md)または[bookingStaffMember](bookingstaffmember.md)にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a9785-105">This is a base type for a person in a Microsoft Bookings business, which can be a [bookingCustomer](bookingcustomer.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a9785-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9785-106">Properties</span></span>
| <span data-ttu-id="a9785-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9785-107">Property</span></span>     | <span data-ttu-id="a9785-108">型</span><span class="sxs-lookup"><span data-stu-id="a9785-108">Type</span></span>   |<span data-ttu-id="a9785-109">説明</span><span class="sxs-lookup"><span data-stu-id="a9785-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9785-110">displayName</span><span class="sxs-lookup"><span data-stu-id="a9785-110">displayName</span></span>|<span data-ttu-id="a9785-111">String</span><span class="sxs-lookup"><span data-stu-id="a9785-111">String</span></span>|<span data-ttu-id="a9785-112">顧客とのインターフェイスとなる派生エンティティの名前。</span><span class="sxs-lookup"><span data-stu-id="a9785-112">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="a9785-113">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a9785-113">emailAddress</span></span>|<span data-ttu-id="a9785-114">String</span><span class="sxs-lookup"><span data-stu-id="a9785-114">String</span></span>|<span data-ttu-id="a9785-115">個人の電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="a9785-115">The email address of the person.</span></span>|
|<span data-ttu-id="a9785-116">id</span><span class="sxs-lookup"><span data-stu-id="a9785-116">id</span></span>|<span data-ttu-id="a9785-117">文字列</span><span class="sxs-lookup"><span data-stu-id="a9785-117">String</span></span>| <span data-ttu-id="a9785-118">派生エンティティの ID。</span><span class="sxs-lookup"><span data-stu-id="a9785-118">The ID for the derived entity.</span></span> <span data-ttu-id="a9785-119">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a9785-119">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9785-120">関係</span><span class="sxs-lookup"><span data-stu-id="a9785-120">Relationships</span></span>
<span data-ttu-id="a9785-121">なし</span><span class="sxs-lookup"><span data-stu-id="a9785-121">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a9785-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a9785-122">JSON representation</span></span>

<span data-ttu-id="a9785-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a9785-123">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingPerson resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
