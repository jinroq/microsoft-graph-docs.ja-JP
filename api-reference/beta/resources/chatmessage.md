---
title: chatMessage リソースの種類
description: チャネルまたはチャット エンティティ内の個別のチャット メッセージを表します。 メッセージは、ルート メッセージまたはメッセージの中の **replyToId** プロパティに定義されているスレッドの一部にすることができます。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 3f27434e5dd8e3ccfc949c870a239522dd96d9d3
ms.sourcegitcommit: ca55fc5f5711966eaa41da31cd1ae99820e9e586
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/13/2019
ms.locfileid: "35645241"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="cd060-104">chatMessage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cd060-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd060-105">[チャネル](channel.md)または[チャット](chat.md)内の個別のチャット メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="cd060-105">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span>
<span data-ttu-id="cd060-106">メッセージは、ルート メッセージまたはメッセージの中の **replyToId** プロパティに定義されているスレッドの一部にすることができます。</span><span class="sxs-lookup"><span data-stu-id="cd060-106">The message can be a root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="cd060-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="cd060-107">Methods</span></span>

| <span data-ttu-id="cd060-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="cd060-108">Method</span></span>       | <span data-ttu-id="cd060-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cd060-109">Return Type</span></span>  |<span data-ttu-id="cd060-110">説明</span><span class="sxs-lookup"><span data-stu-id="cd060-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cd060-111">チャネル メッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cd060-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="cd060-112">[chatMessage](chatmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cd060-112">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="cd060-113">チャネルのすべてのルート メッセージの一覧。</span><span class="sxs-lookup"><span data-stu-id="cd060-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="cd060-114">チャネル メッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="cd060-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="cd060-115">chatMessage</span><span class="sxs-lookup"><span data-stu-id="cd060-115">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="cd060-116">チャネルからのルート メッセージを 1 件取得します。</span><span class="sxs-lookup"><span data-stu-id="cd060-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="cd060-117">メッセージへの返信を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cd060-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="cd060-118">[chatMessage](chatmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cd060-118">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="cd060-119">チャネル内のメッセージへの返信すべての一覧。</span><span class="sxs-lookup"><span data-stu-id="cd060-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="cd060-120">メッセージへの返信を取得する</span><span class="sxs-lookup"><span data-stu-id="cd060-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="cd060-121">chatMessage</span><span class="sxs-lookup"><span data-stu-id="cd060-121">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="cd060-122">チャネル内のメッセージへの返信を 1 件取得します。</span><span class="sxs-lookup"><span data-stu-id="cd060-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="cd060-123">チャネルでの chatMessage の作成</span><span class="sxs-lookup"><span data-stu-id="cd060-123">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="cd060-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="cd060-124">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="cd060-125">チャネル内で新しい最上位レベルのメッセージを作成します。</span><span class="sxs-lookup"><span data-stu-id="cd060-125">Create a new top-level message in a channel.</span></span>|
|[<span data-ttu-id="cd060-126">チャネル内のメッセージに返信する</span><span class="sxs-lookup"><span data-stu-id="cd060-126">Reply to a message in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="cd060-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="cd060-127">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="cd060-128">チャネル内の既存メッセージに返信します。</span><span class="sxs-lookup"><span data-stu-id="cd060-128">Reply to an existing message in a channel.</span></span>|
|[<span data-ttu-id="cd060-129">チャット内のメッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cd060-129">List messages in a chat</span></span>](../api/chat-list-messages.md)  | [<span data-ttu-id="cd060-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="cd060-130">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="cd060-131">1 対 1 またはグループ チャットでのメッセージを一覧表示する。</span><span class="sxs-lookup"><span data-stu-id="cd060-131">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="cd060-132">チャット内のメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="cd060-132">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="cd060-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="cd060-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="cd060-134">チャット内の 1 つのメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="cd060-134">Get a single message in a chat.</span></span> |
|[<span data-ttu-id="cd060-135">ホストされているすべての画像を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cd060-135">List all hosted images</span></span>](../api/chatmessagehostedimage-list-hostedimages.md) | <span data-ttu-id="cd060-136">[hostedimage](../resources/chatmessagehostedimage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cd060-136">[hostedImage](../resources/chatmessagehostedimage.md) collection</span></span>| <span data-ttu-id="cd060-137">メッセージ内のホストされているすべての画像を取得します。</span><span class="sxs-lookup"><span data-stu-id="cd060-137">Get all hosted images in a message.</span></span>|
|[<span data-ttu-id="cd060-138">ホストされている画像を取得する</span><span class="sxs-lookup"><span data-stu-id="cd060-138">Get hosted image</span></span>](../api/chatmessagehostedimage-get.md) | [<span data-ttu-id="cd060-139">hostedImage</span><span class="sxs-lookup"><span data-stu-id="cd060-139">hostedImage</span></span>](../resources/chatmessagehostedimage.md) | <span data-ttu-id="cd060-140">メッセージからホストされている画像を取得します。</span><span class="sxs-lookup"><span data-stu-id="cd060-140">Get a hosted image from a message.</span></span>|
|[<span data-ttu-id="cd060-141">ホストされている画像バイトを取得する</span><span class="sxs-lookup"><span data-stu-id="cd060-141">Get hosted image bytes</span></span>](../api/chatmessagehostedimage-getbytes.md) | <span data-ttu-id="cd060-142">バイナリ画像データ</span><span class="sxs-lookup"><span data-stu-id="cd060-142">binary image data</span></span> | <span data-ttu-id="cd060-143">メッセージからホストされている画像のバイナリ画像データを取得します。</span><span class="sxs-lookup"><span data-stu-id="cd060-143">Get binary image data of a hosted image from a message.</span></span>|

## <a name="properties"></a><span data-ttu-id="cd060-144">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cd060-144">Properties</span></span>

| <span data-ttu-id="cd060-145">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cd060-145">Property</span></span>   | <span data-ttu-id="cd060-146">型</span><span class="sxs-lookup"><span data-stu-id="cd060-146">Type</span></span> |<span data-ttu-id="cd060-147">説明</span><span class="sxs-lookup"><span data-stu-id="cd060-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd060-148">id</span><span class="sxs-lookup"><span data-stu-id="cd060-148">id</span></span>|<span data-ttu-id="cd060-149">String</span><span class="sxs-lookup"><span data-stu-id="cd060-149">String</span></span>| <span data-ttu-id="cd060-150">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cd060-150">Read-only.</span></span> <span data-ttu-id="cd060-151">メッセージの一意の ID。</span><span class="sxs-lookup"><span data-stu-id="cd060-151">Unique ID of the message.</span></span>|
|<span data-ttu-id="cd060-152">replyToId</span><span class="sxs-lookup"><span data-stu-id="cd060-152">replyToId</span></span>| <span data-ttu-id="cd060-153">string</span><span class="sxs-lookup"><span data-stu-id="cd060-153">string</span></span> | <span data-ttu-id="cd060-154">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cd060-154">Read-only.</span></span> <span data-ttu-id="cd060-155">スレッドの親メッセージ/ルート メッセージの ID。</span><span class="sxs-lookup"><span data-stu-id="cd060-155">Id of the parent message/root message of the thread.</span></span> <span data-ttu-id="cd060-156">(チャットではなく、チャネルのメッセージにのみ適用)</span><span class="sxs-lookup"><span data-stu-id="cd060-156">(Only applies to messages in channels not chats)</span></span> |
|<span data-ttu-id="cd060-157">差出人</span><span class="sxs-lookup"><span data-stu-id="cd060-157">from</span></span>|[<span data-ttu-id="cd060-158">identitySet</span><span class="sxs-lookup"><span data-stu-id="cd060-158">identitySet</span></span>](identityset.md)| <span data-ttu-id="cd060-159">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cd060-159">Read only.</span></span> <span data-ttu-id="cd060-160">メッセージの送信者の詳細。</span><span class="sxs-lookup"><span data-stu-id="cd060-160">Details of the sender of the message.</span></span>|
|<span data-ttu-id="cd060-161">etag</span><span class="sxs-lookup"><span data-stu-id="cd060-161">etag</span></span>| <span data-ttu-id="cd060-162">string</span><span class="sxs-lookup"><span data-stu-id="cd060-162">string</span></span> | <span data-ttu-id="cd060-163">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cd060-163">Read-only.</span></span> <span data-ttu-id="cd060-164">メッセージのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="cd060-164">Version number of the message.</span></span> |
|<span data-ttu-id="cd060-165">messageType</span><span class="sxs-lookup"><span data-stu-id="cd060-165">messageType</span></span>|<span data-ttu-id="cd060-166">chatMessageType</span><span class="sxs-lookup"><span data-stu-id="cd060-166">chatMessageType</span></span>|<span data-ttu-id="cd060-167">メッセージの種類。</span><span class="sxs-lookup"><span data-stu-id="cd060-167">The type of message.</span></span> <span data-ttu-id="cd060-168">使用可能な値: `message`。</span><span class="sxs-lookup"><span data-stu-id="cd060-168">The possible values are: `message`, , .</span></span>|
|<span data-ttu-id="cd060-169">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cd060-169">createdDateTime</span></span>|<span data-ttu-id="cd060-170">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd060-170">dateTimeOffset</span></span>|<span data-ttu-id="cd060-171">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cd060-171">Read only.</span></span> <span data-ttu-id="cd060-172">メッセージ作成時のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="cd060-172">Timestamp of when the message was created.</span></span>|
|<span data-ttu-id="cd060-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd060-173">lastModifiedDateTime</span></span>|<span data-ttu-id="cd060-174">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd060-174">dateTimeOffset</span></span>|<span data-ttu-id="cd060-175">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cd060-175">Read only.</span></span> <span data-ttu-id="cd060-176">メッセージの作成/編集時のタイムスタンプには、返信が行われた時間 (チャネル内のルート メッセージの場合) またはリアクションの追加または削除が行われた時間が含まれます。</span><span class="sxs-lookup"><span data-stu-id="cd060-176">Timestamp of when the message is created or edited, including when a reply is made (if it's a root message in a channel) or a reaction is added or removed.</span></span> |
|<span data-ttu-id="cd060-177">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd060-177">deletedDateTime</span></span>|<span data-ttu-id="cd060-178">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd060-178">dateTimeOffset</span></span>|<span data-ttu-id="cd060-179">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cd060-179">Read only.</span></span> <span data-ttu-id="cd060-180">メッセージが削除された時間のタイムスタンプ、または削除されていない場合は Null です。</span><span class="sxs-lookup"><span data-stu-id="cd060-180">Timestamp at which the message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="cd060-181">件名</span><span class="sxs-lookup"><span data-stu-id="cd060-181">subject</span></span>|<span data-ttu-id="cd060-182">string</span><span class="sxs-lookup"><span data-stu-id="cd060-182">string</span></span>| <span data-ttu-id="cd060-183">プレーン テキストでの、メッセージの件名です。</span><span class="sxs-lookup"><span data-stu-id="cd060-183">The subject of the message, in plaintext.</span></span>|
|<span data-ttu-id="cd060-184">本文</span><span class="sxs-lookup"><span data-stu-id="cd060-184">body</span></span>|[<span data-ttu-id="cd060-185">itemBody</span><span class="sxs-lookup"><span data-stu-id="cd060-185">itemBody</span></span>](itembody.md)|<span data-ttu-id="cd060-186">メッセージのコンテンツのプレーンテキスト/HTML 表記。</span><span class="sxs-lookup"><span data-stu-id="cd060-186">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="cd060-187">表記は、本文内の contentType によって指定されます。</span><span class="sxs-lookup"><span data-stu-id="cd060-187">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="cd060-188">メッセージに [chatMessageMention ](chatmessagemention.md) が含まれている場合、コンテンツは常に HTML で表示されます。</span><span class="sxs-lookup"><span data-stu-id="cd060-188">The content is always in HTML if the message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="cd060-189">summary</span><span class="sxs-lookup"><span data-stu-id="cd060-189">summary</span></span>|<span data-ttu-id="cd060-190">string</span><span class="sxs-lookup"><span data-stu-id="cd060-190">string</span></span>| <span data-ttu-id="cd060-191">プッシュ通知および概要ビューまたはフォールバック ビューに使用できるメッセージの概要テキスト。</span><span class="sxs-lookup"><span data-stu-id="cd060-191">Summary text of the message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="cd060-192">チャット メッセージではなく、チャネル メッセージにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="cd060-192">Only applies to channel messages, not chat messages.</span></span> |
|<span data-ttu-id="cd060-193">attachments</span><span class="sxs-lookup"><span data-stu-id="cd060-193">attachments</span></span>|<span data-ttu-id="cd060-194">[chatMessageAttachment](chatmessageattachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cd060-194">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="cd060-195">添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="cd060-195">Attached files.</span></span> <span data-ttu-id="cd060-196">添付ファイルは現在読み取り専用です。添付ファイルの送信はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd060-196">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="cd060-197">mentions</span><span class="sxs-lookup"><span data-stu-id="cd060-197">mentions</span></span>|<span data-ttu-id="cd060-198">[chatMessageMention](chatmessagemention.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cd060-198">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="cd060-199">メッセージに記載されているエンティティの一覧。</span><span class="sxs-lookup"><span data-stu-id="cd060-199">List of entities mentioned in the message.</span></span> <span data-ttu-id="cd060-200">現在、user、bot、team、channel がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="cd060-200">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="cd060-201">importance</span><span class="sxs-lookup"><span data-stu-id="cd060-201">importance</span></span>| <span data-ttu-id="cd060-202">chatMessageImportance</span><span class="sxs-lookup"><span data-stu-id="cd060-202">chatMessageImportance</span></span> | <span data-ttu-id="cd060-203">メッセージの重要度です。</span><span class="sxs-lookup"><span data-stu-id="cd060-203">The importance of the message.</span></span> <span data-ttu-id="cd060-204">使用可能な値: `normal`、`high`、`urgent`。</span><span class="sxs-lookup"><span data-stu-id="cd060-204">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="cd060-205">reactions</span><span class="sxs-lookup"><span data-stu-id="cd060-205">reactions</span></span>| <span data-ttu-id="cd060-206">[chatMessageReaction](chatmessagereaction.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cd060-206">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="cd060-207">このメッセージに対する反応 (例: いいね!)。</span><span class="sxs-lookup"><span data-stu-id="cd060-207">Reactions for this message (for example, Like).</span></span>|
|<span data-ttu-id="cd060-208">locale</span><span class="sxs-lookup"><span data-stu-id="cd060-208">locale</span></span>|<span data-ttu-id="cd060-209">string</span><span class="sxs-lookup"><span data-stu-id="cd060-209">string</span></span>|<span data-ttu-id="cd060-210">クライアントに設定されたメッセージのロケール。</span><span class="sxs-lookup"><span data-stu-id="cd060-210">Locale of the message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cd060-211">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cd060-211">JSON representation</span></span>

<span data-ttu-id="cd060-212">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cd060-212">The following is a JSON representation of the resource.</span></span>

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
