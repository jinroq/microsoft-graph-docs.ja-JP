---
title: scheduleInformation リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
ms.openlocfilehash: e84505ee2f30a5b7b52e9d5b589b8bb24d9a4c95
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521909"
---
# <a name="scheduleinformation-resource-type"></a><span data-ttu-id="28919-104">scheduleInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="28919-104">scheduleInformation resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="28919-105">指定された期間内のユーザー、配布リスト、またはリソースの可用性を表します。</span><span class="sxs-lookup"><span data-stu-id="28919-105">Represents the availability of a user, distribution list, or resource for a specified time period.</span></span>

## <a name="properties"></a><span data-ttu-id="28919-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28919-106">Properties</span></span>
| <span data-ttu-id="28919-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28919-107">Property</span></span>     | <span data-ttu-id="28919-108">型</span><span class="sxs-lookup"><span data-stu-id="28919-108">Type</span></span>   |<span data-ttu-id="28919-109">説明</span><span class="sxs-lookup"><span data-stu-id="28919-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28919-110">availabilityView</span><span class="sxs-lookup"><span data-stu-id="28919-110">availabilityView</span></span> |<span data-ttu-id="28919-111">String</span><span class="sxs-lookup"><span data-stu-id="28919-111">String</span></span> |<span data-ttu-id="28919-112">マージされたビュー内のすべての項目の数を表す`scheduleItems`。</span><span class="sxs-lookup"><span data-stu-id="28919-112">Represents a merged view of availability of all the items in `scheduleItems`.</span></span> <span data-ttu-id="28919-113">ビューは、時間帯で構成されています。</span><span class="sxs-lookup"><span data-stu-id="28919-113">The view consists of time slots.</span></span> <span data-ttu-id="28919-114">各時間帯の可用性で示されます。:`0`無料 = `1`= 仮の予定、 `2`= ビジー状態か、`3`外出中 = `4`= の別の場所で作業します。</span><span class="sxs-lookup"><span data-stu-id="28919-114">Availability during each time slot is indicated with: `0`= free, `1`= tentative, `2`= busy, `3`= out of office, `4`= working elsewhere.</span></span>|
|<span data-ttu-id="28919-115">エラー</span><span class="sxs-lookup"><span data-stu-id="28919-115">error</span></span> |[<span data-ttu-id="28919-116">freeBusyError</span><span class="sxs-lookup"><span data-stu-id="28919-116">freeBusyError</span></span>](freebusyerror.md) |<span data-ttu-id="28919-117">エラー情報が、ユーザー、配布リスト、またはリソースの可用性を取得しようとしていますから。</span><span class="sxs-lookup"><span data-stu-id="28919-117">Error information from attempting to get the availability of the user, distribution list, or resource.</span></span> |
|<span data-ttu-id="28919-118">scheduleId</span><span class="sxs-lookup"><span data-stu-id="28919-118">scheduleId</span></span> |<span data-ttu-id="28919-119">String</span><span class="sxs-lookup"><span data-stu-id="28919-119">String</span></span> |<span data-ttu-id="28919-120">ユーザー、配布リスト、または**scheduleInformation**のインスタンスを識別する、リソースの SMTP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="28919-120">An SMTP address of the user, distribution list, or resource, identifying an instance of **scheduleInformation**.</span></span> |
|<span data-ttu-id="28919-121">scheduleItems</span><span class="sxs-lookup"><span data-stu-id="28919-121">scheduleItems</span></span> |<span data-ttu-id="28919-122">[scheduleItem](scheduleitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="28919-122">[scheduleItem](scheduleitem.md) collection</span></span> |<span data-ttu-id="28919-123">ユーザーまたはリソースの可用性を説明する項目が含まれています。</span><span class="sxs-lookup"><span data-stu-id="28919-123">Contains the items that describe the availability of the user or resource.</span></span> |
|<span data-ttu-id="28919-124">workingHours</span><span class="sxs-lookup"><span data-stu-id="28919-124">workingHours</span></span> |[<span data-ttu-id="28919-125">workingHours</span><span class="sxs-lookup"><span data-stu-id="28919-125">workingHours</span></span>](workinghours.md) |<span data-ttu-id="28919-126">ユーザーが働く曜日と、特定のタイムゾーンの時間。</span><span class="sxs-lookup"><span data-stu-id="28919-126">The days of the week and hours in a specific time zone that the user works.</span></span> <span data-ttu-id="28919-127">これらは、ユーザーの[mailboxSettings](mailboxsettings.md)の一部として設定されています。</span><span class="sxs-lookup"><span data-stu-id="28919-127">These are set as part of the user's [mailboxSettings](mailboxsettings.md).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="28919-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="28919-128">JSON representation</span></span>

<span data-ttu-id="28919-129">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="28919-129">The following is a JSON representation of the resource.</span></span>

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
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/scheduleinformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
