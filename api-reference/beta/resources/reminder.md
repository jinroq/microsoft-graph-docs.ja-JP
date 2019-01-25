---
title: アラーム リソースの種類
description: ユーザーの予定表でイベントを通知します。
localization_priority: Normal
ms.openlocfilehash: 88d9cb4f30f60819a606b3b1f3573d16860d9a00
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521034"
---
# <a name="reminder-resource-type"></a><span data-ttu-id="f7c67-103">アラーム リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f7c67-103">reminder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7c67-104">ユーザー[の予定表](calendar.md)の[イベント](event.md)を通知します。</span><span class="sxs-lookup"><span data-stu-id="f7c67-104">A reminder for an [event](event.md) in a user [calendar](calendar.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f7c67-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7c67-105">Properties</span></span>
| <span data-ttu-id="f7c67-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7c67-106">Property</span></span>     | <span data-ttu-id="f7c67-107">型</span><span class="sxs-lookup"><span data-stu-id="f7c67-107">Type</span></span>   |<span data-ttu-id="f7c67-108">説明</span><span class="sxs-lookup"><span data-stu-id="f7c67-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7c67-109">changeKey</span><span class="sxs-lookup"><span data-stu-id="f7c67-109">changeKey</span></span>|<span data-ttu-id="f7c67-110">String</span><span class="sxs-lookup"><span data-stu-id="f7c67-110">String</span></span>|<span data-ttu-id="f7c67-p101">アラームのバージョンを識別します。アラームを変更するたびに **changeKey** も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。</span><span class="sxs-lookup"><span data-stu-id="f7c67-p101">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="f7c67-114">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="f7c67-114">eventEndTime</span></span>|[<span data-ttu-id="f7c67-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="f7c67-115">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="f7c67-116">イベントが終了する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="f7c67-116">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="f7c67-117">eventId</span><span class="sxs-lookup"><span data-stu-id="f7c67-117">eventId</span></span>|<span data-ttu-id="f7c67-118">String</span><span class="sxs-lookup"><span data-stu-id="f7c67-118">String</span></span>|<span data-ttu-id="f7c67-p102">イベントの一意の ID。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f7c67-p102">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="f7c67-121">eventLocation</span><span class="sxs-lookup"><span data-stu-id="f7c67-121">eventLocation</span></span>|[<span data-ttu-id="f7c67-122">Location</span><span class="sxs-lookup"><span data-stu-id="f7c67-122">Location</span></span>](location.md)|<span data-ttu-id="f7c67-123">イベントの場所。</span><span class="sxs-lookup"><span data-stu-id="f7c67-123">The location of the event.</span></span>|
|<span data-ttu-id="f7c67-124">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="f7c67-124">eventStartTime</span></span>|[<span data-ttu-id="f7c67-125">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="f7c67-125">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="f7c67-126">イベントが開始する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="f7c67-126">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="f7c67-127">eventSubject</span><span class="sxs-lookup"><span data-stu-id="f7c67-127">eventSubject</span></span>|<span data-ttu-id="f7c67-128">String</span><span class="sxs-lookup"><span data-stu-id="f7c67-128">String</span></span>|<span data-ttu-id="f7c67-129">イベントの件名行のテキスト。</span><span class="sxs-lookup"><span data-stu-id="f7c67-129">The text of the event's subject line.</span></span>|
|<span data-ttu-id="f7c67-130">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="f7c67-130">eventWebLink</span></span>|<span data-ttu-id="f7c67-131">String</span><span class="sxs-lookup"><span data-stu-id="f7c67-131">String</span></span>|<span data-ttu-id="f7c67-132">Web 上の Outlook でイベントを開く URL。</span><span class="sxs-lookup"><span data-stu-id="f7c67-132">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="f7c67-p103">Web 上の Outlook のメールボックスにログインしている場合、ブラウザーでイベントが開きます。まだブラウザーでログインしていない場合、ログインするように求められます。</span><span class="sxs-lookup"><span data-stu-id="f7c67-p103">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="f7c67-135">この URL には、iFrame 内からアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="f7c67-135">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="f7c67-136">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="f7c67-136">reminderFireTime</span></span>|[<span data-ttu-id="f7c67-137">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="f7c67-137">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="f7c67-138">アラームの発生を設定する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="f7c67-138">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f7c67-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f7c67-139">JSON representation</span></span>

<span data-ttu-id="f7c67-140">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="f7c67-140">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "reminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/reminder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
