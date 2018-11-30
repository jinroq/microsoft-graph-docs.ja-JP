---
title: onlineMeeting リソースの種類
description: 結合 URL、出席者リスト、説明など、会議に関する情報をキャプチャします。
ms.openlocfilehash: 73e45f7f2c04df469f2c2fb0faf1c8a0f8680a64
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067419"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="fd2da-103">onlineMeeting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fd2da-103">onlineMeeting resource type</span></span>

> <span data-ttu-id="fd2da-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fd2da-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd2da-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd2da-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fd2da-106">結合 URL、出席者リスト、説明など、会議に関する情報をキャプチャします。</span><span class="sxs-lookup"><span data-stu-id="fd2da-106">Captures information about the meeting, including the join URL, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="fd2da-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="fd2da-107">Methods</span></span>

| <span data-ttu-id="fd2da-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="fd2da-108">Method</span></span>         | <span data-ttu-id="fd2da-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fd2da-109">Return Type</span></span> | <span data-ttu-id="fd2da-110">説明</span><span class="sxs-lookup"><span data-stu-id="fd2da-110">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="fd2da-111">OnlineMeeting を取得します。</span><span class="sxs-lookup"><span data-stu-id="fd2da-111">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="fd2da-112">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="fd2da-112">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="fd2da-113">OnlineMeeting オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fd2da-113">Read properties and relationships of onlineMeeting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fd2da-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd2da-114">Properties</span></span>

| <span data-ttu-id="fd2da-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd2da-115">Property</span></span>                  | <span data-ttu-id="fd2da-116">型</span><span class="sxs-lookup"><span data-stu-id="fd2da-116">Type</span></span>                                                   | <span data-ttu-id="fd2da-117">説明</span><span class="sxs-lookup"><span data-stu-id="fd2da-117">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="fd2da-118">accessLevel</span><span class="sxs-lookup"><span data-stu-id="fd2da-118">accessLevel</span></span>               | <span data-ttu-id="fd2da-119">String</span><span class="sxs-lookup"><span data-stu-id="fd2da-119">String</span></span>                                                 | <span data-ttu-id="fd2da-120">オンラインの会議出席依頼の受付を制御するアクセス レベルです。</span><span class="sxs-lookup"><span data-stu-id="fd2da-120">The access level that controls admission to the online meeting.</span></span> <span data-ttu-id="fd2da-121">可能な値は、`everyone`、`invited`、`locked`、`sameEnterprise`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="fd2da-121">Possible values are: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`.</span></span> |
| <span data-ttu-id="fd2da-122">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="fd2da-122">audioConferencing</span></span>         | [<span data-ttu-id="fd2da-123">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="fd2da-123">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="fd2da-124">OnlineMeeting には、電話アクセス情報を表します。</span><span class="sxs-lookup"><span data-stu-id="fd2da-124">Represents phone access information for an onlineMeeting.</span></span> |
| <span data-ttu-id="fd2da-125">canceledDateTime</span><span class="sxs-lookup"><span data-stu-id="fd2da-125">canceledDateTime</span></span>          | <span data-ttu-id="fd2da-126">DateTime</span><span class="sxs-lookup"><span data-stu-id="fd2da-126">DateTime</span></span>                                               | <span data-ttu-id="fd2da-127">会議がキャンセルされた時刻。</span><span class="sxs-lookup"><span data-stu-id="fd2da-127">The time when the meeting was canceled.</span></span> |
| <span data-ttu-id="fd2da-128">chatInfo</span><span class="sxs-lookup"><span data-stu-id="fd2da-128">chatInfo</span></span>                  | [<span data-ttu-id="fd2da-129">chatInfo</span><span class="sxs-lookup"><span data-stu-id="fd2da-129">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="fd2da-130">この会議に関連付けられているチャット。</span><span class="sxs-lookup"><span data-stu-id="fd2da-130">The chat associated with this meeting.</span></span> |
| <span data-ttu-id="fd2da-131">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="fd2da-131">creationDateTime</span></span>          | <span data-ttu-id="fd2da-132">DateTime</span><span class="sxs-lookup"><span data-stu-id="fd2da-132">DateTime</span></span>                                               | <span data-ttu-id="fd2da-133">ミーティングが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="fd2da-133">The time when the meeting was created.</span></span> <span data-ttu-id="fd2da-134">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fd2da-134">Readonly.</span></span>
| <span data-ttu-id="fd2da-135">endDateTime</span><span class="sxs-lookup"><span data-stu-id="fd2da-135">endDateTime</span></span>               | <span data-ttu-id="fd2da-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="fd2da-136">DateTime</span></span>                                               | <span data-ttu-id="fd2da-137">会議の終了時間です。</span><span class="sxs-lookup"><span data-stu-id="fd2da-137">End time of the meeting.</span></span> |
| <span data-ttu-id="fd2da-138">entryExitAnnouncement</span><span class="sxs-lookup"><span data-stu-id="fd2da-138">entryExitAnnouncement</span></span>     | <span data-ttu-id="fd2da-139">ブール値</span><span class="sxs-lookup"><span data-stu-id="fd2da-139">Boolean</span></span>                                                | <span data-ttu-id="fd2da-140">オンライン会議の出席のお知らせ状態です。</span><span class="sxs-lookup"><span data-stu-id="fd2da-140">The attendance announcements status for the online meeting.</span></span> <span data-ttu-id="fd2da-141">出勤のお知らせを有効にすると、オンライン会議、発表 participantswho 結合の名前、会議のオーディオを使用します。</span><span class="sxs-lookup"><span data-stu-id="fd2da-141">When attendance announcements are enabled, the online meeting will announce the names of the participantswho join the meeting through audio.</span></span> |
| <span data-ttu-id="fd2da-142">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fd2da-142">expirationDateTime</span></span>        | <span data-ttu-id="fd2da-143">DateTime</span><span class="sxs-lookup"><span data-stu-id="fd2da-143">DateTime</span></span>                                               | <span data-ttu-id="fd2da-144">絶対の世界協定時刻 (UTC) の日付と時刻は、オンライン会議を削除できます。</span><span class="sxs-lookup"><span data-stu-id="fd2da-144">The absolute Coordinated Universal Time (UTC) date and time after which the online meeting can be deleted.</span></span> <span data-ttu-id="fd2da-145">曜日と時間は、1 年前に、および現在の日付と、サーバー上の時刻の後 10 年間する必要があります。</span><span class="sxs-lookup"><span data-stu-id="fd2da-145">The day and time must be between one year before, and ten years after, the current date and time on the server.</span></span> |
| <span data-ttu-id="fd2da-146">id</span><span class="sxs-lookup"><span data-stu-id="fd2da-146">id</span></span>                        | <span data-ttu-id="fd2da-147">String</span><span class="sxs-lookup"><span data-stu-id="fd2da-147">String</span></span>                                                 | <span data-ttu-id="fd2da-148">オンライン会議に関連付けられている ID です。</span><span class="sxs-lookup"><span data-stu-id="fd2da-148">The ID associated with the online meeting.</span></span> <span data-ttu-id="fd2da-149">HTTP の GET 要求では ID として使用</span><span class="sxs-lookup"><span data-stu-id="fd2da-149">Used in a GET HTTP request as the ID.</span></span> <span data-ttu-id="fd2da-150">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="fd2da-150">Read-only.</span></span> <span data-ttu-id="fd2da-151">サーバーを生成します。</span><span class="sxs-lookup"><span data-stu-id="fd2da-151">Server generated.</span></span> |
| <span data-ttu-id="fd2da-152">isCancelled</span><span class="sxs-lookup"><span data-stu-id="fd2da-152">isCancelled</span></span>               | <span data-ttu-id="fd2da-153">ブール値</span><span class="sxs-lookup"><span data-stu-id="fd2da-153">Boolean</span></span>                                                | <span data-ttu-id="fd2da-154">かどうか、会議はキャンセルされました。</span><span class="sxs-lookup"><span data-stu-id="fd2da-154">Whether the meeting has been canceled.</span></span> |
| <span data-ttu-id="fd2da-155">joinUrl</span><span class="sxs-lookup"><span data-stu-id="fd2da-155">joinUrl</span></span>                   | <span data-ttu-id="fd2da-156">String</span><span class="sxs-lookup"><span data-stu-id="fd2da-156">String</span></span>                                                 | <span data-ttu-id="fd2da-157">Web サイトからオンライン会議を結合するときに使用される URL です。</span><span class="sxs-lookup"><span data-stu-id="fd2da-157">The URL that is used when the online meeting is joined from the web.</span></span> |
| <span data-ttu-id="fd2da-158">meetingType</span><span class="sxs-lookup"><span data-stu-id="fd2da-158">meetingType</span></span>               | <span data-ttu-id="fd2da-159">String</span><span class="sxs-lookup"><span data-stu-id="fd2da-159">String</span></span>                                                 | <span data-ttu-id="fd2da-160">使用可能な値: `meetNow`、 `scheduled`、 `recurring`、`broadcast`</span><span class="sxs-lookup"><span data-stu-id="fd2da-160">Possible values are: `meetNow`, `scheduled`, `recurring`, `broadcast`</span></span> |
| <span data-ttu-id="fd2da-161">participants</span><span class="sxs-lookup"><span data-stu-id="fd2da-161">participants</span></span>              | [<span data-ttu-id="fd2da-162">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="fd2da-162">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="fd2da-163">参加者がオンライン会議に関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="fd2da-163">The participants associated with the online meeting.</span></span>  <span data-ttu-id="fd2da-164">これには、開催者と出席者が含まれます。</span><span class="sxs-lookup"><span data-stu-id="fd2da-164">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="fd2da-165">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fd2da-165">startDateTime</span></span>             | <span data-ttu-id="fd2da-166">DateTime</span><span class="sxs-lookup"><span data-stu-id="fd2da-166">DateTime</span></span>                                               | <span data-ttu-id="fd2da-167">会議の開始時刻。</span><span class="sxs-lookup"><span data-stu-id="fd2da-167">Start time of the meeting.</span></span> |
| <span data-ttu-id="fd2da-168">subject</span><span class="sxs-lookup"><span data-stu-id="fd2da-168">subject</span></span>                   | <span data-ttu-id="fd2da-169">String</span><span class="sxs-lookup"><span data-stu-id="fd2da-169">String</span></span>                                                 | <span data-ttu-id="fd2da-170">オンライン会議の件名です。</span><span class="sxs-lookup"><span data-stu-id="fd2da-170">The subject of the online meeting.</span></span> |

## <a name="relationships"></a><span data-ttu-id="fd2da-171">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fd2da-171">Relationships</span></span>
<span data-ttu-id="fd2da-172">なし</span><span class="sxs-lookup"><span data-stu-id="fd2da-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd2da-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fd2da-173">JSON representation</span></span>

<span data-ttu-id="fd2da-174">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fd2da-174">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "accessLevel": "everyone | invited | locked | sameEnterprise",
  "audioConferencing": {"@odata.type": "#microsoft.graph.audioConferencing"},
  "canceledDateTime": "String (timestamp)",
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "entryExitAnnouncement": true,
  "expirationDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "isCancelled": false,
  "joinUrl": "String",
  "meetingType": "meetNow | scheduled | recurring | broadcast",
  "participants": {"@odata.type": "#microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onlineMeeting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
