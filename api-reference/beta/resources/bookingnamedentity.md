---
title: bookingNamedEntity リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 1cee769181fdf8dce694050cdbc2658fdf29ece4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515322"
---
# <a name="bookingnamedentity-resource-type"></a><span data-ttu-id="e29d4-104">bookingNamedEntity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e29d4-104">bookingNamedEntity resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="e29d4-105">これは、たとえば、表示名を提供する Microsoft の予約のエンティティ、 [bookingBusiness](bookingbusiness.md)、 [bookingPerson](bookingperson.md)、 [bookingService](bookingservice.md)の基本型です。</span><span class="sxs-lookup"><span data-stu-id="e29d4-105">This is a base type for Microsoft Bookings entities that provide a display name, for example, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e29d4-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e29d4-106">Properties</span></span>
| <span data-ttu-id="e29d4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e29d4-107">Property</span></span>     | <span data-ttu-id="e29d4-108">型</span><span class="sxs-lookup"><span data-stu-id="e29d4-108">Type</span></span>   |<span data-ttu-id="e29d4-109">説明</span><span class="sxs-lookup"><span data-stu-id="e29d4-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e29d4-110">displayName</span><span class="sxs-lookup"><span data-stu-id="e29d4-110">displayName</span></span>|<span data-ttu-id="e29d4-111">String</span><span class="sxs-lookup"><span data-stu-id="e29d4-111">String</span></span>|<span data-ttu-id="e29d4-112">派生のエンティティは、顧客とのインターフェイスの名前です。</span><span class="sxs-lookup"><span data-stu-id="e29d4-112">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="e29d4-113">id</span><span class="sxs-lookup"><span data-stu-id="e29d4-113">id</span></span>|<span data-ttu-id="e29d4-114">String</span><span class="sxs-lookup"><span data-stu-id="e29d4-114">String</span></span>| <span data-ttu-id="e29d4-115">派生エンティティの ID です。</span><span class="sxs-lookup"><span data-stu-id="e29d4-115">The ID for the derived entity.</span></span> <span data-ttu-id="e29d4-116">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e29d4-116">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e29d4-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e29d4-117">Relationships</span></span>
<span data-ttu-id="e29d4-118">なし</span><span class="sxs-lookup"><span data-stu-id="e29d4-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e29d4-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e29d4-119">JSON representation</span></span>

<span data-ttu-id="e29d4-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e29d4-120">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingnamedentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
