---
title: timeoffitem リソースの種類
description: timeoff のバージョンを表します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c83a8725a0048a622ed88ec8265be76c30e46cc0
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657855"
---
# <a name="timeoffitem-resource-type"></a><span data-ttu-id="4d22c-103">timeoffitem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4d22c-103">timeOffItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d22c-104">[timeoff](timeoff.md)のバージョンを表します。</span><span class="sxs-lookup"><span data-stu-id="4d22c-104">Represents a version of the [timeOff](timeoff.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4d22c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d22c-105">Properties</span></span>
| <span data-ttu-id="4d22c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d22c-106">Property</span></span>                         | <span data-ttu-id="4d22c-107">型</span><span class="sxs-lookup"><span data-stu-id="4d22c-107">Type</span></span>                    | <span data-ttu-id="4d22c-108">説明</span><span class="sxs-lookup"><span data-stu-id="4d22c-108">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="4d22c-109">timeoff理由 id</span><span class="sxs-lookup"><span data-stu-id="4d22c-109">timeOffReasonId</span></span>               | `string`                  | <span data-ttu-id="4d22c-110">`timeOffReason`のの ID `timeOffItem`。</span><span class="sxs-lookup"><span data-stu-id="4d22c-110">ID of the `timeOffReason` for this `timeOffItem`.</span></span> <span data-ttu-id="4d22c-111">必須。</span><span class="sxs-lookup"><span data-stu-id="4d22c-111">Required.</span></span>     |
| <span data-ttu-id="4d22c-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4d22c-112">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="4d22c-113">の開始日時`timeOffItem`。</span><span class="sxs-lookup"><span data-stu-id="4d22c-113">The start date and time for the `timeOffItem`.</span></span> <span data-ttu-id="4d22c-114">必須。</span><span class="sxs-lookup"><span data-stu-id="4d22c-114">Required.</span></span> <span data-ttu-id="4d22c-115">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="4d22c-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4d22c-116">たとえば、2014年1月1日午前0時 (UTC) は次のようになります。 ' 2014-01-01t00:00: 00z ' のようになります。</span><span class="sxs-lookup"><span data-stu-id="4d22c-116">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="4d22c-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="4d22c-117">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="4d22c-118">の終了日時`timeOffItem`。</span><span class="sxs-lookup"><span data-stu-id="4d22c-118">The end date and time for the `timeOffItem`.</span></span> <span data-ttu-id="4d22c-119">必須。</span><span class="sxs-lookup"><span data-stu-id="4d22c-119">Required.</span></span> <span data-ttu-id="4d22c-120">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="4d22c-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4d22c-121">たとえば、2014年1月1日午前0時 (UTC) は次のようになります。 ' 2014-01-01t00:00: 00z ' のようになります。</span><span class="sxs-lookup"><span data-stu-id="4d22c-121">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="4d22c-122">theme</span><span class="sxs-lookup"><span data-stu-id="4d22c-122">theme</span></span> | `enum`   | <span data-ttu-id="4d22c-123">サポートされている色: 白。水色緑青紫色ピンクイエロー灰色darkBlue;darkGreen;darkPurple;darkPink;darkYellow。</span><span class="sxs-lookup"><span data-stu-id="4d22c-123">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4d22c-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4d22c-124">JSON representation</span></span>

<span data-ttu-id="4d22c-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4d22c-125">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffItem"
}-->
```json
{
  "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
  "startDateTime": "2019-03-11T07:00:00Z",
  "endDateTime": "2019-03-12T07:00:00Z",
  "theme": "pink"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOffItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeoffitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
