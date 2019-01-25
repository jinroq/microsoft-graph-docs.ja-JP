---
title: onlineMeeting リソースの種類
description: 結合 URL、出席者リスト、説明など、会議に関する情報をキャプチャします。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d7009ceaf815986d50c8eb3b64d2541c32f01a88
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519599"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="ca4fa-103">onlineMeeting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ca4fa-103">onlineMeeting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca4fa-104">結合 URL、出席者リスト、説明など、会議に関する情報をキャプチャします。</span><span class="sxs-lookup"><span data-stu-id="ca4fa-104">Captures information about the meeting, including the join URL, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="ca4fa-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="ca4fa-105">Methods</span></span>

| <span data-ttu-id="ca4fa-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="ca4fa-106">Method</span></span>         | <span data-ttu-id="ca4fa-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ca4fa-107">Return Type</span></span> | <span data-ttu-id="ca4fa-108">説明</span><span class="sxs-lookup"><span data-stu-id="ca4fa-108">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="ca4fa-109">OnlineMeeting を取得します。</span><span class="sxs-lookup"><span data-stu-id="ca4fa-109">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="ca4fa-110">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="ca4fa-110">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="ca4fa-111">OnlineMeeting オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ca4fa-111">Read properties and relationships of onlineMeeting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ca4fa-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca4fa-112">Properties</span></span>

| <span data-ttu-id="ca4fa-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca4fa-113">Property</span></span>                  | <span data-ttu-id="ca4fa-114">型</span><span class="sxs-lookup"><span data-stu-id="ca4fa-114">Type</span></span>                                                   | <span data-ttu-id="ca4fa-115">説明</span><span class="sxs-lookup"><span data-stu-id="ca4fa-115">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ca4fa-116">AccessLevel</span><span class="sxs-lookup"><span data-stu-id="ca4fa-116">accessLevel</span></span>               | <span data-ttu-id="ca4fa-117">String</span><span class="sxs-lookup"><span data-stu-id="ca4fa-117">String</span></span>                                                 | <span data-ttu-id="ca4fa-118">オンラインの会議出席依頼の受付を制御するアクセス レベルです。</span><span class="sxs-lookup"><span data-stu-id="ca4fa-118">The access level that controls admission to the online meeting.</span></span> <span data-ttu-id="ca4fa-119">可能な値は、`everyone`、`invited`、`locked`、`sameEnterprise`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="ca4fa-119">Possible values are: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`.</span></span> |
| <span data-ttu-id="ca4fa-120">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="ca4fa-120">audioConferencing</span></span>         | [<span data-ttu-id="ca4fa-121">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="ca4fa-121">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="ca4fa-122">OnlineMeeting には、電話アクセス情報を表します。</span><span class="sxs-lookup"><span data-stu-id="ca4fa-122">Represents phone access information for an onlineMeeting.</span></span> |
| <span data-ttu-id="ca4fa-123">canceledDateTime</span><span class="sxs-lookup"><span data-stu-id="ca4fa-123">canceledDateTime</span></span>          | <span data-ttu-id="ca4fa-124">DateTime
</span><span class="sxs-lookup"><span data-stu-id="ca4fa-124">DateTime</span></span>                                               | <span data-ttu-id="ca4fa-125">会議がキャンセルされた時刻。</span><span class="sxs-lookup"><span data-stu-id="ca4fa-125">The time when the meeting was canceled.</span></span> |
| <span data-ttu-id="ca4fa-126">chatInfo</span><span class="sxs-lookup"><span data-stu-id="ca4fa-126">chatInfo</span></span>                  | [<span data-ttu-id="ca4fa-127">chatInfo</span><span class="sxs-lookup"><span data-stu-id="ca4fa-127">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="ca4fa-128">この会議に関連付けられているチャット。</span><span class="sxs-lookup"><span data-stu-id="ca4fa-128">The chat associated with this meeting.</span></span> |
| <span data-ttu-id="ca4fa-129">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="ca4fa-129">creationDateTime</span></span>          | <span data-ttu-id="ca4fa-130">DateTime
</span><span class="sxs-lookup"><span data-stu-id="ca4fa-130">DateTime</span></span>                                               | <span data-ttu-id="ca4fa-131">ミーティングが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="ca4fa-131">The time when the meeting was created.</span></span> <span data-ttu-id="ca4fa-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ca4fa-132">Readonly.</span></span>
| <span data-ttu-id="ca4fa-133">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ca4fa-133">endDateTime</span></span>               | <span data-ttu-id="ca4fa-134">DateTime
</span><span class="sxs-lookup"><span data-stu-id="ca4fa-134">DateTime</span></span>                                               | <span data-ttu-id="ca4fa-135">会議の終了時間です。</span><span class="sxs-lookup"><span data-stu-id="ca4fa-135">End time of the meeting.</span></span> |
| <span data-ttu-id="ca4fa-136">entryExitAnnouncement</span><span class="sxs-lookup"><span data-stu-id="ca4fa-136">entryExitAnnouncement</span></span>     | <span data-ttu-id="ca4fa-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="ca4fa-137">Boolean</span></span>                                                | <span data-ttu-id="ca4fa-138">オンライン会議の出席のお知らせ状態です。</span><span class="sxs-lookup"><span data-stu-id="ca4fa-138">The attendance announcements status for the online meeting.</span></span> <span data-ttu-id="ca4fa-139">出勤のお知らせを有効にすると、オンライン会議、発表 participantswho 結合の名前、会議のオーディオを使用します。</span><span class="sxs-lookup"><span data-stu-id="ca4fa-139">When attendance announcements are enabled, the online meeting will announce the names of the participantswho join the meeting through audio.</span></span> |
| <span data-ttu-id="ca4fa-140">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ca4fa-140">expirationDateTime</span></span>        | <span data-ttu-id="ca4fa-141">DateTime
</span><span class="sxs-lookup"><span data-stu-id="ca4fa-141">DateTime</span></span>                                               | <span data-ttu-id="ca4fa-142">絶対の世界協定時刻 (UTC) の日付と時刻は、オンライン会議を削除できます。</span><span class="sxs-lookup"><span data-stu-id="ca4fa-142">The absolute Coordinated Universal Time (UTC) date and time after which the online meeting can be deleted.</span></span> <span data-ttu-id="ca4fa-143">曜日と時間は、1 年前に、および現在の日付と、サーバー上の時刻の後 10 年間する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ca4fa-143">The day and time must be between one year before, and ten years after, the current date and time on the server.</span></span> |
| <span data-ttu-id="ca4fa-144">id</span><span class="sxs-lookup"><span data-stu-id="ca4fa-144">id</span></span>                        | <span data-ttu-id="ca4fa-145">String</span><span class="sxs-lookup"><span data-stu-id="ca4fa-145">String</span></span>                                                 | <span data-ttu-id="ca4fa-146">オンライン会議に関連付けられている ID です。</span><span class="sxs-lookup"><span data-stu-id="ca4fa-146">The ID associated with the online meeting.</span></span> <span data-ttu-id="ca4fa-147">HTTP の GET 要求では ID として使用</span><span class="sxs-lookup"><span data-stu-id="ca4fa-147">Used in a GET HTTP request as the ID.</span></span> <span data-ttu-id="ca4fa-148">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ca4fa-148">Read-only.</span></span> <span data-ttu-id="ca4fa-149">サーバーを生成します。</span><span class="sxs-lookup"><span data-stu-id="ca4fa-149">Server generated.</span></span> |
| <span data-ttu-id="ca4fa-150">isCancelled</span><span class="sxs-lookup"><span data-stu-id="ca4fa-150">isCancelled</span></span>               | <span data-ttu-id="ca4fa-151">ブール値</span><span class="sxs-lookup"><span data-stu-id="ca4fa-151">Boolean</span></span>                                                | <span data-ttu-id="ca4fa-152">かどうか、会議はキャンセルされました。</span><span class="sxs-lookup"><span data-stu-id="ca4fa-152">Whether the meeting has been canceled.</span></span> |
| <span data-ttu-id="ca4fa-153">joinUrl</span><span class="sxs-lookup"><span data-stu-id="ca4fa-153">joinUrl</span></span>                   | <span data-ttu-id="ca4fa-154">String</span><span class="sxs-lookup"><span data-stu-id="ca4fa-154">String</span></span>                                                 | <span data-ttu-id="ca4fa-155">Web サイトからオンライン会議を結合するときに使用される URL です。</span><span class="sxs-lookup"><span data-stu-id="ca4fa-155">The URL that is used when the online meeting is joined from the web.</span></span> |
| <span data-ttu-id="ca4fa-156">meetingType</span><span class="sxs-lookup"><span data-stu-id="ca4fa-156">meetingType</span></span>               | <span data-ttu-id="ca4fa-157">String</span><span class="sxs-lookup"><span data-stu-id="ca4fa-157">String</span></span>                                                 | <span data-ttu-id="ca4fa-158">可能な値は、`meetNow`、`scheduled`、`recurring` です。</span><span class="sxs-lookup"><span data-stu-id="ca4fa-158">Possible values are: `meetNow`, `scheduled`, `recurring`, `broadcast`</span></span> |
| <span data-ttu-id="ca4fa-159">participants</span><span class="sxs-lookup"><span data-stu-id="ca4fa-159">participants</span></span>              | [<span data-ttu-id="ca4fa-160">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="ca4fa-160">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="ca4fa-161">参加者がオンライン会議に関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="ca4fa-161">The participants associated with the online meeting.</span></span>  <span data-ttu-id="ca4fa-162">これには、開催者と出席者が含まれます。</span><span class="sxs-lookup"><span data-stu-id="ca4fa-162">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="ca4fa-163">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ca4fa-163">startDateTime</span></span>             | <span data-ttu-id="ca4fa-164">DateTime
</span><span class="sxs-lookup"><span data-stu-id="ca4fa-164">DateTime</span></span>                                               | <span data-ttu-id="ca4fa-165">会議の開始時刻。</span><span class="sxs-lookup"><span data-stu-id="ca4fa-165">Start time of the meeting.</span></span> |
| <span data-ttu-id="ca4fa-166">subject</span><span class="sxs-lookup"><span data-stu-id="ca4fa-166">subject</span></span>                   | <span data-ttu-id="ca4fa-167">String</span><span class="sxs-lookup"><span data-stu-id="ca4fa-167">String</span></span>                                                 | <span data-ttu-id="ca4fa-168">オンライン会議の件名です。</span><span class="sxs-lookup"><span data-stu-id="ca4fa-168">The subject of the online meeting.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ca4fa-169">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ca4fa-169">Relationships</span></span>
<span data-ttu-id="ca4fa-170">なし</span><span class="sxs-lookup"><span data-stu-id="ca4fa-170">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca4fa-171">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ca4fa-171">JSON representation</span></span>

<span data-ttu-id="ca4fa-172">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ca4fa-172">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "onlineMeeting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onlinemeeting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
