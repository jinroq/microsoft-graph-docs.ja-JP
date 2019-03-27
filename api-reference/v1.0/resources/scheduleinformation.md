---
title: scheduleinformation リソースの種類
description: 指定した期間のユーザー、配布リスト、またはリソースの空き時間情報を表します。
localization_priority: Normal
ms.openlocfilehash: a19689eeafe9723cdadeb6147700933ab171637c
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/27/2019
ms.locfileid: "30926615"
---
# <a name="scheduleinformation-resource-type"></a><span data-ttu-id="84263-103">scheduleinformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="84263-103">scheduleInformation resource type</span></span>

<span data-ttu-id="84263-104">指定した期間のユーザー、配布リスト、またはリソース (会議室または備品) の空き時間情報を表します。</span><span class="sxs-lookup"><span data-stu-id="84263-104">Represents the availability of a user, distribution list, or resource (room or equipment) for a specified time period.</span></span>

## <a name="properties"></a><span data-ttu-id="84263-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84263-105">Properties</span></span>
| <span data-ttu-id="84263-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84263-106">Property</span></span>     | <span data-ttu-id="84263-107">型</span><span class="sxs-lookup"><span data-stu-id="84263-107">Type</span></span>   |<span data-ttu-id="84263-108">説明</span><span class="sxs-lookup"><span data-stu-id="84263-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84263-109">availabilityView</span><span class="sxs-lookup"><span data-stu-id="84263-109">availabilityView</span></span> |<span data-ttu-id="84263-110">String</span><span class="sxs-lookup"><span data-stu-id="84263-110">String</span></span> |<span data-ttu-id="84263-111">のすべてのアイテムの利用可能時間のマージさ`scheduleItems`れたビューを表します。</span><span class="sxs-lookup"><span data-stu-id="84263-111">Represents a merged view of availability of all the items in `scheduleItems`.</span></span> <span data-ttu-id="84263-112">ビューは、時間帯で構成されます。</span><span class="sxs-lookup"><span data-stu-id="84263-112">The view consists of time slots.</span></span> <span data-ttu-id="84263-113">各時間帯の可用性は、次の`0`ように表示`1`されます`2`。 = free `3`、= 仮設、= `4`busy、out 不在、または他の場所で動作します。</span><span class="sxs-lookup"><span data-stu-id="84263-113">Availability during each time slot is indicated with: `0`= free, `1`= tentative, `2`= busy, `3`= out of office, `4`= working elsewhere.</span></span>|
|<span data-ttu-id="84263-114">エラー</span><span class="sxs-lookup"><span data-stu-id="84263-114">error</span></span> |[<span data-ttu-id="84263-115">freeBusyError</span><span class="sxs-lookup"><span data-stu-id="84263-115">freeBusyError</span></span>](freebusyerror.md) |<span data-ttu-id="84263-116">ユーザー、配布リスト、またはリソースの空き時間情報を取得しようとしたエラー情報。</span><span class="sxs-lookup"><span data-stu-id="84263-116">Error information from attempting to get the availability of the user, distribution list, or resource.</span></span> |
|<span data-ttu-id="84263-117">scheduleId</span><span class="sxs-lookup"><span data-stu-id="84263-117">scheduleId</span></span> |<span data-ttu-id="84263-118">String</span><span class="sxs-lookup"><span data-stu-id="84263-118">String</span></span> |<span data-ttu-id="84263-119">**scheduleinformation**のインスタンスを識別する、ユーザー、配布リスト、またはリソースの SMTP アドレス。</span><span class="sxs-lookup"><span data-stu-id="84263-119">An SMTP address of the user, distribution list, or resource, identifying an instance of **scheduleInformation**.</span></span> |
|<span data-ttu-id="84263-120">scheduleitems</span><span class="sxs-lookup"><span data-stu-id="84263-120">scheduleItems</span></span> |<span data-ttu-id="84263-121">[scheduleitem](scheduleitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="84263-121">[scheduleItem](scheduleitem.md) collection</span></span> |<span data-ttu-id="84263-122">ユーザーまたはリソースの空き時間情報を示す項目を含みます。</span><span class="sxs-lookup"><span data-stu-id="84263-122">Contains the items that describe the availability of the user or resource.</span></span> |
|<span data-ttu-id="84263-123">workingHours</span><span class="sxs-lookup"><span data-stu-id="84263-123">workingHours</span></span> |[<span data-ttu-id="84263-124">workingHours</span><span class="sxs-lookup"><span data-stu-id="84263-124">workingHours</span></span>](workinghours.md) |<span data-ttu-id="84263-125">ユーザーが働く曜日と、特定のタイムゾーンの時間。</span><span class="sxs-lookup"><span data-stu-id="84263-125">The days of the week and hours in a specific time zone that the user works.</span></span> <span data-ttu-id="84263-126">これらは、ユーザーの[mailboxSettings](mailboxsettings.md)の一部として設定されます。</span><span class="sxs-lookup"><span data-stu-id="84263-126">These are set as part of the user's [mailboxSettings](mailboxsettings.md).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="84263-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="84263-127">JSON representation</span></span>

<span data-ttu-id="84263-128">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="84263-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scheduleInformation"
}-->

```json
{
  "availabilityView": "String",
  "error": {"@odata.type": "microsoft.graph.freeBusyError"},
  "scheduleId": "String",
  "scheduleItems": [{"@odata.type": "microsoft.graph.scheduleItem"}],
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scheduleInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->