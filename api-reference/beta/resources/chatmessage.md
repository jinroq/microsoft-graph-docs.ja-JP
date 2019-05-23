---
title: chatMessage リソースの種類
description: チャネルまたはチャット エンティティ内の個別のチャット メッセージを表します。 メッセージは、ルート メッセージまたはメッセージの中の **replyToId** プロパティに定義されているスレッドの一部にすることができます。
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 0639fd0b5317abd4814123b500ec0548f78d05ac
ms.sourcegitcommit: abca7fcefeaa74b50f4600b35d816b626ba08468
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/21/2019
ms.locfileid: "34311162"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="9ad1d-104">chatMessage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9ad1d-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ad1d-105">[チャネル](channel.md)または[チャット](chat.md)内の個別のチャット メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-105">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span> <span data-ttu-id="9ad1d-106">メッセージは、ルート メッセージまたはメッセージの中の **replyToId** プロパティに定義されているスレッドの一部にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-106">The message can be a root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="9ad1d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="9ad1d-107">Methods</span></span>

| <span data-ttu-id="9ad1d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="9ad1d-108">Method</span></span>       | <span data-ttu-id="9ad1d-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9ad1d-109">Return Type</span></span>  |<span data-ttu-id="9ad1d-110">説明</span><span class="sxs-lookup"><span data-stu-id="9ad1d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9ad1d-111">チャネル メッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="9ad1d-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="9ad1d-112">[chatmessage](chatmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9ad1d-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="9ad1d-113">チャネルのすべてのルート メッセージの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="9ad1d-114">チャネル メッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="9ad1d-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="9ad1d-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="9ad1d-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="9ad1d-116">チャネルからのルート メッセージを 1 件取得します。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="9ad1d-117">メッセージへの返信を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="9ad1d-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="9ad1d-118">[chatmessage](chatmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9ad1d-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="9ad1d-119">チャネル内のメッセージへの返信すべての一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="9ad1d-120">メッセージへの返信を取得する</span><span class="sxs-lookup"><span data-stu-id="9ad1d-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="9ad1d-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="9ad1d-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="9ad1d-122">チャネル内のメッセージへの返信を 1 件取得します。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="9ad1d-123">チャネル内でメッセージを送信する</span><span class="sxs-lookup"><span data-stu-id="9ad1d-123">Send a message in a channel</span></span>](../api/channel-post-chatmessage.md) | [<span data-ttu-id="9ad1d-124">chatmessage</span><span class="sxs-lookup"><span data-stu-id="9ad1d-124">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="9ad1d-125">チャネル内で新しい最上位レベルのメッセージを作成します。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-125">Create a new top-level message in a channel.</span></span>|
|[<span data-ttu-id="9ad1d-126">チャネル内のメッセージに返信する</span><span class="sxs-lookup"><span data-stu-id="9ad1d-126">Reply to a message in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="9ad1d-127">chatmessage</span><span class="sxs-lookup"><span data-stu-id="9ad1d-127">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="9ad1d-128">チャネル内の既存メッセージに返信します。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-128">Reply to an existing message in a channel.</span></span>|
|[<span data-ttu-id="9ad1d-129">チャット内のメッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="9ad1d-129">List messages in a chat</span></span>](../api/chat-list-messages.md)  | [<span data-ttu-id="9ad1d-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="9ad1d-130">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="9ad1d-131">1 対 1 またはグループ チャットでのメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-131">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="9ad1d-132">チャット内のメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="9ad1d-132">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="9ad1d-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="9ad1d-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="9ad1d-134">チャット内の 1 つのメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-134">Get a single message in a chat.</span></span> |


## <a name="properties"></a><span data-ttu-id="9ad1d-135">Properties</span><span class="sxs-lookup"><span data-stu-id="9ad1d-135">Properties</span></span>
| <span data-ttu-id="9ad1d-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ad1d-136">Property</span></span>     | <span data-ttu-id="9ad1d-137">型</span><span class="sxs-lookup"><span data-stu-id="9ad1d-137">Type</span></span>   |<span data-ttu-id="9ad1d-138">説明</span><span class="sxs-lookup"><span data-stu-id="9ad1d-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ad1d-139">id</span><span class="sxs-lookup"><span data-stu-id="9ad1d-139">id</span></span>|<span data-ttu-id="9ad1d-140">String</span><span class="sxs-lookup"><span data-stu-id="9ad1d-140">String</span></span>| <span data-ttu-id="9ad1d-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-141">Read-only.</span></span> <span data-ttu-id="9ad1d-142">メッセージの一意の ID。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-142">Unique ID of the message.</span></span>|
|<span data-ttu-id="9ad1d-143">replyToId</span><span class="sxs-lookup"><span data-stu-id="9ad1d-143">replyToId</span></span>| <span data-ttu-id="9ad1d-144">string</span><span class="sxs-lookup"><span data-stu-id="9ad1d-144">string</span></span> | <span data-ttu-id="9ad1d-145">スレッドの親メッセージ/ルート メッセージの ID。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-145">Id of the parent message/root message of the thread.</span></span> <span data-ttu-id="9ad1d-146">(チャットではなく、チャネルのメッセージにのみ適用)</span><span class="sxs-lookup"><span data-stu-id="9ad1d-146">(Only applies to messages in channels not chats)</span></span> |
|<span data-ttu-id="9ad1d-147">差出人</span><span class="sxs-lookup"><span data-stu-id="9ad1d-147">from</span></span>|[<span data-ttu-id="9ad1d-148">identitySet</span><span class="sxs-lookup"><span data-stu-id="9ad1d-148">identitySet</span></span>](identityset.md)| <span data-ttu-id="9ad1d-149">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-149">Read only.</span></span> <span data-ttu-id="9ad1d-150">メッセージの送信者の詳細。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-150">Details of the sender of the message.</span></span>|
|<span data-ttu-id="9ad1d-151">etag</span><span class="sxs-lookup"><span data-stu-id="9ad1d-151">etag</span></span>| <span data-ttu-id="9ad1d-152">string</span><span class="sxs-lookup"><span data-stu-id="9ad1d-152">string</span></span> | <span data-ttu-id="9ad1d-153">メッセージのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-153">Version number of the message.</span></span> |
|<span data-ttu-id="9ad1d-154">messageType</span><span class="sxs-lookup"><span data-stu-id="9ad1d-154">messageType</span></span>|<span data-ttu-id="9ad1d-155">String</span><span class="sxs-lookup"><span data-stu-id="9ad1d-155">String</span></span>|<span data-ttu-id="9ad1d-156">メッセージの種類。現在サポートされている値は message、chatEvent、Typing。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-156">The type of message, current supported values are: message, chatEvent, Typing.</span></span>|
|<span data-ttu-id="9ad1d-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ad1d-157">createdDateTime</span></span>|<span data-ttu-id="9ad1d-158">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ad1d-158">dateTimeOffset</span></span>|<span data-ttu-id="9ad1d-159">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-159">Read only.</span></span> <span data-ttu-id="9ad1d-160">メッセージ作成時のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-160">Timestamp of when the message was created.</span></span>|
|<span data-ttu-id="9ad1d-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ad1d-161">lastModifiedDateTime</span></span>|<span data-ttu-id="9ad1d-162">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ad1d-162">dateTimeOffset</span></span>|<span data-ttu-id="9ad1d-163">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-163">Read only.</span></span> <span data-ttu-id="9ad1d-164">メッセージ編集/更新時のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-164">Timestamp of when the message was edited/updated.</span></span>|
|<span data-ttu-id="9ad1d-165">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ad1d-165">deletedDateTime</span></span>|<span data-ttu-id="9ad1d-166">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ad1d-166">dateTimeOffset</span></span>|<span data-ttu-id="9ad1d-167">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-167">Read only.</span></span> <span data-ttu-id="9ad1d-168">メッセージが削除された時間のタイムスタンプ、または削除されていない場合は Null です。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-168">Timestamp at which the message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="9ad1d-169">件名</span><span class="sxs-lookup"><span data-stu-id="9ad1d-169">subject</span></span>|<span data-ttu-id="9ad1d-170">string</span><span class="sxs-lookup"><span data-stu-id="9ad1d-170">string</span></span>| <span data-ttu-id="9ad1d-171">プレーン テキストでの、メッセージの件名です。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-171">The subject of the message, in plaintext.</span></span>|
|<span data-ttu-id="9ad1d-172">本文</span><span class="sxs-lookup"><span data-stu-id="9ad1d-172">body</span></span>|[<span data-ttu-id="9ad1d-173">itemBody</span><span class="sxs-lookup"><span data-stu-id="9ad1d-173">itemBody</span></span>](itembody.md)|<span data-ttu-id="9ad1d-174">メッセージのコンテンツのプレーンテキスト/HTML 表記。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-174">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="9ad1d-175">表記は、本文内の contentType によって指定されます。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-175">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="9ad1d-176">メッセージに [chatMessageMention ](chatmessagemention.md) が含まれている場合、コンテンツは常に HTML で表示されます。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-176">The content is always in HTML if the message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="9ad1d-177">summary</span><span class="sxs-lookup"><span data-stu-id="9ad1d-177">summary</span></span>|<span data-ttu-id="9ad1d-178">string</span><span class="sxs-lookup"><span data-stu-id="9ad1d-178">string</span></span>| <span data-ttu-id="9ad1d-179">プッシュ通知および概要ビューまたはフォールバック ビューに使用できるメッセージの概要テキスト。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-179">Summary text of the message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="9ad1d-180">チャット メッセージではなく、チャネル メッセージにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-180">Only applies to channel messages, not chat messages.</span></span> |
|<span data-ttu-id="9ad1d-181">attachments</span><span class="sxs-lookup"><span data-stu-id="9ad1d-181">attachments</span></span>|<span data-ttu-id="9ad1d-182">[chatMessageAttachment](chatmessageattachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9ad1d-182">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="9ad1d-183">添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-183">Attached files.</span></span> <span data-ttu-id="9ad1d-184">添付ファイルは現在読み取り専用です。添付ファイルの送信はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-184">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="9ad1d-185">mentions</span><span class="sxs-lookup"><span data-stu-id="9ad1d-185">mentions</span></span>|<span data-ttu-id="9ad1d-186">[chatMessageMention](chatmessagemention.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9ad1d-186">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="9ad1d-187">メッセージに記載されているエンティティの一覧。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-187">List of entities mentioned in the message.</span></span> <span data-ttu-id="9ad1d-188">現在、user、bot、team、channel がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-188">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="9ad1d-189">importance</span><span class="sxs-lookup"><span data-stu-id="9ad1d-189">importance</span></span>| <span data-ttu-id="9ad1d-190">string</span><span class="sxs-lookup"><span data-stu-id="9ad1d-190">string</span></span> | <span data-ttu-id="9ad1d-191">メッセージの重要度: 通常、高。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-191">The importance of the message: Normal, High.</span></span>|
|<span data-ttu-id="9ad1d-192">reactions</span><span class="sxs-lookup"><span data-stu-id="9ad1d-192">reactions</span></span>| <span data-ttu-id="9ad1d-193">[chatMessageReaction](chatmessagereaction.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9ad1d-193">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="9ad1d-194">このメッセージに対する反応 (例: いいね!)。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-194">Reactions for this message (for example, Like).</span></span>|
|<span data-ttu-id="9ad1d-195">locale</span><span class="sxs-lookup"><span data-stu-id="9ad1d-195">locale</span></span>|<span data-ttu-id="9ad1d-196">string</span><span class="sxs-lookup"><span data-stu-id="9ad1d-196">string</span></span>|<span data-ttu-id="9ad1d-197">クライアントに設定されたメッセージのロケール。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-197">Locale of the message set by the client.</span></span>|
|<span data-ttu-id="9ad1d-198">webUrl</span><span class="sxs-lookup"><span data-stu-id="9ad1d-198">webUrl</span></span>|<span data-ttu-id="9ad1d-199">string</span><span class="sxs-lookup"><span data-stu-id="9ad1d-199">string</span></span>|<span data-ttu-id="9ad1d-200">Microsoft Teams のチャネルに移動するハイパーリンク。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-200">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="9ad1d-201">これは、Microsoft Teams でチャネルを右クリックし、[チームへのリンクを取得] を選択すると作成される URL です。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-201">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="9ad1d-202">この URL は不透明 blob として扱われる必要があり、また解析されません。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-202">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="9ad1d-203">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-203">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ad1d-204">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9ad1d-204">JSON representation</span></span>

<span data-ttu-id="9ad1d-205">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9ad1d-205">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "deleted",
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
  "deletedDateTime": "string (timestamp)",
  "subject": "string",
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "summary": "string",
  "attachments": [{"@odata.type": "microsoft.graph.chatMessageAttachment"}],
  "mentions": [{"@odata.type": "microsoft.graph.chatMessageMention"}],
  "importance": "string",
  "policyViolation": "string",
  "reactions": [{"@odata.type": "microsoft.graph.chatMessageReaction"}],
  "locale": "string",
  "deleted": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
