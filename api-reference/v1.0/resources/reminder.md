---
title: アラーム リソースの種類
description: ユーザーの予定表でイベントを通知します。
localization_priority: Normal
ms.openlocfilehash: e8aa591f078b90249b36d3dc2f666ddac4502461
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815723"
---
# <a name="reminder-resource-type"></a><span data-ttu-id="fd19b-103">アラーム リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fd19b-103">reminder resource type</span></span>

<span data-ttu-id="fd19b-104">ユーザー[の予定表](calendar.md)の[イベント](event.md)を通知します。</span><span class="sxs-lookup"><span data-stu-id="fd19b-104">A reminder for an [event](event.md) in a user [calendar](calendar.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fd19b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd19b-105">Properties</span></span>
| <span data-ttu-id="fd19b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd19b-106">Property</span></span>     | <span data-ttu-id="fd19b-107">種類</span><span class="sxs-lookup"><span data-stu-id="fd19b-107">Type</span></span>   |<span data-ttu-id="fd19b-108">説明</span><span class="sxs-lookup"><span data-stu-id="fd19b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd19b-109">changeKey</span><span class="sxs-lookup"><span data-stu-id="fd19b-109">changeKey</span></span>|<span data-ttu-id="fd19b-110">String</span><span class="sxs-lookup"><span data-stu-id="fd19b-110">String</span></span>|<span data-ttu-id="fd19b-p101">アラームのバージョンを識別します。アラームを変更するたびに **changeKey** も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。</span><span class="sxs-lookup"><span data-stu-id="fd19b-p101">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="fd19b-114">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="fd19b-114">eventEndTime</span></span>|[<span data-ttu-id="fd19b-115">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="fd19b-115">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="fd19b-116">イベントが終了する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="fd19b-116">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="fd19b-117">eventId</span><span class="sxs-lookup"><span data-stu-id="fd19b-117">eventId</span></span>|<span data-ttu-id="fd19b-118">String</span><span class="sxs-lookup"><span data-stu-id="fd19b-118">String</span></span>|<span data-ttu-id="fd19b-p102">イベントの一意の ID。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fd19b-p102">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="fd19b-121">eventLocation</span><span class="sxs-lookup"><span data-stu-id="fd19b-121">eventLocation</span></span>|[<span data-ttu-id="fd19b-122">Location</span><span class="sxs-lookup"><span data-stu-id="fd19b-122">Location</span></span>](location.md)|<span data-ttu-id="fd19b-123">イベントの場所。</span><span class="sxs-lookup"><span data-stu-id="fd19b-123">The location of the event.</span></span>|
|<span data-ttu-id="fd19b-124">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="fd19b-124">eventStartTime</span></span>|[<span data-ttu-id="fd19b-125">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="fd19b-125">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="fd19b-126">イベントが開始する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="fd19b-126">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="fd19b-127">eventSubject</span><span class="sxs-lookup"><span data-stu-id="fd19b-127">eventSubject</span></span>|<span data-ttu-id="fd19b-128">String</span><span class="sxs-lookup"><span data-stu-id="fd19b-128">String</span></span>|<span data-ttu-id="fd19b-129">イベントの件名行のテキスト。</span><span class="sxs-lookup"><span data-stu-id="fd19b-129">The text of the event's subject line.</span></span>|
|<span data-ttu-id="fd19b-130">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="fd19b-130">eventWebLink</span></span>|<span data-ttu-id="fd19b-131">String</span><span class="sxs-lookup"><span data-stu-id="fd19b-131">String</span></span>|<span data-ttu-id="fd19b-132">Web 上の Outlook でイベントを開く URL。</span><span class="sxs-lookup"><span data-stu-id="fd19b-132">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="fd19b-p103">Web 上の Outlook のメールボックスにログインしている場合、ブラウザーでイベントが開きます。まだブラウザーでログインしていない場合、ログインするように求められます。</span><span class="sxs-lookup"><span data-stu-id="fd19b-p103">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="fd19b-135">この URL には、iFrame 内からアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="fd19b-135">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="fd19b-136">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="fd19b-136">reminderFireTime</span></span>|[<span data-ttu-id="fd19b-137">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="fd19b-137">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="fd19b-138">アラームの発生を設定する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="fd19b-138">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fd19b-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fd19b-139">JSON representation</span></span>

<span data-ttu-id="fd19b-140">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="fd19b-140">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reminder"
}-->

```json
{
  "changeKey": "string",
  "eventEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventId": "string",
  "eventLocation": {"@odata.type": "microsoft.graph.location"},
  "eventStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventSubject": "string",
  "eventWebLink": "string",
  "reminderFireTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
