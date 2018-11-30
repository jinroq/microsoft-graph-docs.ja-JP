---
title: bookingNamedEntity リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: 1d82fcf6fcf7ffad6e60baea3f3e1118ec60345d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066944"
---
# <a name="bookingnamedentity-resource-type"></a><span data-ttu-id="bd044-104">bookingNamedEntity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bd044-104">bookingNamedEntity resource type</span></span>

 > <span data-ttu-id="bd044-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bd044-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd044-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd044-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="bd044-107">これは、たとえば、表示名を提供する Microsoft の予約のエンティティ、 [bookingBusiness](bookingbusiness.md)、 [bookingPerson](bookingperson.md)、 [bookingService](bookingservice.md)の基本型です。</span><span class="sxs-lookup"><span data-stu-id="bd044-107">This is a base type for Microsoft Bookings entities that provide a display name, for example, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bd044-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bd044-108">Properties</span></span>
| <span data-ttu-id="bd044-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bd044-109">Property</span></span>     | <span data-ttu-id="bd044-110">型</span><span class="sxs-lookup"><span data-stu-id="bd044-110">Type</span></span>   |<span data-ttu-id="bd044-111">説明</span><span class="sxs-lookup"><span data-stu-id="bd044-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd044-112">displayName</span><span class="sxs-lookup"><span data-stu-id="bd044-112">displayName</span></span>|<span data-ttu-id="bd044-113">String</span><span class="sxs-lookup"><span data-stu-id="bd044-113">String</span></span>|<span data-ttu-id="bd044-114">派生のエンティティは、顧客とのインターフェイスの名前です。</span><span class="sxs-lookup"><span data-stu-id="bd044-114">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="bd044-115">id</span><span class="sxs-lookup"><span data-stu-id="bd044-115">id</span></span>|<span data-ttu-id="bd044-116">String</span><span class="sxs-lookup"><span data-stu-id="bd044-116">String</span></span>| <span data-ttu-id="bd044-117">派生エンティティの ID です。</span><span class="sxs-lookup"><span data-stu-id="bd044-117">The ID for the derived entity.</span></span> <span data-ttu-id="bd044-118">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="bd044-118">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd044-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bd044-119">Relationships</span></span>
<span data-ttu-id="bd044-120">なし</span><span class="sxs-lookup"><span data-stu-id="bd044-120">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="bd044-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bd044-121">JSON representation</span></span>

<span data-ttu-id="bd044-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bd044-122">The following is a JSON representation of the resource.</span></span>

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