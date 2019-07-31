---
title: shiftActivity リソースの種類
description: Shift でのアクティビティを表します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 8acfb16235c90cf6067ad5fd6c5d8e82ae239f8d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965076"
---
# <a name="shiftactivity-resource-type"></a><span data-ttu-id="2ca40-103">shiftActivity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2ca40-103">shiftActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ca40-104">[Shift](shift.md)でのアクティビティを表します。</span><span class="sxs-lookup"><span data-stu-id="2ca40-104">Represents an activity in a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2ca40-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ca40-105">Properties</span></span>
| <span data-ttu-id="2ca40-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ca40-106">Property</span></span>                         | <span data-ttu-id="2ca40-107">型</span><span class="sxs-lookup"><span data-stu-id="2ca40-107">Type</span></span>                    | <span data-ttu-id="2ca40-108">説明</span><span class="sxs-lookup"><span data-stu-id="2ca40-108">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="2ca40-109">isPaid</span><span class="sxs-lookup"><span data-stu-id="2ca40-109">isPaid</span></span>               | `bool`                  | <span data-ttu-id="2ca40-110">を使用し`microsoft.graph.user`ている間に、活動に対し`shift`てを支払う必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2ca40-110">Indicates whether the `microsoft.graph.user` should be paid for the activity during their `shift`.</span></span> <span data-ttu-id="2ca40-111">必須です。</span><span class="sxs-lookup"><span data-stu-id="2ca40-111">Required.</span></span>    |
| <span data-ttu-id="2ca40-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2ca40-112">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="2ca40-113">の開始日時`shiftActivity`。</span><span class="sxs-lookup"><span data-stu-id="2ca40-113">The start date and time for the `shiftActivity`.</span></span> <span data-ttu-id="2ca40-114">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="2ca40-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2ca40-115">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。</span><span class="sxs-lookup"><span data-stu-id="2ca40-115">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="2ca40-116">必須です。</span><span class="sxs-lookup"><span data-stu-id="2ca40-116">Required.</span></span> |
| <span data-ttu-id="2ca40-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="2ca40-117">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="2ca40-118">の終了日時`shiftActivity`。</span><span class="sxs-lookup"><span data-stu-id="2ca40-118">The end date and time for the `shiftActivity`.</span></span> <span data-ttu-id="2ca40-119">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="2ca40-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2ca40-120">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。</span><span class="sxs-lookup"><span data-stu-id="2ca40-120">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="2ca40-121">必須です。</span><span class="sxs-lookup"><span data-stu-id="2ca40-121">Required.</span></span>    |
| <span data-ttu-id="2ca40-122">code</span><span class="sxs-lookup"><span data-stu-id="2ca40-122">code</span></span>               | `string`                  | <span data-ttu-id="2ca40-123">の顧客定義コード`shiftActivity`。</span><span class="sxs-lookup"><span data-stu-id="2ca40-123">Customer defined code for the `shiftActivity`.</span></span> <span data-ttu-id="2ca40-124">必須です。</span><span class="sxs-lookup"><span data-stu-id="2ca40-124">Required.</span></span>    |
| <span data-ttu-id="2ca40-125">displayName</span><span class="sxs-lookup"><span data-stu-id="2ca40-125">displayName</span></span>               | `string`                  | <span data-ttu-id="2ca40-126">の名前`shiftActivity`。</span><span class="sxs-lookup"><span data-stu-id="2ca40-126">The name of the `shiftActivity`.</span></span> <span data-ttu-id="2ca40-127">必須。</span><span class="sxs-lookup"><span data-stu-id="2ca40-127">Required.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="2ca40-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2ca40-128">JSON representation</span></span>

<span data-ttu-id="2ca40-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2ca40-129">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
