---
title: アラーム リソースの種類
description: ユーザーの予定表でイベントを通知します。
localization_priority: Normal
ms.openlocfilehash: a78c7f82ea0a7db9da45a60de98bb3b1311aaeeb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819965"
---
# <a name="reminder-resource-type"></a><span data-ttu-id="0f06d-103">アラーム リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0f06d-103">reminder resource type</span></span>

> <span data-ttu-id="0f06d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0f06d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f06d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f06d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0f06d-106">ユーザー[の予定表](calendar.md)の[イベント](event.md)を通知します。</span><span class="sxs-lookup"><span data-stu-id="0f06d-106">A reminder for an [event](event.md) in a user [calendar](calendar.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0f06d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f06d-107">Properties</span></span>
| <span data-ttu-id="0f06d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f06d-108">Property</span></span>     | <span data-ttu-id="0f06d-109">種類</span><span class="sxs-lookup"><span data-stu-id="0f06d-109">Type</span></span>   |<span data-ttu-id="0f06d-110">説明</span><span class="sxs-lookup"><span data-stu-id="0f06d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f06d-111">changeKey</span><span class="sxs-lookup"><span data-stu-id="0f06d-111">changeKey</span></span>|<span data-ttu-id="0f06d-112">String</span><span class="sxs-lookup"><span data-stu-id="0f06d-112">String</span></span>|<span data-ttu-id="0f06d-p102">アラームのバージョンを識別します。アラームを変更するたびに **changeKey** も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。</span><span class="sxs-lookup"><span data-stu-id="0f06d-p102">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="0f06d-116">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="0f06d-116">eventEndTime</span></span>|[<span data-ttu-id="0f06d-117">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="0f06d-117">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="0f06d-118">イベントが終了する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="0f06d-118">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="0f06d-119">eventId</span><span class="sxs-lookup"><span data-stu-id="0f06d-119">eventId</span></span>|<span data-ttu-id="0f06d-120">String</span><span class="sxs-lookup"><span data-stu-id="0f06d-120">String</span></span>|<span data-ttu-id="0f06d-p103">イベントの一意の ID。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0f06d-p103">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="0f06d-123">eventLocation</span><span class="sxs-lookup"><span data-stu-id="0f06d-123">eventLocation</span></span>|[<span data-ttu-id="0f06d-124">Location</span><span class="sxs-lookup"><span data-stu-id="0f06d-124">Location</span></span>](location.md)|<span data-ttu-id="0f06d-125">イベントの場所。</span><span class="sxs-lookup"><span data-stu-id="0f06d-125">The location of the event.</span></span>|
|<span data-ttu-id="0f06d-126">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="0f06d-126">eventStartTime</span></span>|[<span data-ttu-id="0f06d-127">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="0f06d-127">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="0f06d-128">イベントが開始する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="0f06d-128">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="0f06d-129">eventSubject</span><span class="sxs-lookup"><span data-stu-id="0f06d-129">eventSubject</span></span>|<span data-ttu-id="0f06d-130">String</span><span class="sxs-lookup"><span data-stu-id="0f06d-130">String</span></span>|<span data-ttu-id="0f06d-131">イベントの件名行のテキスト。</span><span class="sxs-lookup"><span data-stu-id="0f06d-131">The text of the event's subject line.</span></span>|
|<span data-ttu-id="0f06d-132">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="0f06d-132">eventWebLink</span></span>|<span data-ttu-id="0f06d-133">String</span><span class="sxs-lookup"><span data-stu-id="0f06d-133">String</span></span>|<span data-ttu-id="0f06d-134">Web 上の Outlook でイベントを開く URL。</span><span class="sxs-lookup"><span data-stu-id="0f06d-134">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="0f06d-p104">Web 上の Outlook のメールボックスにログインしている場合、ブラウザーでイベントが開きます。まだブラウザーでログインしていない場合、ログインするように求められます。</span><span class="sxs-lookup"><span data-stu-id="0f06d-p104">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="0f06d-137">この URL には、iFrame 内からアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="0f06d-137">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="0f06d-138">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="0f06d-138">reminderFireTime</span></span>|[<span data-ttu-id="0f06d-139">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="0f06d-139">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="0f06d-140">アラームの発生を設定する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="0f06d-140">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f06d-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0f06d-141">JSON representation</span></span>

<span data-ttu-id="0f06d-142">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="0f06d-142">Here is a JSON representation of the resource</span></span>

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
