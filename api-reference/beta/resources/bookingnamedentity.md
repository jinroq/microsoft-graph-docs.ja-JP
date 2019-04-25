---
title: bookingnamedentity リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 1cee769181fdf8dce694050cdbc2658fdf29ece4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535455"
---
# <a name="bookingnamedentity-resource-type"></a><span data-ttu-id="e2dad-104">bookingnamedentity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e2dad-104">bookingNamedEntity resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="e2dad-105">これは、表示名 ( [bookingbusiness](bookingbusiness.md)、 [bookingbusiness](bookingperson.md)、 [bookingbusiness](bookingservice.md)など) を提供する Microsoft の予約エンティティの基本型です。</span><span class="sxs-lookup"><span data-stu-id="e2dad-105">This is a base type for Microsoft Bookings entities that provide a display name, for example, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e2dad-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2dad-106">Properties</span></span>
| <span data-ttu-id="e2dad-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2dad-107">Property</span></span>     | <span data-ttu-id="e2dad-108">型</span><span class="sxs-lookup"><span data-stu-id="e2dad-108">Type</span></span>   |<span data-ttu-id="e2dad-109">説明</span><span class="sxs-lookup"><span data-stu-id="e2dad-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2dad-110">displayName</span><span class="sxs-lookup"><span data-stu-id="e2dad-110">displayName</span></span>|<span data-ttu-id="e2dad-111">String</span><span class="sxs-lookup"><span data-stu-id="e2dad-111">String</span></span>|<span data-ttu-id="e2dad-112">顧客とのインターフェイスとなる派生エンティティの名前。</span><span class="sxs-lookup"><span data-stu-id="e2dad-112">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="e2dad-113">id</span><span class="sxs-lookup"><span data-stu-id="e2dad-113">id</span></span>|<span data-ttu-id="e2dad-114">String</span><span class="sxs-lookup"><span data-stu-id="e2dad-114">String</span></span>| <span data-ttu-id="e2dad-115">派生エンティティの ID。</span><span class="sxs-lookup"><span data-stu-id="e2dad-115">The ID for the derived entity.</span></span> <span data-ttu-id="e2dad-116">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="e2dad-116">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2dad-117">関係</span><span class="sxs-lookup"><span data-stu-id="e2dad-117">Relationships</span></span>
<span data-ttu-id="e2dad-118">なし</span><span class="sxs-lookup"><span data-stu-id="e2dad-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e2dad-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e2dad-119">JSON representation</span></span>

<span data-ttu-id="e2dad-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e2dad-120">The following is a JSON representation of the resource.</span></span>

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
