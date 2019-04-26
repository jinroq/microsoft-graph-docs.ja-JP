---
title: bookingreminder リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 18265a9d9e86b79706b6a268df3b8512b7b65111
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328203"
---
# <a name="bookingreminder-resource-type"></a><span data-ttu-id="de206-104">bookingreminder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="de206-104">bookingReminder resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="de206-105">電子メール通知を送信するタイミングと送信先を表します。</span><span class="sxs-lookup"><span data-stu-id="de206-105">Represents when and to whom to send an email reminder.</span></span>


## <a name="properties"></a><span data-ttu-id="de206-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de206-106">Properties</span></span>
| <span data-ttu-id="de206-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de206-107">Property</span></span>     | <span data-ttu-id="de206-108">型</span><span class="sxs-lookup"><span data-stu-id="de206-108">Type</span></span>   |<span data-ttu-id="de206-109">説明</span><span class="sxs-lookup"><span data-stu-id="de206-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de206-110">メッセージ​​</span><span class="sxs-lookup"><span data-stu-id="de206-110">message</span></span>|<span data-ttu-id="de206-111">String</span><span class="sxs-lookup"><span data-stu-id="de206-111">String</span></span>|<span data-ttu-id="de206-112">アラームのメッセージ。</span><span class="sxs-lookup"><span data-stu-id="de206-112">The message in the reminder.</span></span>|
|<span data-ttu-id="de206-113">交互</span><span class="sxs-lookup"><span data-stu-id="de206-113">offset</span></span>|<span data-ttu-id="de206-114">期間</span><span class="sxs-lookup"><span data-stu-id="de206-114">Duration</span></span>|<span data-ttu-id="de206-115">予定の開始時刻から事前通知を送信するまでの時間の長さ。</span><span class="sxs-lookup"><span data-stu-id="de206-115">The amount of time before the start of an appointment that the reminder should be sent.</span></span> <span data-ttu-id="de206-116">[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式で示されています。</span><span class="sxs-lookup"><span data-stu-id="de206-116">It's denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="de206-117">受信者</span><span class="sxs-lookup"><span data-stu-id="de206-117">recipients</span></span>|<span data-ttu-id="de206-118">String</span><span class="sxs-lookup"><span data-stu-id="de206-118">String</span></span>| <span data-ttu-id="de206-119">shouold がアラームを受信する人物。</span><span class="sxs-lookup"><span data-stu-id="de206-119">The persons who shouold receive the reminder.</span></span> <span data-ttu-id="de206-120">可能な値は、`allAttendees`、`staff`、`customer` です。</span><span class="sxs-lookup"><span data-stu-id="de206-120">Possible values are: `allAttendees`, `staff`, `customer`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="de206-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="de206-121">JSON representation</span></span>

<span data-ttu-id="de206-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="de206-122">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
