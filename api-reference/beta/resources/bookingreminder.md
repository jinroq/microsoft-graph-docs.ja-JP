---
title: bookingreminder リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 0e5188a5a440134d11404c102b4641fc98cad04f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535484"
---
# <a name="bookingreminder-resource-type"></a><span data-ttu-id="c1d53-104">bookingreminder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c1d53-104">bookingReminder resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="c1d53-105">電子メール通知を送信するタイミングと送信先を表します。</span><span class="sxs-lookup"><span data-stu-id="c1d53-105">Represents when and to whom to send an email reminder.</span></span>


## <a name="properties"></a><span data-ttu-id="c1d53-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1d53-106">Properties</span></span>
| <span data-ttu-id="c1d53-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1d53-107">Property</span></span>     | <span data-ttu-id="c1d53-108">型</span><span class="sxs-lookup"><span data-stu-id="c1d53-108">Type</span></span>   |<span data-ttu-id="c1d53-109">説明</span><span class="sxs-lookup"><span data-stu-id="c1d53-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1d53-110">メッセージ​​</span><span class="sxs-lookup"><span data-stu-id="c1d53-110">message</span></span>|<span data-ttu-id="c1d53-111">String</span><span class="sxs-lookup"><span data-stu-id="c1d53-111">String</span></span>|<span data-ttu-id="c1d53-112">アラームのメッセージ。</span><span class="sxs-lookup"><span data-stu-id="c1d53-112">The message in the reminder.</span></span>|
|<span data-ttu-id="c1d53-113">交互</span><span class="sxs-lookup"><span data-stu-id="c1d53-113">offset</span></span>|<span data-ttu-id="c1d53-114">期間</span><span class="sxs-lookup"><span data-stu-id="c1d53-114">Duration</span></span>|<span data-ttu-id="c1d53-115">予定の開始時刻から事前通知を送信するまでの時間の長さ。</span><span class="sxs-lookup"><span data-stu-id="c1d53-115">The amount of time before the start of an appointment that the reminder should be sent.</span></span> <span data-ttu-id="c1d53-116">[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式で示されています。</span><span class="sxs-lookup"><span data-stu-id="c1d53-116">It's denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="c1d53-117">受信者</span><span class="sxs-lookup"><span data-stu-id="c1d53-117">recipients</span></span>|<span data-ttu-id="c1d53-118">String</span><span class="sxs-lookup"><span data-stu-id="c1d53-118">String</span></span>| <span data-ttu-id="c1d53-119">shouold がアラームを受信する人物。</span><span class="sxs-lookup"><span data-stu-id="c1d53-119">The persons who shouold receive the reminder.</span></span> <span data-ttu-id="c1d53-120">使用可能な値は、`allAttendees`、`staff`、`customer` です。</span><span class="sxs-lookup"><span data-stu-id="c1d53-120">Possible values are: `allAttendees`, `staff`, `customer`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c1d53-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c1d53-121">JSON representation</span></span>

<span data-ttu-id="c1d53-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c1d53-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingReminder"
}-->

```json
{
  "message": "String",
  "offset": "String (timestamp)",
  "recipients": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingReminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingreminder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
