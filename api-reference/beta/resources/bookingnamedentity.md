---
title: bookingnamedentity リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: c9dc533360d28fc470a3a00528a20cea1b7ea551
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328193"
---
# <a name="bookingnamedentity-resource-type"></a><span data-ttu-id="62d4f-104">bookingnamedentity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="62d4f-104">bookingNamedEntity resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="62d4f-105">これは、表示名 ( [bookingbusiness](bookingbusiness.md)、 [bookingbusiness](bookingperson.md)、 [bookingbusiness](bookingservice.md)など) を提供する Microsoft の予約エンティティの基本型です。</span><span class="sxs-lookup"><span data-stu-id="62d4f-105">This is a base type for Microsoft Bookings entities that provide a display name, for example, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span></span>

## <a name="properties"></a><span data-ttu-id="62d4f-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62d4f-106">Properties</span></span>
| <span data-ttu-id="62d4f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62d4f-107">Property</span></span>     | <span data-ttu-id="62d4f-108">型</span><span class="sxs-lookup"><span data-stu-id="62d4f-108">Type</span></span>   |<span data-ttu-id="62d4f-109">説明</span><span class="sxs-lookup"><span data-stu-id="62d4f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62d4f-110">displayName</span><span class="sxs-lookup"><span data-stu-id="62d4f-110">displayName</span></span>|<span data-ttu-id="62d4f-111">String</span><span class="sxs-lookup"><span data-stu-id="62d4f-111">String</span></span>|<span data-ttu-id="62d4f-112">顧客とのインターフェイスとなる派生エンティティの名前。</span><span class="sxs-lookup"><span data-stu-id="62d4f-112">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="62d4f-113">id</span><span class="sxs-lookup"><span data-stu-id="62d4f-113">id</span></span>|<span data-ttu-id="62d4f-114">String</span><span class="sxs-lookup"><span data-stu-id="62d4f-114">String</span></span>| <span data-ttu-id="62d4f-115">派生エンティティの ID。</span><span class="sxs-lookup"><span data-stu-id="62d4f-115">The ID for the derived entity.</span></span> <span data-ttu-id="62d4f-116">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="62d4f-116">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62d4f-117">関係</span><span class="sxs-lookup"><span data-stu-id="62d4f-117">Relationships</span></span>
<span data-ttu-id="62d4f-118">なし</span><span class="sxs-lookup"><span data-stu-id="62d4f-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="62d4f-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="62d4f-119">JSON representation</span></span>

<span data-ttu-id="62d4f-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="62d4f-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingNamedEntity"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingNamedEntity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
