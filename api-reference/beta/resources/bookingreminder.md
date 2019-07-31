---
title: bookingReminder リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: a87f504824136fc1f3e3639361e22f78c6719dba
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974137"
---
# <a name="bookingreminder-resource-type"></a><span data-ttu-id="fbafa-104">bookingReminder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fbafa-104">bookingReminder resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="fbafa-105">電子メール通知を送信するタイミングと送信先を表します。</span><span class="sxs-lookup"><span data-stu-id="fbafa-105">Represents when and to whom to send an email reminder.</span></span>


## <a name="properties"></a><span data-ttu-id="fbafa-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fbafa-106">Properties</span></span>
| <span data-ttu-id="fbafa-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fbafa-107">Property</span></span>     | <span data-ttu-id="fbafa-108">型</span><span class="sxs-lookup"><span data-stu-id="fbafa-108">Type</span></span>   |<span data-ttu-id="fbafa-109">説明</span><span class="sxs-lookup"><span data-stu-id="fbafa-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fbafa-110">メッセージ​​</span><span class="sxs-lookup"><span data-stu-id="fbafa-110">message</span></span>|<span data-ttu-id="fbafa-111">String</span><span class="sxs-lookup"><span data-stu-id="fbafa-111">String</span></span>|<span data-ttu-id="fbafa-112">アラームのメッセージ。</span><span class="sxs-lookup"><span data-stu-id="fbafa-112">The message in the reminder.</span></span>|
|<span data-ttu-id="fbafa-113">交互</span><span class="sxs-lookup"><span data-stu-id="fbafa-113">offset</span></span>|<span data-ttu-id="fbafa-114">期間</span><span class="sxs-lookup"><span data-stu-id="fbafa-114">Duration</span></span>|<span data-ttu-id="fbafa-115">予定の開始時刻から事前通知を送信するまでの時間の長さ。</span><span class="sxs-lookup"><span data-stu-id="fbafa-115">The amount of time before the start of an appointment that the reminder should be sent.</span></span> <span data-ttu-id="fbafa-116">[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式で示されています。</span><span class="sxs-lookup"><span data-stu-id="fbafa-116">It's denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="fbafa-117">受信者</span><span class="sxs-lookup"><span data-stu-id="fbafa-117">recipients</span></span>|<span data-ttu-id="fbafa-118">String</span><span class="sxs-lookup"><span data-stu-id="fbafa-118">String</span></span>| <span data-ttu-id="fbafa-119">Shouold がアラームを受信する人物。</span><span class="sxs-lookup"><span data-stu-id="fbafa-119">The persons who shouold receive the reminder.</span></span> <span data-ttu-id="fbafa-120">可能な値は、`allAttendees`、`staff`、`customer` です。</span><span class="sxs-lookup"><span data-stu-id="fbafa-120">Possible values are: `allAttendees`, `staff`, `customer`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fbafa-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fbafa-121">JSON representation</span></span>

<span data-ttu-id="fbafa-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fbafa-122">The following is a JSON representation of the resource.</span></span>

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
