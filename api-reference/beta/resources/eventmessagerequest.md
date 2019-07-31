---
title: eventMessageRequest リソースの種類
description: 会議出席依頼を表すメッセージ。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 3d691b814517a6180a42ecd13954e019cc75be8b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973592"
---
# <a name="eventmessagerequest-resource-type"></a><span data-ttu-id="79e7a-103">eventMessageRequest リソースの種類</span><span class="sxs-lookup"><span data-stu-id="79e7a-103">eventMessageRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79e7a-104">会議出席依頼を表すメッセージ。</span><span class="sxs-lookup"><span data-stu-id="79e7a-104">A message that represents a meeting request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="79e7a-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="79e7a-105">JSON representation</span></span>

<span data-ttu-id="79e7a-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="79e7a-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [
    "attachments",
    "event",
    "extensions",
    "previousLocation",
    "previousStartDateTime",
    "previousEndDateTime"
  ],
  "@odata.type": "microsoft.graph.eventMessageRequest"
}-->

```json
{
  "bccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "string",
  "categories": ["string"],
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "changeKey": "string",
  "conversationId": "string",
  "createdDateTime": "String (timestamp)",
  "endDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isOutOfDate": "Boolean",
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "String (timestamp)",
  "location": {"@odata.type": "microsoft.graph.location"},
  "meetingMessageType": "microsoft.graph.meetingMessageType",
  "parentFolderId": "string",
  "previousEndDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "previousLocation": {"@odata.type": "microsoft.graph.location"},
  "previousStartDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "receivedDateTime": "String (timestamp)",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "String (timestamp)",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "subject": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "type": "string",
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "webLink": "string"
}

```
## <a name="properties"></a><span data-ttu-id="79e7a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79e7a-107">Properties</span></span>
| <span data-ttu-id="79e7a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79e7a-108">Property</span></span>     | <span data-ttu-id="79e7a-109">型</span><span class="sxs-lookup"><span data-stu-id="79e7a-109">Type</span></span>   |<span data-ttu-id="79e7a-110">説明</span><span class="sxs-lookup"><span data-stu-id="79e7a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79e7a-111">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="79e7a-111">bccRecipients</span></span>|<span data-ttu-id="79e7a-112">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="79e7a-112">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="79e7a-113">メッセージの BCC 受信者。</span><span class="sxs-lookup"><span data-stu-id="79e7a-113">The Bcc: recipients for the message.</span></span>|
|<span data-ttu-id="79e7a-114">body</span><span class="sxs-lookup"><span data-stu-id="79e7a-114">body</span></span>|[<span data-ttu-id="79e7a-115">itemBody</span><span class="sxs-lookup"><span data-stu-id="79e7a-115">itemBody</span></span>](itembody.md)|<span data-ttu-id="79e7a-116">メッセージの本文。</span><span class="sxs-lookup"><span data-stu-id="79e7a-116">The body of the message.</span></span>|
|<span data-ttu-id="79e7a-117">bodyPreview</span><span class="sxs-lookup"><span data-stu-id="79e7a-117">bodyPreview</span></span>|<span data-ttu-id="79e7a-118">String</span><span class="sxs-lookup"><span data-stu-id="79e7a-118">String</span></span>|<span data-ttu-id="79e7a-119">メッセージ本文の最初の 255 文字。</span><span class="sxs-lookup"><span data-stu-id="79e7a-119">The first 255 characters of the message body.</span></span>|
|<span data-ttu-id="79e7a-120">categories</span><span class="sxs-lookup"><span data-stu-id="79e7a-120">categories</span></span>|<span data-ttu-id="79e7a-121">String collection</span><span class="sxs-lookup"><span data-stu-id="79e7a-121">String collection</span></span>|<span data-ttu-id="79e7a-122">メッセージに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="79e7a-122">The categories associated with the message.</span></span>|
|<span data-ttu-id="79e7a-123">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="79e7a-123">ccRecipients</span></span>|<span data-ttu-id="79e7a-124">[recipient](recipient.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="79e7a-124">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="79e7a-125">メッセージの CC 受信者。</span><span class="sxs-lookup"><span data-stu-id="79e7a-125">The Cc: recipients for the message.</span></span>|
|<span data-ttu-id="79e7a-126">changeKey</span><span class="sxs-lookup"><span data-stu-id="79e7a-126">changeKey</span></span>|<span data-ttu-id="79e7a-127">String</span><span class="sxs-lookup"><span data-stu-id="79e7a-127">String</span></span>|<span data-ttu-id="79e7a-128">メッセージのバージョン。</span><span class="sxs-lookup"><span data-stu-id="79e7a-128">The version of the message.</span></span>|
|<span data-ttu-id="79e7a-129">conversationId</span><span class="sxs-lookup"><span data-stu-id="79e7a-129">conversationId</span></span>|<span data-ttu-id="79e7a-130">String</span><span class="sxs-lookup"><span data-stu-id="79e7a-130">String</span></span>|<span data-ttu-id="79e7a-131">電子メールが属している会話の ID。</span><span class="sxs-lookup"><span data-stu-id="79e7a-131">The ID of the conversation the email belongs to.</span></span>|
|<span data-ttu-id="79e7a-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79e7a-132">createdDateTime</span></span>|<span data-ttu-id="79e7a-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79e7a-133">DateTimeOffset</span></span>|<span data-ttu-id="79e7a-134">メッセージが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="79e7a-134">The date and time the message was created.</span></span>|
|<span data-ttu-id="79e7a-135">endDateTime</span><span class="sxs-lookup"><span data-stu-id="79e7a-135">endDateTime</span></span>|[<span data-ttu-id="79e7a-136">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="79e7a-136">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="79e7a-137">要求された会議の終了時刻。</span><span class="sxs-lookup"><span data-stu-id="79e7a-137">The end time of the requested meeting.</span></span>|
|<span data-ttu-id="79e7a-138">from</span><span class="sxs-lookup"><span data-stu-id="79e7a-138">from</span></span>|[<span data-ttu-id="79e7a-139">recipient</span><span class="sxs-lookup"><span data-stu-id="79e7a-139">recipient</span></span>](recipient.md)|<span data-ttu-id="79e7a-140">メッセージのメールボックス所有者と送信者。</span><span class="sxs-lookup"><span data-stu-id="79e7a-140">The mailbox owner and sender of the message.</span></span>|
|<span data-ttu-id="79e7a-141">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="79e7a-141">hasAttachments</span></span>|<span data-ttu-id="79e7a-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="79e7a-142">Boolean</span></span>|<span data-ttu-id="79e7a-143">メッセージに添付ファイルがあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="79e7a-143">Indicates whether the message has attachments.</span></span>|
|<span data-ttu-id="79e7a-144">id</span><span class="sxs-lookup"><span data-stu-id="79e7a-144">id</span></span>|<span data-ttu-id="79e7a-145">文字列</span><span class="sxs-lookup"><span data-stu-id="79e7a-145">String</span></span>|<span data-ttu-id="79e7a-146">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="79e7a-146">Read-only.</span></span>|
|<span data-ttu-id="79e7a-147">importance</span><span class="sxs-lookup"><span data-stu-id="79e7a-147">importance</span></span>|<span data-ttu-id="79e7a-148">String</span><span class="sxs-lookup"><span data-stu-id="79e7a-148">String</span></span>| <span data-ttu-id="79e7a-149">メッセージの重要度: `Low`、`Normal`、`High`。</span><span class="sxs-lookup"><span data-stu-id="79e7a-149">The importance of the message: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="79e7a-150">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="79e7a-150">inferenceClassification</span></span>|<span data-ttu-id="79e7a-151">String</span><span class="sxs-lookup"><span data-stu-id="79e7a-151">String</span></span>| <span data-ttu-id="79e7a-152">可能な値は、`Focused`、`Other` です。</span><span class="sxs-lookup"><span data-stu-id="79e7a-152">Possible values are: `Focused`, `Other`.</span></span>|
|<span data-ttu-id="79e7a-153">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="79e7a-153">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="79e7a-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="79e7a-154">Boolean</span></span>|<span data-ttu-id="79e7a-155">メッセージの開封確認メッセージが要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="79e7a-155">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="79e7a-156">isDraft</span><span class="sxs-lookup"><span data-stu-id="79e7a-156">isDraft</span></span>|<span data-ttu-id="79e7a-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="79e7a-157">Boolean</span></span>|<span data-ttu-id="79e7a-p101">メッセージが下書きかどうかを示します。メッセージがまだ送信されていなければ下書きです。</span><span class="sxs-lookup"><span data-stu-id="79e7a-p101">Indicates whether the message is a draft. A message is a draft if it hasn't been sent yet.</span></span>|
|<span data-ttu-id="79e7a-160">isOutOfDate</span><span class="sxs-lookup"><span data-stu-id="79e7a-160">isOutOfDate</span></span>|<span data-ttu-id="79e7a-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="79e7a-161">Boolean</span></span>|<span data-ttu-id="79e7a-162">この会議出席要求がより新しい要求によって古くなっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="79e7a-162">Indicates whether this meeting request has been made out-of-date by a more recent request.</span></span>|
|<span data-ttu-id="79e7a-163">isRead</span><span class="sxs-lookup"><span data-stu-id="79e7a-163">isRead</span></span>|<span data-ttu-id="79e7a-164">ブール値</span><span class="sxs-lookup"><span data-stu-id="79e7a-164">Boolean</span></span>|<span data-ttu-id="79e7a-165">メッセージが開封されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="79e7a-165">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="79e7a-166">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="79e7a-166">isReadReceiptRequested</span></span>|<span data-ttu-id="79e7a-167">ブール値</span><span class="sxs-lookup"><span data-stu-id="79e7a-167">Boolean</span></span>|<span data-ttu-id="79e7a-168">メッセージの開封確認メッセージが要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="79e7a-168">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="79e7a-169">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="79e7a-169">lastModifiedDateTime</span></span>|<span data-ttu-id="79e7a-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79e7a-170">DateTimeOffset</span></span>|<span data-ttu-id="79e7a-171">メッセージが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="79e7a-171">The date and time the message was last changed.</span></span>|
|<span data-ttu-id="79e7a-172">location</span><span class="sxs-lookup"><span data-stu-id="79e7a-172">location</span></span>|[<span data-ttu-id="79e7a-173">Location</span><span class="sxs-lookup"><span data-stu-id="79e7a-173">Location</span></span>](location.md)|<span data-ttu-id="79e7a-174">要求された会議の場所。</span><span class="sxs-lookup"><span data-stu-id="79e7a-174">The location of the requested meeting.</span></span>|
|<span data-ttu-id="79e7a-175">meetingMessageType</span><span class="sxs-lookup"><span data-stu-id="79e7a-175">meetingMessageType</span></span>|<span data-ttu-id="79e7a-176">String</span><span class="sxs-lookup"><span data-stu-id="79e7a-176">String</span></span>| <span data-ttu-id="79e7a-177">イベント メッセージの種類: `none`、`meetingRequest`、`meetingCancelled``meetingAccepted``meetingTentativelyAccepted``meetingDeclined`。</span><span class="sxs-lookup"><span data-stu-id="79e7a-177">The type of event message: `none`, `meetingRequest`, `meetingCancelled`, `meetingAccepted`, `meetingTentativelyAccepted`, `meetingDeclined`.</span></span>|
|<span data-ttu-id="79e7a-178">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="79e7a-178">parentFolderId</span></span>|<span data-ttu-id="79e7a-179">String</span><span class="sxs-lookup"><span data-stu-id="79e7a-179">String</span></span>|<span data-ttu-id="79e7a-180">メッセージの親 mailFolder の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="79e7a-180">The unique identifier for the message's parent mailFolder.</span></span>|
|<span data-ttu-id="79e7a-181">前の Enddatetime</span><span class="sxs-lookup"><span data-stu-id="79e7a-181">previousEndDateTime</span></span>|[<span data-ttu-id="79e7a-182">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="79e7a-182">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="79e7a-183">要求された会議の前回の終了時刻。</span><span class="sxs-lookup"><span data-stu-id="79e7a-183">The previous end time of the requested meeting.</span></span>|
|<span data-ttu-id="79e7a-184">previousLocation</span><span class="sxs-lookup"><span data-stu-id="79e7a-184">previousLocation</span></span>|[<span data-ttu-id="79e7a-185">Location</span><span class="sxs-lookup"><span data-stu-id="79e7a-185">Location</span></span>](location.md)|<span data-ttu-id="79e7a-186">会議出席依頼の以前の場所。</span><span class="sxs-lookup"><span data-stu-id="79e7a-186">The previous location of the requested meeting.</span></span>|
|<span data-ttu-id="79e7a-187">previousStartDateTime</span><span class="sxs-lookup"><span data-stu-id="79e7a-187">previousStartDateTime</span></span>|[<span data-ttu-id="79e7a-188">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="79e7a-188">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="79e7a-189">要求された会議の前回の開始時刻。</span><span class="sxs-lookup"><span data-stu-id="79e7a-189">The previous start time of the requested meeting.</span></span>|
|<span data-ttu-id="79e7a-190">receivedDateTime</span><span class="sxs-lookup"><span data-stu-id="79e7a-190">receivedDateTime</span></span>|<span data-ttu-id="79e7a-191">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79e7a-191">DateTimeOffset</span></span>|<span data-ttu-id="79e7a-192">メッセージが受信された日時です。</span><span class="sxs-lookup"><span data-stu-id="79e7a-192">The date and time the message was received.</span></span>|
|<span data-ttu-id="79e7a-193">recurrence</span><span class="sxs-lookup"><span data-stu-id="79e7a-193">recurrence</span></span>|[<span data-ttu-id="79e7a-194">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="79e7a-194">PatternedRecurrence</span></span>](patternedrecurrence.md)|<span data-ttu-id="79e7a-195">要求された会議の定期的なパターン。</span><span class="sxs-lookup"><span data-stu-id="79e7a-195">The recurrence pattern of the requested meeting.</span></span>|
|<span data-ttu-id="79e7a-196">replyTo</span><span class="sxs-lookup"><span data-stu-id="79e7a-196">replyTo</span></span>|<span data-ttu-id="79e7a-197">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="79e7a-197">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="79e7a-198">返信時に使用される電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="79e7a-198">The email addresses to use when replying.</span></span>|
|<span data-ttu-id="79e7a-199">sender</span><span class="sxs-lookup"><span data-stu-id="79e7a-199">sender</span></span>|[<span data-ttu-id="79e7a-200">recipient</span><span class="sxs-lookup"><span data-stu-id="79e7a-200">recipient</span></span>](recipient.md)|<span data-ttu-id="79e7a-201">メッセージを生成するために実際に使用されるアカウント。</span><span class="sxs-lookup"><span data-stu-id="79e7a-201">The account that is actually used to generate the message.</span></span>|
|<span data-ttu-id="79e7a-202">sentDateTime</span><span class="sxs-lookup"><span data-stu-id="79e7a-202">sentDateTime</span></span>|<span data-ttu-id="79e7a-203">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79e7a-203">DateTimeOffset</span></span>|<span data-ttu-id="79e7a-204">メッセージが送信された日時。</span><span class="sxs-lookup"><span data-stu-id="79e7a-204">The date and time the message was sent.</span></span>|
|<span data-ttu-id="79e7a-205">startDateTime</span><span class="sxs-lookup"><span data-stu-id="79e7a-205">startDateTime</span></span>|[<span data-ttu-id="79e7a-206">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="79e7a-206">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="79e7a-207">要求された会議の開始時刻。</span><span class="sxs-lookup"><span data-stu-id="79e7a-207">The start time of the requested meeting.</span></span>|
|<span data-ttu-id="79e7a-208">subject</span><span class="sxs-lookup"><span data-stu-id="79e7a-208">subject</span></span>|<span data-ttu-id="79e7a-209">String</span><span class="sxs-lookup"><span data-stu-id="79e7a-209">String</span></span>|<span data-ttu-id="79e7a-210">メッセージの件名。</span><span class="sxs-lookup"><span data-stu-id="79e7a-210">The subject of the message.</span></span>|
|<span data-ttu-id="79e7a-211">toRecipients</span><span class="sxs-lookup"><span data-stu-id="79e7a-211">toRecipients</span></span>|<span data-ttu-id="79e7a-212">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="79e7a-212">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="79e7a-213">メッセージの宛先。</span><span class="sxs-lookup"><span data-stu-id="79e7a-213">The To: recipients for the message.</span></span>|
|<span data-ttu-id="79e7a-214">type</span><span class="sxs-lookup"><span data-stu-id="79e7a-214">type</span></span>|<span data-ttu-id="79e7a-215">String</span><span class="sxs-lookup"><span data-stu-id="79e7a-215">String</span></span>|<span data-ttu-id="79e7a-216">要求された会議の`singleInstance`種類`occurence`: `exception`、 `seriesMaster`、、。</span><span class="sxs-lookup"><span data-stu-id="79e7a-216">The type of requested meeting: `singleInstance`, `occurence`, `exception`, `seriesMaster`.</span></span>|
|<span data-ttu-id="79e7a-217">uniqueBody</span><span class="sxs-lookup"><span data-stu-id="79e7a-217">uniqueBody</span></span>|[<span data-ttu-id="79e7a-218">itemBody</span><span class="sxs-lookup"><span data-stu-id="79e7a-218">itemBody</span></span>](itembody.md)|<span data-ttu-id="79e7a-219">現在のメッセージに特有のメッセージの本文の一部。</span><span class="sxs-lookup"><span data-stu-id="79e7a-219">The part of the body of the message that is unique to the current message.</span></span>|
|<span data-ttu-id="79e7a-220">webLink</span><span class="sxs-lookup"><span data-stu-id="79e7a-220">webLink</span></span>|<span data-ttu-id="79e7a-221">String</span><span class="sxs-lookup"><span data-stu-id="79e7a-221">String</span></span>|<span data-ttu-id="79e7a-222">Outlook Web App でメッセージを開く URL。</span><span class="sxs-lookup"><span data-stu-id="79e7a-222">The URL to open the message in Outlook Web App.</span></span><br><br><span data-ttu-id="79e7a-p102">URL の末尾に ispopout 引数を付加して、メッセージの表示方法を変更できます。ispopout が存在しない、または 1 に設定されている場合は、メッセージがポップアウト ウィンドウに表示されます。ispopout が 0 に設定されている場合、ブラウザーの Outlook Web App レビュー ウィンドウにメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="79e7a-p102">You can append an ispopout argument to the end of the URL to change how the message is displayed. If ispopout is not present or if it is set to 1, then the message is shown in a popout window. If ispopout is set to 0, then the browser will show the message in the Outlook Web App review pane.</span></span><br><br><span data-ttu-id="79e7a-p103">Outlook Web App のメールボックスにログインしている場合、ブラウザーでメッセージが開きます。まだブラウザーでログインしていない場合、ログインするように求められます。</span><span class="sxs-lookup"><span data-stu-id="79e7a-p103">The message will open in the browser if you are logged in to your mailbox via Outlook Web App. You will be prompted to login if you are not already logged in with the browser.</span></span><br><br><span data-ttu-id="79e7a-228">この URL には、iFrame 内からアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="79e7a-228">This URL can be accessed from within an iFrame.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79e7a-229">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="79e7a-229">Relationships</span></span>
| <span data-ttu-id="79e7a-230">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="79e7a-230">Relationship</span></span> | <span data-ttu-id="79e7a-231">型</span><span class="sxs-lookup"><span data-stu-id="79e7a-231">Type</span></span>   |<span data-ttu-id="79e7a-232">説明</span><span class="sxs-lookup"><span data-stu-id="79e7a-232">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79e7a-233">attachments</span><span class="sxs-lookup"><span data-stu-id="79e7a-233">attachments</span></span>|<span data-ttu-id="79e7a-234">[Attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="79e7a-234">[Attachment](attachment.md) collection</span></span>| <span data-ttu-id="79e7a-p104">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="79e7a-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="79e7a-237">イベント</span><span class="sxs-lookup"><span data-stu-id="79e7a-237">event</span></span>|[<span data-ttu-id="79e7a-238">Event</span><span class="sxs-lookup"><span data-stu-id="79e7a-238">Event</span></span>](event.md)| <span data-ttu-id="79e7a-p105">イベント メッセージに関連付けられたイベント。参加者または部屋リソースの前提は、会議出席依頼イベント メッセージが届いたときにイベントを含む予定表を自動的に更新するようにカレンダー アテンダントが設定されていることです。ナビゲーション プロパティ。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="79e7a-p105">The event associated with the event message. The assumption for attendees or room resources is that the Calendar Attendant is set to automatically update the calendar with an event when meeting request event messages arrive. Navigation property.  Read-only.</span></span>|
|<span data-ttu-id="79e7a-243">extensions</span><span class="sxs-lookup"><span data-stu-id="79e7a-243">extensions</span></span>|<span data-ttu-id="79e7a-244">[Extension](extension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="79e7a-244">[Extension](extension.md) collection</span></span>| <span data-ttu-id="79e7a-245">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="79e7a-245">Read-only.</span></span> <span data-ttu-id="79e7a-246">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="79e7a-246">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="79e7a-247">メソッド</span><span class="sxs-lookup"><span data-stu-id="79e7a-247">Methods</span></span>

| <span data-ttu-id="79e7a-248">メソッド</span><span class="sxs-lookup"><span data-stu-id="79e7a-248">Method</span></span>           | <span data-ttu-id="79e7a-249">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="79e7a-249">Return Type</span></span>    |<span data-ttu-id="79e7a-250">説明</span><span class="sxs-lookup"><span data-stu-id="79e7a-250">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="79e7a-251">eventMessage の取得</span><span class="sxs-lookup"><span data-stu-id="79e7a-251">Get eventMessage</span></span>](../api/eventmessage-get.md) | [<span data-ttu-id="79e7a-252">eventMessage</span><span class="sxs-lookup"><span data-stu-id="79e7a-252">eventMessage</span></span>](eventmessage.md) |<span data-ttu-id="79e7a-253">eventMessage オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="79e7a-253">Read properties and relationships of eventMessage object.</span></span>|
|[<span data-ttu-id="79e7a-254">添付ファイルの作成</span><span class="sxs-lookup"><span data-stu-id="79e7a-254">Create Attachment</span></span>](../api/eventmessage-post-attachments.md) |[<span data-ttu-id="79e7a-255">Attachment</span><span class="sxs-lookup"><span data-stu-id="79e7a-255">Attachment</span></span>](attachment.md)| <span data-ttu-id="79e7a-256">添付ファイル コレクションへの投稿により、新しい添付ファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="79e7a-256">Create a new Attachment by posting to the attachments collection.</span></span>|
|[<span data-ttu-id="79e7a-257">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="79e7a-257">List attachments</span></span>](../api/eventmessage-list-attachments.md) |<span data-ttu-id="79e7a-258">[Attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="79e7a-258">[Attachment](attachment.md) collection</span></span>| <span data-ttu-id="79e7a-259">添付ファイルのオブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="79e7a-259">Get a Attachment object collection.</span></span>|
|[<span data-ttu-id="79e7a-260">更新する</span><span class="sxs-lookup"><span data-stu-id="79e7a-260">Update</span></span>](../api/eventmessage-update.md) | [<span data-ttu-id="79e7a-261">eventMessage</span><span class="sxs-lookup"><span data-stu-id="79e7a-261">eventMessage</span></span>](eventmessage.md)  |<span data-ttu-id="79e7a-262">eventMessage オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="79e7a-262">Update eventMessage object.</span></span> |
|[<span data-ttu-id="79e7a-263">Delete</span><span class="sxs-lookup"><span data-stu-id="79e7a-263">Delete</span></span>](../api/eventmessage-delete.md) | <span data-ttu-id="79e7a-264">None</span><span class="sxs-lookup"><span data-stu-id="79e7a-264">None</span></span> |<span data-ttu-id="79e7a-265">eventMessage オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="79e7a-265">Delete eventMessage object.</span></span> |
|[<span data-ttu-id="79e7a-266">コピー</span><span class="sxs-lookup"><span data-stu-id="79e7a-266">copy</span></span>](../api/message-copy.md)|[<span data-ttu-id="79e7a-267">Message</span><span class="sxs-lookup"><span data-stu-id="79e7a-267">Message</span></span>](message.md)||
|[<span data-ttu-id="79e7a-268">createForward</span><span class="sxs-lookup"><span data-stu-id="79e7a-268">createForward</span></span>](../api/message-createforward.md)|[<span data-ttu-id="79e7a-269">Message</span><span class="sxs-lookup"><span data-stu-id="79e7a-269">Message</span></span>](message.md)||
|[<span data-ttu-id="79e7a-270">createReply</span><span class="sxs-lookup"><span data-stu-id="79e7a-270">createReply</span></span>](../api/message-createreply.md)|[<span data-ttu-id="79e7a-271">Message</span><span class="sxs-lookup"><span data-stu-id="79e7a-271">Message</span></span>](message.md)||
|[<span data-ttu-id="79e7a-272">createReplyAll</span><span class="sxs-lookup"><span data-stu-id="79e7a-272">createReplyAll</span></span>](../api/message-createreplyall.md)|[<span data-ttu-id="79e7a-273">Message</span><span class="sxs-lookup"><span data-stu-id="79e7a-273">Message</span></span>](message.md)||
|[<span data-ttu-id="79e7a-274">forward</span><span class="sxs-lookup"><span data-stu-id="79e7a-274">forward</span></span>](../api/message-forward.md)|<span data-ttu-id="79e7a-275">None</span><span class="sxs-lookup"><span data-stu-id="79e7a-275">None</span></span>|<span data-ttu-id="79e7a-276">メッセージを転送します。</span><span class="sxs-lookup"><span data-stu-id="79e7a-276">Forwards a message.</span></span> <span data-ttu-id="79e7a-277">その後、メッセージは [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="79e7a-277">The message is then saved in the Sent Items folder.</span></span>|
|[<span data-ttu-id="79e7a-278">move</span><span class="sxs-lookup"><span data-stu-id="79e7a-278">move</span></span>](../api/message-move.md)|[<span data-ttu-id="79e7a-279">Message</span><span class="sxs-lookup"><span data-stu-id="79e7a-279">Message</span></span>](message.md)|<span data-ttu-id="79e7a-280">メッセージを mailFolder に移動します。</span><span class="sxs-lookup"><span data-stu-id="79e7a-280">Move the message to a mailFolder.</span></span>|
|[<span data-ttu-id="79e7a-281">返信</span><span class="sxs-lookup"><span data-stu-id="79e7a-281">reply</span></span>](../api/message-reply.md)|<span data-ttu-id="79e7a-282">None</span><span class="sxs-lookup"><span data-stu-id="79e7a-282">None</span></span>|<span data-ttu-id="79e7a-283">メッセージの送信者に replys を送信します。</span><span class="sxs-lookup"><span data-stu-id="79e7a-283">Replys to the sender of a message.</span></span> <span data-ttu-id="79e7a-284">その後、メッセージは [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="79e7a-284">The message is then saved in the Sent Items folder.</span></span>|
|[<span data-ttu-id="79e7a-285">replyAll</span><span class="sxs-lookup"><span data-stu-id="79e7a-285">replyAll</span></span>](../api/message-replyall.md)|<span data-ttu-id="79e7a-286">なし</span><span class="sxs-lookup"><span data-stu-id="79e7a-286">None</span></span>|<span data-ttu-id="79e7a-p109">メッセージの受信者すべてに返信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="79e7a-p109">Reply to all recipients of a message. The message is then saved in the Sent Items folder.</span></span>|
|[<span data-ttu-id="79e7a-289">送信</span><span class="sxs-lookup"><span data-stu-id="79e7a-289">send</span></span>](../api/message-send.md)|<span data-ttu-id="79e7a-290">なし</span><span class="sxs-lookup"><span data-stu-id="79e7a-290">None</span></span>|<span data-ttu-id="79e7a-p110">以前に作成したメッセージの下書きを送信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="79e7a-p110">Sends a previously created message draft. The message is then saved in the Sent Items folder.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "eventMessageRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
