---
title: "\"佐々木 ftitem\" リソースの種類"
description: "\"佐々木 ftitem\" は、シフトのバージョンを表します。"
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7ff829ca0f43124404b4b99b048c9919368b6009
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657708"
---
# <a name="shiftitem-resource-type"></a><span data-ttu-id="cf030-103">"佐々木 ftitem" リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cf030-103">shiftItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf030-104">[シフト](shift.md)のバージョンを表します。</span><span class="sxs-lookup"><span data-stu-id="cf030-104">Represents a version of a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cf030-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf030-105">Properties</span></span>
| <span data-ttu-id="cf030-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf030-106">Property</span></span>                         | <span data-ttu-id="cf030-107">型</span><span class="sxs-lookup"><span data-stu-id="cf030-107">Type</span></span>                    | <span data-ttu-id="cf030-108">説明</span><span class="sxs-lookup"><span data-stu-id="cf030-108">Description</span></span>                                                                             |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="cf030-109">notes</span><span class="sxs-lookup"><span data-stu-id="cf030-109">notes</span></span>               | `string`                  | <span data-ttu-id="cf030-110">のメモ`shiftItem`。</span><span class="sxs-lookup"><span data-stu-id="cf030-110">The notes for the `shiftItem`.</span></span>      |
| <span data-ttu-id="cf030-111">displayName</span><span class="sxs-lookup"><span data-stu-id="cf030-111">displayName</span></span>               | `string`                  | <span data-ttu-id="cf030-112">の名前`shiftItem`。</span><span class="sxs-lookup"><span data-stu-id="cf030-112">The name of the `shiftItem`.</span></span> |
| <span data-ttu-id="cf030-113">startDateTime</span><span class="sxs-lookup"><span data-stu-id="cf030-113">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="cf030-114">の開始日時`shiftItem`。</span><span class="sxs-lookup"><span data-stu-id="cf030-114">The start date and time for the `shiftItem`.</span></span> <span data-ttu-id="cf030-115">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="cf030-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cf030-116">たとえば、2014年1月1日午前0時 (UTC) は次のようになります。 ' 2014-01-01t00:00: 00z ' のようになります。</span><span class="sxs-lookup"><span data-stu-id="cf030-116">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="cf030-117">必須。</span><span class="sxs-lookup"><span data-stu-id="cf030-117">Required.</span></span> |
| <span data-ttu-id="cf030-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="cf030-118">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="cf030-119">の終了日時`shiftItem`。</span><span class="sxs-lookup"><span data-stu-id="cf030-119">The end date and time for the `shiftItem`.</span></span> <span data-ttu-id="cf030-120">必須。</span><span class="sxs-lookup"><span data-stu-id="cf030-120">Required.</span></span> <span data-ttu-id="cf030-121">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="cf030-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cf030-122">たとえば、2014年1月1日午前0時 (UTC) は次のようになります。 ' 2014-01-01t00:00: 00z ' のようになります。</span><span class="sxs-lookup"><span data-stu-id="cf030-122">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="cf030-123">theme</span><span class="sxs-lookup"><span data-stu-id="cf030-123">theme</span></span> | `enum`   |    |  |  | <span data-ttu-id="cf030-124">サポートされている色: 白。水色緑青紫色ピンクイエロー灰色darkBlue;darkGreen;darkPurple;darkPink;darkYellow。</span><span class="sxs-lookup"><span data-stu-id="cf030-124">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |
| <span data-ttu-id="cf030-125">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="cf030-125">activities</span></span>    | `collection([shiftActivity](shiftactivity.md))`    | <span data-ttu-id="cf030-126">従業員がいつ、どのような時間帯に勤務しているかを詳細に説明できる、シフトの増分部分。</span><span class="sxs-lookup"><span data-stu-id="cf030-126">An incremental part of a shift which can cover details of when and where an employee is during their shift.</span></span> <span data-ttu-id="cf030-127">たとえば、割り当て、またはスケジュールされた休憩またはランチ。</span><span class="sxs-lookup"><span data-stu-id="cf030-127">For example, an assignment or a scheduled break or lunch.</span></span> <span data-ttu-id="cf030-128">必須。</span><span class="sxs-lookup"><span data-stu-id="cf030-128">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cf030-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cf030-129">JSON representation</span></span>

<span data-ttu-id="cf030-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cf030-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftItem"
}-->
```json
{
  "displayName": "Day shift",
  "notes": "Please do inventory as part of your shift.",
  "startDateTime": "2019-03-11T15:00:00Z",
  "endDateTime": "2019-03-12T00:00:00Z",
  "theme": "blue",
  "activities": [
    {
      "isPaid": true,
      "startDateTime": "2019-03-11T15:00:00Z",
      "endDateTime": "2019-03-11T15:15:00Z",
      "code": "",
      "displayName": "Lunch"
    }
  ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shiftItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/shiftitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
