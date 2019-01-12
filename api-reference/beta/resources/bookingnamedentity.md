---
title: bookingNamedEntity リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: abd5c9e85357caa6ba6cbbd52d67550a463e36e9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985782"
---
# <a name="bookingnamedentity-resource-type"></a><span data-ttu-id="96430-104">bookingNamedEntity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="96430-104">bookingNamedEntity resource type</span></span>

 > <span data-ttu-id="96430-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="96430-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96430-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96430-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="96430-107">これは、たとえば、表示名を提供する Microsoft の予約のエンティティ、 [bookingBusiness](bookingbusiness.md)、 [bookingPerson](bookingperson.md)、 [bookingService](bookingservice.md)の基本型です。</span><span class="sxs-lookup"><span data-stu-id="96430-107">This is a base type for Microsoft Bookings entities that provide a display name, for example, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span></span>

## <a name="properties"></a><span data-ttu-id="96430-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96430-108">Properties</span></span>
| <span data-ttu-id="96430-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96430-109">Property</span></span>     | <span data-ttu-id="96430-110">種類</span><span class="sxs-lookup"><span data-stu-id="96430-110">Type</span></span>   |<span data-ttu-id="96430-111">説明</span><span class="sxs-lookup"><span data-stu-id="96430-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96430-112">displayName</span><span class="sxs-lookup"><span data-stu-id="96430-112">displayName</span></span>|<span data-ttu-id="96430-113">String</span><span class="sxs-lookup"><span data-stu-id="96430-113">String</span></span>|<span data-ttu-id="96430-114">派生のエンティティは、顧客とのインターフェイスの名前です。</span><span class="sxs-lookup"><span data-stu-id="96430-114">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="96430-115">id</span><span class="sxs-lookup"><span data-stu-id="96430-115">id</span></span>|<span data-ttu-id="96430-116">String</span><span class="sxs-lookup"><span data-stu-id="96430-116">String</span></span>| <span data-ttu-id="96430-117">派生エンティティの ID です。</span><span class="sxs-lookup"><span data-stu-id="96430-117">The ID for the derived entity.</span></span> <span data-ttu-id="96430-118">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96430-118">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96430-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="96430-119">Relationships</span></span>
<span data-ttu-id="96430-120">なし</span><span class="sxs-lookup"><span data-stu-id="96430-120">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="96430-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="96430-121">JSON representation</span></span>

<span data-ttu-id="96430-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="96430-122">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingNamedEntity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
