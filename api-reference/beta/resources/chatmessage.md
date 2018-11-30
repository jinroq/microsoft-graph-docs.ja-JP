---
title: chatMessage リソースの種類
description: チャネルまたはチャットのエンティティ内で個別のチャット メッセージを表します。 メッセージは、ルートのメッセージまたはメッセージ内の**replyToId**プロパティで定義されているスレッドの一部にできます。
ms.openlocfilehash: 1fba27567d5a1c80a36a5758925ec427735504cf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066604"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="1f5a3-104">chatMessage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1f5a3-104">chatMessage resource type</span></span>

> <span data-ttu-id="1f5a3-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1f5a3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f5a3-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f5a3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1f5a3-107">[チャネル](channel.md)またはチャットのエンティティ内で個別のチャット メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="1f5a3-107">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="1f5a3-108">メッセージは、ルートのメッセージまたはメッセージ内の**replyToId**プロパティで定義されているスレッドの一部にできます。</span><span class="sxs-lookup"><span data-stu-id="1f5a3-108">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="1f5a3-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="1f5a3-109">Methods</span></span>

| <span data-ttu-id="1f5a3-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="1f5a3-110">Method</span></span>       | <span data-ttu-id="1f5a3-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1f5a3-111">Return Type</span></span>  |<span data-ttu-id="1f5a3-112">説明</span><span class="sxs-lookup"><span data-stu-id="1f5a3-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1f5a3-113">リストのチャネルのメッセージ</span><span class="sxs-lookup"><span data-stu-id="1f5a3-113">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="1f5a3-114">[chatmessage](chatmessage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1f5a3-114">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="1f5a3-115">チャネルでは、ルートのすべてのメッセージの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="1f5a3-115">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="1f5a3-116">チャネル取得メッセージ</span><span class="sxs-lookup"><span data-stu-id="1f5a3-116">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="1f5a3-117">chatmessage</span><span class="sxs-lookup"><span data-stu-id="1f5a3-117">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="1f5a3-118">チャンネルから 1 つのルートのメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="1f5a3-118">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="1f5a3-119">メッセージに対する返信の一覧</span><span class="sxs-lookup"><span data-stu-id="1f5a3-119">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="1f5a3-120">[chatmessage](chatmessage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1f5a3-120">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="1f5a3-121">チャネルでのメッセージに対する返信をすべての一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="1f5a3-121">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="1f5a3-122">メッセージへの応答を取得します。</span><span class="sxs-lookup"><span data-stu-id="1f5a3-122">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="1f5a3-123">chatmessage</span><span class="sxs-lookup"><span data-stu-id="1f5a3-123">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="1f5a3-124">チャネル内のメッセージに 1 つの返信を取得します。</span><span class="sxs-lookup"><span data-stu-id="1f5a3-124">Get a single reply to a message in a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="1f5a3-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f5a3-125">Properties</span></span>
| <span data-ttu-id="1f5a3-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f5a3-126">Property</span></span>     | <span data-ttu-id="1f5a3-127">型</span><span class="sxs-lookup"><span data-stu-id="1f5a3-127">Type</span></span>   |<span data-ttu-id="1f5a3-128">説明</span><span class="sxs-lookup"><span data-stu-id="1f5a3-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f5a3-129">id</span><span class="sxs-lookup"><span data-stu-id="1f5a3-129">id</span></span>|<span data-ttu-id="1f5a3-130">String</span><span class="sxs-lookup"><span data-stu-id="1f5a3-130">String</span></span>| <span data-ttu-id="1f5a3-131">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="1f5a3-131">Read-only.</span></span> <span data-ttu-id="1f5a3-132">メッセージの一意の ID です。</span><span class="sxs-lookup"><span data-stu-id="1f5a3-132">Unique ID of the message.</span></span>|
|<span data-ttu-id="1f5a3-133">replyToId</span><span class="sxs-lookup"><span data-stu-id="1f5a3-133">replyToId</span></span>| <span data-ttu-id="1f5a3-134">文字列</span><span class="sxs-lookup"><span data-stu-id="1f5a3-134">string</span></span> | <span data-ttu-id="1f5a3-135">スレッドの親メッセージとルートのメッセージの id</span><span class="sxs-lookup"><span data-stu-id="1f5a3-135">Id of the parent message/root message of the thread</span></span> |
|<span data-ttu-id="1f5a3-136">from</span><span class="sxs-lookup"><span data-stu-id="1f5a3-136">from</span></span>|[<span data-ttu-id="1f5a3-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="1f5a3-137">identitySet</span></span>](identityset.md)| <span data-ttu-id="1f5a3-138">メッセージの送信者の詳細</span><span class="sxs-lookup"><span data-stu-id="1f5a3-138">Details of the sender of the message</span></span>|
|<span data-ttu-id="1f5a3-139">etag</span><span class="sxs-lookup"><span data-stu-id="1f5a3-139">etag</span></span>| <span data-ttu-id="1f5a3-140">文字列</span><span class="sxs-lookup"><span data-stu-id="1f5a3-140">string</span></span> | <span data-ttu-id="1f5a3-141">メッセージのバージョン番号</span><span class="sxs-lookup"><span data-stu-id="1f5a3-141">Version number of the message</span></span> |
|<span data-ttu-id="1f5a3-142">messageType</span><span class="sxs-lookup"><span data-stu-id="1f5a3-142">messageType</span></span>|<span data-ttu-id="1f5a3-143">String</span><span class="sxs-lookup"><span data-stu-id="1f5a3-143">String</span></span>|<span data-ttu-id="1f5a3-144">サポートされているメッセージでは、現在の type の値: メッセージ、chatEvent を入力します。</span><span class="sxs-lookup"><span data-stu-id="1f5a3-144">The type of message, current supported values are: message, chatEvent, Typing</span></span>|
|<span data-ttu-id="1f5a3-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1f5a3-145">createdDateTime</span></span>|<span data-ttu-id="1f5a3-146">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f5a3-146">dateTimeOffset</span></span>|<span data-ttu-id="1f5a3-147">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1f5a3-147">Read only.</span></span> <span data-ttu-id="1f5a3-148">メッセージが作成された日時のタイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="1f5a3-148">Timestamp of when the message was created</span></span>|
|<span data-ttu-id="1f5a3-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f5a3-149">lastModifiedDateTime</span></span>|<span data-ttu-id="1f5a3-150">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f5a3-150">dateTimeOffset</span></span>|<span data-ttu-id="1f5a3-151">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1f5a3-151">Read only.</span></span> <span data-ttu-id="1f5a3-152">メッセージが編集更新をされたときのタイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="1f5a3-152">Timestamp of when the message was edited/updated</span></span>|
|<span data-ttu-id="1f5a3-153">isDeleted</span><span class="sxs-lookup"><span data-stu-id="1f5a3-153">isDeleted</span></span>|<span data-ttu-id="1f5a3-154">ブール</span><span class="sxs-lookup"><span data-stu-id="1f5a3-154">boolean</span></span>|<span data-ttu-id="1f5a3-155">メッセージをソフト削除されている場合を表します。</span><span class="sxs-lookup"><span data-stu-id="1f5a3-155">Represents if a message has been soft deleted</span></span>|
|<span data-ttu-id="1f5a3-156">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f5a3-156">deletedDateTime</span></span>|<span data-ttu-id="1f5a3-157">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f5a3-157">dateTimeOffset</span></span>|<span data-ttu-id="1f5a3-158">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1f5a3-158">Read only.</span></span> <span data-ttu-id="1f5a3-159">タイムスタンプは、メッセージが削除されました</span><span class="sxs-lookup"><span data-stu-id="1f5a3-159">Timestamp at which the message was deleted</span></span> |
|<span data-ttu-id="1f5a3-160">subject</span><span class="sxs-lookup"><span data-stu-id="1f5a3-160">subject</span></span>|<span data-ttu-id="1f5a3-161">文字列</span><span class="sxs-lookup"><span data-stu-id="1f5a3-161">string</span></span>|<span data-ttu-id="1f5a3-162">メッセージの件名です。</span><span class="sxs-lookup"><span data-stu-id="1f5a3-162">Message subject line.</span></span> <span data-ttu-id="1f5a3-163">省略可能</span><span class="sxs-lookup"><span data-stu-id="1f5a3-163">Optional</span></span>|
|<span data-ttu-id="1f5a3-164">body</span><span class="sxs-lookup"><span data-stu-id="1f5a3-164">body</span></span>|[<span data-ttu-id="1f5a3-165">itemBody</span><span class="sxs-lookup"><span data-stu-id="1f5a3-165">itemBody</span></span>](itembody.md)|<span data-ttu-id="1f5a3-166">メッセージのコンテンツのプレーン テキストと HTML 形式です。</span><span class="sxs-lookup"><span data-stu-id="1f5a3-166">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="1f5a3-167">プレーン テキストを返します既定では、アプリケーションは、クエリ パラメーターの一部として HTML を選択できます。</span><span class="sxs-lookup"><span data-stu-id="1f5a3-167">Returns plain text by default, application can choose HTML as part of a query param</span></span>|
|<span data-ttu-id="1f5a3-168">概要</span><span class="sxs-lookup"><span data-stu-id="1f5a3-168">summary</span></span>|<span data-ttu-id="1f5a3-169">文字列</span><span class="sxs-lookup"><span data-stu-id="1f5a3-169">string</span></span>|<span data-ttu-id="1f5a3-170">プッシュ通知し、サマリー ・ ビューまたはフォール バック ・ ビューの使用できるメッセージの概要のテキスト</span><span class="sxs-lookup"><span data-stu-id="1f5a3-170">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="1f5a3-171">mentions</span><span class="sxs-lookup"><span data-stu-id="1f5a3-171">mentions</span></span>|<span data-ttu-id="1f5a3-172">[chatMessageMention](chatmention.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1f5a3-172">[chatMessageMention](chatmention.md) collection</span></span>| <span data-ttu-id="1f5a3-173">メッセージに記載されているエンティティの一覧です。</span><span class="sxs-lookup"><span data-stu-id="1f5a3-173">List of entities mentioned in the message.</span></span> <span data-ttu-id="1f5a3-174">チャネル、ユーザー、ボット、チームが現在サポートしています</span><span class="sxs-lookup"><span data-stu-id="1f5a3-174">Currently supports user, bot, team, channel</span></span>|
|<span data-ttu-id="1f5a3-175">importance</span><span class="sxs-lookup"><span data-stu-id="1f5a3-175">importance</span></span>| <span data-ttu-id="1f5a3-176">文字列</span><span class="sxs-lookup"><span data-stu-id="1f5a3-176">string</span></span> | <span data-ttu-id="1f5a3-177">メッセージの重要度: 高、通常</span><span class="sxs-lookup"><span data-stu-id="1f5a3-177">The importance of the message: Normal, High</span></span>|
|<span data-ttu-id="1f5a3-178">反力</span><span class="sxs-lookup"><span data-stu-id="1f5a3-178">reactions</span></span>| <span data-ttu-id="1f5a3-179">[chatMessageReaction](chatreaction.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1f5a3-179">[chatMessageReaction](chatreaction.md) collection</span></span> | <span data-ttu-id="1f5a3-180">このメッセージの反応 (たとえばなど)</span><span class="sxs-lookup"><span data-stu-id="1f5a3-180">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="1f5a3-181">locale</span><span class="sxs-lookup"><span data-stu-id="1f5a3-181">locale</span></span>|<span data-ttu-id="1f5a3-182">文字列</span><span class="sxs-lookup"><span data-stu-id="1f5a3-182">string</span></span>|<span data-ttu-id="1f5a3-183">クライアントが設定するメッセージのロケール</span><span class="sxs-lookup"><span data-stu-id="1f5a3-183">Locale of the message set by the client</span></span>|
|<span data-ttu-id="1f5a3-184">attachments</span><span class="sxs-lookup"><span data-stu-id="1f5a3-184">attachments</span></span>|<span data-ttu-id="1f5a3-185">[chatMessageAttachment](chatattachment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1f5a3-185">[chatMessageAttachment](chatattachment.md) collection</span></span> |<span data-ttu-id="1f5a3-186">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="1f5a3-186">Attached files</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1f5a3-187">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1f5a3-187">JSON representation</span></span>

<span data-ttu-id="1f5a3-188">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1f5a3-188">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "isDeleted",
    "deletedDateTime",
    "attachments",
    "importance",
    "reactions",
    "mentions",
    "subject",
    "summary"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessage"
}-->

```json
{
  "id": "string (identifier)",
  "replyToId": "string (identifier)",
  "from": {"@odata.type": "microsoft.graph.identitySet"},
  "etag": "string",
  "messageType": "string",
  "createdDateTime": "string (timestamp)",
  "lastModifiedDateTime": "string (timestamp)",
  "isDeleted": "boolean",
  "deletedDateTime": "string (timestamp)",
  "subject": "string",
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "summary": "string",
  "attachments": [{"@odata.type": "microsoft.graph.chatMessageAttachment"}],
  "mentions": [{"@odata.type": "microsoft.graph.chatMessageMention"}],
  "importance": "string",
  "reactions": [{"@odata.type": "microsoft.graph.chatMessageReaction"}],
  "locale": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
