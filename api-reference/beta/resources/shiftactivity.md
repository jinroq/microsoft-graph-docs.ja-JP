---
title: shiftActivity リソースの種類
description: shift でのアクティビティを表します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0a5b877c2c24d1764e9badb44dab1f25143c2dce
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657526"
---
# <a name="shiftactivity-resource-type"></a><span data-ttu-id="ba75b-103">shiftActivity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ba75b-103">shiftActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba75b-104">[shift](shift.md)でのアクティビティを表します。</span><span class="sxs-lookup"><span data-stu-id="ba75b-104">Represents an activity in a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ba75b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba75b-105">Properties</span></span>
| <span data-ttu-id="ba75b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba75b-106">Property</span></span>                         | <span data-ttu-id="ba75b-107">型</span><span class="sxs-lookup"><span data-stu-id="ba75b-107">Type</span></span>                    | <span data-ttu-id="ba75b-108">説明</span><span class="sxs-lookup"><span data-stu-id="ba75b-108">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="ba75b-109">ispaid</span><span class="sxs-lookup"><span data-stu-id="ba75b-109">isPaid</span></span>               | `bool`                  | <span data-ttu-id="ba75b-110">を使用し`microsoft.graph.user`ている間に、活動に対し`shift`てを支払う必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ba75b-110">Indicates whether the `microsoft.graph.user` should be paid for the activity during their `shift`.</span></span> <span data-ttu-id="ba75b-111">必須。</span><span class="sxs-lookup"><span data-stu-id="ba75b-111">Required.</span></span>    |
| <span data-ttu-id="ba75b-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ba75b-112">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="ba75b-113">の開始日時`shiftActivity`。</span><span class="sxs-lookup"><span data-stu-id="ba75b-113">The start date and time for the `shiftActivity`.</span></span> <span data-ttu-id="ba75b-114">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="ba75b-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ba75b-115">たとえば、2014年1月1日午前0時 (UTC) は次のようになります。 ' 2014-01-01t00:00: 00z ' のようになります。</span><span class="sxs-lookup"><span data-stu-id="ba75b-115">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="ba75b-116">必須。</span><span class="sxs-lookup"><span data-stu-id="ba75b-116">Required.</span></span> |
| <span data-ttu-id="ba75b-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ba75b-117">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="ba75b-118">の終了日時`shiftActivity`。</span><span class="sxs-lookup"><span data-stu-id="ba75b-118">The end date and time for the `shiftActivity`.</span></span> <span data-ttu-id="ba75b-119">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="ba75b-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ba75b-120">たとえば、2014年1月1日午前0時 (UTC) は次のようになります。 ' 2014-01-01t00:00: 00z ' のようになります。</span><span class="sxs-lookup"><span data-stu-id="ba75b-120">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="ba75b-121">必須。</span><span class="sxs-lookup"><span data-stu-id="ba75b-121">Required.</span></span>    |
| <span data-ttu-id="ba75b-122">code</span><span class="sxs-lookup"><span data-stu-id="ba75b-122">code</span></span>               | `string`                  | <span data-ttu-id="ba75b-123">の顧客定義コード`shiftActivity`。</span><span class="sxs-lookup"><span data-stu-id="ba75b-123">Customer defined code for the `shiftActivity`.</span></span> <span data-ttu-id="ba75b-124">必須。</span><span class="sxs-lookup"><span data-stu-id="ba75b-124">Required.</span></span>    |
| <span data-ttu-id="ba75b-125">displayName</span><span class="sxs-lookup"><span data-stu-id="ba75b-125">displayName</span></span>               | `string`                  | <span data-ttu-id="ba75b-126">の名前`shiftActivity`。</span><span class="sxs-lookup"><span data-stu-id="ba75b-126">The name of the `shiftActivity`.</span></span> <span data-ttu-id="ba75b-127">必須。</span><span class="sxs-lookup"><span data-stu-id="ba75b-127">Required.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="ba75b-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ba75b-128">JSON representation</span></span>

<span data-ttu-id="ba75b-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ba75b-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftActivity"
}-->
```json
{
  "isPaid": true,
  "startDateTime": "2019-03-11T15:00:00Z",
  "endDateTime": "2019-03-11T15:15:00Z",
  "code": "",
  "displayName": "Lunch"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shiftActivity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/shiftactivity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
