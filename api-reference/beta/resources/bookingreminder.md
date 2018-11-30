---
title: bookingReminder リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: f5f7b30c296433dd96ffa14a75e3f0286e8a16a1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070674"
---
# <a name="bookingreminder-resource-type"></a><span data-ttu-id="89f55-104">bookingReminder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="89f55-104">bookingReminder resource type</span></span>

 > <span data-ttu-id="89f55-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="89f55-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89f55-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89f55-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="89f55-107">電子メールの事前通知を送信する先を表します。</span><span class="sxs-lookup"><span data-stu-id="89f55-107">Represents when and to whom to send an email reminder.</span></span>


## <a name="properties"></a><span data-ttu-id="89f55-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="89f55-108">Properties</span></span>
| <span data-ttu-id="89f55-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="89f55-109">Property</span></span>     | <span data-ttu-id="89f55-110">型</span><span class="sxs-lookup"><span data-stu-id="89f55-110">Type</span></span>   |<span data-ttu-id="89f55-111">説明</span><span class="sxs-lookup"><span data-stu-id="89f55-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89f55-112">message</span><span class="sxs-lookup"><span data-stu-id="89f55-112">message</span></span>|<span data-ttu-id="89f55-113">String</span><span class="sxs-lookup"><span data-stu-id="89f55-113">String</span></span>|<span data-ttu-id="89f55-114">アラームのメッセージです。</span><span class="sxs-lookup"><span data-stu-id="89f55-114">The message in the reminder.</span></span>|
|<span data-ttu-id="89f55-115">オフセット</span><span class="sxs-lookup"><span data-stu-id="89f55-115">offset</span></span>|<span data-ttu-id="89f55-116">Duration</span><span class="sxs-lookup"><span data-stu-id="89f55-116">Duration</span></span>|<span data-ttu-id="89f55-117">アラームを送信する予定の開始までの時間の量。</span><span class="sxs-lookup"><span data-stu-id="89f55-117">The amount of time before the start of an appointment that the reminder should be sent.</span></span> <span data-ttu-id="89f55-118">それは、 [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式で表されます。</span><span class="sxs-lookup"><span data-stu-id="89f55-118">It's denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="89f55-119">Recipients</span><span class="sxs-lookup"><span data-stu-id="89f55-119">recipients</span></span>|<span data-ttu-id="89f55-120">String</span><span class="sxs-lookup"><span data-stu-id="89f55-120">String</span></span>| <span data-ttu-id="89f55-121">Shouold を受信したユーザー、通知します。</span><span class="sxs-lookup"><span data-stu-id="89f55-121">The persons who shouold receive the reminder.</span></span> <span data-ttu-id="89f55-122">可能な値は、`allAttendees`、`staff`、`customer` です。</span><span class="sxs-lookup"><span data-stu-id="89f55-122">Possible values are: `allAttendees`, `staff`, `customer`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="89f55-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="89f55-123">JSON representation</span></span>

<span data-ttu-id="89f55-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="89f55-124">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingReminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->