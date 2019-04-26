---
title: onlineMeeting リソースの種類
description: 参加 URL、参加者リスト、説明など、会議に関する情報を取り込みます。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d7009ceaf815986d50c8eb3b64d2541c32f01a88
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568864"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="794e4-103">onlineMeeting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="794e4-103">onlineMeeting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="794e4-104">参加 URL、参加者リスト、説明など、会議に関する情報を取り込みます。</span><span class="sxs-lookup"><span data-stu-id="794e4-104">Captures information about the meeting, including the join URL, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="794e4-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="794e4-105">Methods</span></span>

| <span data-ttu-id="794e4-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="794e4-106">Method</span></span>         | <span data-ttu-id="794e4-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="794e4-107">Return Type</span></span> | <span data-ttu-id="794e4-108">説明</span><span class="sxs-lookup"><span data-stu-id="794e4-108">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="794e4-109">onlineMeeting を取得する</span><span class="sxs-lookup"><span data-stu-id="794e4-109">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="794e4-110">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="794e4-110">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="794e4-111">onlineMeeting オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="794e4-111">Read properties and relationships of onlineMeeting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="794e4-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="794e4-112">Properties</span></span>

| <span data-ttu-id="794e4-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="794e4-113">Property</span></span>                  | <span data-ttu-id="794e4-114">型</span><span class="sxs-lookup"><span data-stu-id="794e4-114">Type</span></span>                                                   | <span data-ttu-id="794e4-115">説明</span><span class="sxs-lookup"><span data-stu-id="794e4-115">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="794e4-116">accessLevel</span><span class="sxs-lookup"><span data-stu-id="794e4-116">accessLevel</span></span>               | <span data-ttu-id="794e4-117">String</span><span class="sxs-lookup"><span data-stu-id="794e4-117">String</span></span>                                                 | <span data-ttu-id="794e4-118">オンライン会議への受付を制御するアクセスレベル。</span><span class="sxs-lookup"><span data-stu-id="794e4-118">The access level that controls admission to the online meeting.</span></span> <span data-ttu-id="794e4-119">可能な値は、`everyone`、`invited`、`locked`、`sameEnterprise`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="794e4-119">Possible values are: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`.</span></span> |
| <span data-ttu-id="794e4-120">audioconferencing</span><span class="sxs-lookup"><span data-stu-id="794e4-120">audioConferencing</span></span>         | [<span data-ttu-id="794e4-121">audioconferencing</span><span class="sxs-lookup"><span data-stu-id="794e4-121">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="794e4-122">onlineMeeting の電話アクセス情報を表します。</span><span class="sxs-lookup"><span data-stu-id="794e4-122">Represents phone access information for an onlineMeeting.</span></span> |
| <span data-ttu-id="794e4-123">canceleddatetime</span><span class="sxs-lookup"><span data-stu-id="794e4-123">canceledDateTime</span></span>          | <span data-ttu-id="794e4-124">DateTime
</span><span class="sxs-lookup"><span data-stu-id="794e4-124">DateTime</span></span>                                               | <span data-ttu-id="794e4-125">会議がキャンセルされた時刻。</span><span class="sxs-lookup"><span data-stu-id="794e4-125">The time when the meeting was canceled.</span></span> |
| <span data-ttu-id="794e4-126">chatInfo</span><span class="sxs-lookup"><span data-stu-id="794e4-126">chatInfo</span></span>                  | [<span data-ttu-id="794e4-127">chatInfo</span><span class="sxs-lookup"><span data-stu-id="794e4-127">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="794e4-128">この会議に関連付けられているチャット。</span><span class="sxs-lookup"><span data-stu-id="794e4-128">The chat associated with this meeting.</span></span> |
| <span data-ttu-id="794e4-129">日付/時刻 (datetime)</span><span class="sxs-lookup"><span data-stu-id="794e4-129">creationDateTime</span></span>          | <span data-ttu-id="794e4-130">DateTime
</span><span class="sxs-lookup"><span data-stu-id="794e4-130">DateTime</span></span>                                               | <span data-ttu-id="794e4-131">会議が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="794e4-131">The time when the meeting was created.</span></span> <span data-ttu-id="794e4-132">該当.</span><span class="sxs-lookup"><span data-stu-id="794e4-132">Readonly.</span></span>
| <span data-ttu-id="794e4-133">endDateTime</span><span class="sxs-lookup"><span data-stu-id="794e4-133">endDateTime</span></span>               | <span data-ttu-id="794e4-134">DateTime
</span><span class="sxs-lookup"><span data-stu-id="794e4-134">DateTime</span></span>                                               | <span data-ttu-id="794e4-135">会議の終了時刻。</span><span class="sxs-lookup"><span data-stu-id="794e4-135">End time of the meeting.</span></span> |
| <span data-ttu-id="794e4-136">entryexitannouncement</span><span class="sxs-lookup"><span data-stu-id="794e4-136">entryExitAnnouncement</span></span>     | <span data-ttu-id="794e4-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="794e4-137">Boolean</span></span>                                                | <span data-ttu-id="794e4-138">オンライン会議の出席アナウンスの状態。</span><span class="sxs-lookup"><span data-stu-id="794e4-138">The attendance announcements status for the online meeting.</span></span> <span data-ttu-id="794e4-139">出席依頼のアナウンスが有効になっている場合、オンライン会議では、participantswho の名前が音声で会議に参加するようにアナウンスされます。</span><span class="sxs-lookup"><span data-stu-id="794e4-139">When attendance announcements are enabled, the online meeting will announce the names of the participantswho join the meeting through audio.</span></span> |
| <span data-ttu-id="794e4-140">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="794e4-140">expirationDateTime</span></span>        | <span data-ttu-id="794e4-141">DateTime
</span><span class="sxs-lookup"><span data-stu-id="794e4-141">DateTime</span></span>                                               | <span data-ttu-id="794e4-142">オンライン会議を削除できる、世界協定時 (UTC) の日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="794e4-142">The absolute Coordinated Universal Time (UTC) date and time after which the online meeting can be deleted.</span></span> <span data-ttu-id="794e4-143">日付と時刻は、サーバー上の現在の日付と時刻の1年前、10年前にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="794e4-143">The day and time must be between one year before, and ten years after, the current date and time on the server.</span></span> |
| <span data-ttu-id="794e4-144">id</span><span class="sxs-lookup"><span data-stu-id="794e4-144">id</span></span>                        | <span data-ttu-id="794e4-145">String</span><span class="sxs-lookup"><span data-stu-id="794e4-145">String</span></span>                                                 | <span data-ttu-id="794e4-146">オンライン会議に関連付けられている ID。</span><span class="sxs-lookup"><span data-stu-id="794e4-146">The ID associated with the online meeting.</span></span> <span data-ttu-id="794e4-147">ID として GET HTTP 要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="794e4-147">Used in a GET HTTP request as the ID.</span></span> <span data-ttu-id="794e4-148">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="794e4-148">Read-only.</span></span> <span data-ttu-id="794e4-149">サーバーによって生成されます。</span><span class="sxs-lookup"><span data-stu-id="794e4-149">Server generated.</span></span> |
| <span data-ttu-id="794e4-150">isCancelled</span><span class="sxs-lookup"><span data-stu-id="794e4-150">isCancelled</span></span>               | <span data-ttu-id="794e4-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="794e4-151">Boolean</span></span>                                                | <span data-ttu-id="794e4-152">会議がキャンセルされたかどうか。</span><span class="sxs-lookup"><span data-stu-id="794e4-152">Whether the meeting has been canceled.</span></span> |
| <span data-ttu-id="794e4-153">joinurl</span><span class="sxs-lookup"><span data-stu-id="794e4-153">joinUrl</span></span>                   | <span data-ttu-id="794e4-154">String</span><span class="sxs-lookup"><span data-stu-id="794e4-154">String</span></span>                                                 | <span data-ttu-id="794e4-155">オンライン会議が web から参加しているときに使用される URL。</span><span class="sxs-lookup"><span data-stu-id="794e4-155">The URL that is used when the online meeting is joined from the web.</span></span> |
| <span data-ttu-id="794e4-156">会議の種類</span><span class="sxs-lookup"><span data-stu-id="794e4-156">meetingType</span></span>               | <span data-ttu-id="794e4-157">String</span><span class="sxs-lookup"><span data-stu-id="794e4-157">String</span></span>                                                 | <span data-ttu-id="794e4-158">可能な値は`meetNow`、 `scheduled`、 `recurring`、、です。`broadcast`</span><span class="sxs-lookup"><span data-stu-id="794e4-158">Possible values are: `meetNow`, `scheduled`, `recurring`, `broadcast`</span></span> |
| <span data-ttu-id="794e4-159">参加者</span><span class="sxs-lookup"><span data-stu-id="794e4-159">participants</span></span>              | [<span data-ttu-id="794e4-160">会議参加者</span><span class="sxs-lookup"><span data-stu-id="794e4-160">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="794e4-161">オンライン会議に関連付けられている参加者。</span><span class="sxs-lookup"><span data-stu-id="794e4-161">The participants associated with the online meeting.</span></span>  <span data-ttu-id="794e4-162">これには、開催者と出席者が含まれます。</span><span class="sxs-lookup"><span data-stu-id="794e4-162">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="794e4-163">startDateTime</span><span class="sxs-lookup"><span data-stu-id="794e4-163">startDateTime</span></span>             | <span data-ttu-id="794e4-164">DateTime
</span><span class="sxs-lookup"><span data-stu-id="794e4-164">DateTime</span></span>                                               | <span data-ttu-id="794e4-165">会議の開始時刻。</span><span class="sxs-lookup"><span data-stu-id="794e4-165">Start time of the meeting.</span></span> |
| <span data-ttu-id="794e4-166">subject</span><span class="sxs-lookup"><span data-stu-id="794e4-166">subject</span></span>                   | <span data-ttu-id="794e4-167">String</span><span class="sxs-lookup"><span data-stu-id="794e4-167">String</span></span>                                                 | <span data-ttu-id="794e4-168">オンライン会議の件名。</span><span class="sxs-lookup"><span data-stu-id="794e4-168">The subject of the online meeting.</span></span> |

## <a name="relationships"></a><span data-ttu-id="794e4-169">関係</span><span class="sxs-lookup"><span data-stu-id="794e4-169">Relationships</span></span>
<span data-ttu-id="794e4-170">なし</span><span class="sxs-lookup"><span data-stu-id="794e4-170">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="794e4-171">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="794e4-171">JSON representation</span></span>

<span data-ttu-id="794e4-172">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="794e4-172">The following is a JSON representation of the resource.</span></span>

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
