---
title: chatMessage リソースの種類
description: チャネルまたはチャット エンティティ内の個別のチャット メッセージを表します。 メッセージは、ルート メッセージまたはメッセージの中の **replyToId** プロパティに定義されているスレッドの一部にすることができます。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 99e69bd51a661b67fd4cb325fffe80db91214714
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778671"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="0839d-104">chatMessage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0839d-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0839d-105">[チャネル](channel.md)または[チャット](chat.md)内の個別のチャット メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="0839d-105">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span>
<span data-ttu-id="0839d-106">メッセージは、ルート メッセージまたはメッセージの中の **replyToId** プロパティに定義されているスレッドの一部にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0839d-106">The message can be a root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="0839d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0839d-107">Methods</span></span>

| <span data-ttu-id="0839d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0839d-108">Method</span></span>       | <span data-ttu-id="0839d-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0839d-109">Return Type</span></span>  |<span data-ttu-id="0839d-110">説明</span><span class="sxs-lookup"><span data-stu-id="0839d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0839d-111">チャネル メッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="0839d-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="0839d-112">[chatMessage](chatmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0839d-112">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="0839d-113">チャネル内のすべてのルートメッセージのリスト。</span><span class="sxs-lookup"><span data-stu-id="0839d-113">List of all root messages in a channel.</span></span>|
|[<span data-ttu-id="0839d-114">チャネル メッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="0839d-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="0839d-115">chatMessage</span><span class="sxs-lookup"><span data-stu-id="0839d-115">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="0839d-116">チャネルからのルート メッセージを 1 件取得します。</span><span class="sxs-lookup"><span data-stu-id="0839d-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="0839d-117">メッセージへの返信を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="0839d-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="0839d-118">[chatMessage](chatmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0839d-118">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="0839d-119">チャネル内のメッセージへのすべての返信のリスト。</span><span class="sxs-lookup"><span data-stu-id="0839d-119">List of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="0839d-120">メッセージへの返信を取得する</span><span class="sxs-lookup"><span data-stu-id="0839d-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="0839d-121">chatMessage</span><span class="sxs-lookup"><span data-stu-id="0839d-121">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="0839d-122">チャネル内のメッセージへの返信を 1 件取得します。</span><span class="sxs-lookup"><span data-stu-id="0839d-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="0839d-123">チャネルでの chatMessage の作成</span><span class="sxs-lookup"><span data-stu-id="0839d-123">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="0839d-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="0839d-124">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="0839d-125">チャネル内で新しい最上位レベルのメッセージを作成します。</span><span class="sxs-lookup"><span data-stu-id="0839d-125">Create a new top-level message in a channel.</span></span>|
|[<span data-ttu-id="0839d-126">チャネル内のメッセージに返信する</span><span class="sxs-lookup"><span data-stu-id="0839d-126">Reply to a message in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="0839d-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="0839d-127">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="0839d-128">チャネル内の既存メッセージに返信します。</span><span class="sxs-lookup"><span data-stu-id="0839d-128">Reply to an existing message in a channel.</span></span>|
|[<span data-ttu-id="0839d-129">チャット内のメッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="0839d-129">List messages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="0839d-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="0839d-130">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="0839d-131">1:1 またはグループチャットのメッセージを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="0839d-131">List messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="0839d-132">チャット内のメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="0839d-132">Get message in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="0839d-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="0839d-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="0839d-134">チャット内の 1 つのメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="0839d-134">Get a single message in a chat.</span></span> |
|[<span data-ttu-id="0839d-135">ホストされているすべての画像を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="0839d-135">List all hosted images</span></span>](../api/chatmessagehostedimage-list-hostedimages.md) | <span data-ttu-id="0839d-136">[Hostedimage](../resources/chatmessagehostedimage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0839d-136">[hostedImage](../resources/chatmessagehostedimage.md) collection</span></span>| <span data-ttu-id="0839d-137">メッセージ内のすべてのホストされた画像を取得します。</span><span class="sxs-lookup"><span data-stu-id="0839d-137">Get all hosted images in a message.</span></span>|
|[<span data-ttu-id="0839d-138">ホストされた画像を取得する</span><span class="sxs-lookup"><span data-stu-id="0839d-138">Get hosted image</span></span>](../api/chatmessagehostedimage-get.md) | [<span data-ttu-id="0839d-139">hostedImage</span><span class="sxs-lookup"><span data-stu-id="0839d-139">hostedImage</span></span>](../resources/chatmessagehostedimage.md) | <span data-ttu-id="0839d-140">メッセージからホストされたイメージを取得します。</span><span class="sxs-lookup"><span data-stu-id="0839d-140">Get a hosted image from a message.</span></span>|
|[<span data-ttu-id="0839d-141">ホストされた画像バイトを取得する</span><span class="sxs-lookup"><span data-stu-id="0839d-141">Get hosted image bytes</span></span>](../api/chatmessagehostedimage-getbytes.md) | <span data-ttu-id="0839d-142">バイナリイメージデータ</span><span class="sxs-lookup"><span data-stu-id="0839d-142">binary image data</span></span> | <span data-ttu-id="0839d-143">メッセージからホストされたイメージのバイナリイメージデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="0839d-143">Get binary image data of a hosted image from a message.</span></span>|

## <a name="properties"></a><span data-ttu-id="0839d-144">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0839d-144">Properties</span></span>

| <span data-ttu-id="0839d-145">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0839d-145">Property</span></span>   | <span data-ttu-id="0839d-146">型</span><span class="sxs-lookup"><span data-stu-id="0839d-146">Type</span></span> |<span data-ttu-id="0839d-147">説明</span><span class="sxs-lookup"><span data-stu-id="0839d-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0839d-148">id</span><span class="sxs-lookup"><span data-stu-id="0839d-148">id</span></span>|<span data-ttu-id="0839d-149">String</span><span class="sxs-lookup"><span data-stu-id="0839d-149">String</span></span>| <span data-ttu-id="0839d-150">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="0839d-150">Read-only.</span></span> <span data-ttu-id="0839d-151">メッセージの一意の Id。</span><span class="sxs-lookup"><span data-stu-id="0839d-151">Unique Id of the message.</span></span>|
|<span data-ttu-id="0839d-152">replyToId</span><span class="sxs-lookup"><span data-stu-id="0839d-152">replyToId</span></span>| <span data-ttu-id="0839d-153">string</span><span class="sxs-lookup"><span data-stu-id="0839d-153">string</span></span> | <span data-ttu-id="0839d-154">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0839d-154">Read-only.</span></span> <span data-ttu-id="0839d-155">スレッドの親メッセージ/ルート メッセージの ID。</span><span class="sxs-lookup"><span data-stu-id="0839d-155">Id of the parent message/root message of the thread.</span></span> <span data-ttu-id="0839d-156">(チャットではなく、チャネルのメッセージにのみ適用)</span><span class="sxs-lookup"><span data-stu-id="0839d-156">(Only applies to messages in channels not chats)</span></span> |
|<span data-ttu-id="0839d-157">差出人</span><span class="sxs-lookup"><span data-stu-id="0839d-157">from</span></span>|[<span data-ttu-id="0839d-158">identitySet</span><span class="sxs-lookup"><span data-stu-id="0839d-158">identitySet</span></span>](identityset.md)| <span data-ttu-id="0839d-159">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0839d-159">Read only.</span></span> <span data-ttu-id="0839d-160">メッセージの送信者の詳細。</span><span class="sxs-lookup"><span data-stu-id="0839d-160">Details of the sender of the message.</span></span>|
|<span data-ttu-id="0839d-161">etag</span><span class="sxs-lookup"><span data-stu-id="0839d-161">etag</span></span>| <span data-ttu-id="0839d-162">string</span><span class="sxs-lookup"><span data-stu-id="0839d-162">string</span></span> | <span data-ttu-id="0839d-163">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0839d-163">Read-only.</span></span> <span data-ttu-id="0839d-164">メッセージのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="0839d-164">Version number of the message.</span></span> |
|<span data-ttu-id="0839d-165">messageType</span><span class="sxs-lookup"><span data-stu-id="0839d-165">messageType</span></span>|<span data-ttu-id="0839d-166">chatMessageType</span><span class="sxs-lookup"><span data-stu-id="0839d-166">chatMessageType</span></span>|<span data-ttu-id="0839d-167">メッセージの種類。</span><span class="sxs-lookup"><span data-stu-id="0839d-167">The type of message.</span></span> <span data-ttu-id="0839d-168">使用可能な値は`message`次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="0839d-168">The possible values are: `message`.</span></span>|
|<span data-ttu-id="0839d-169">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0839d-169">createdDateTime</span></span>|<span data-ttu-id="0839d-170">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0839d-170">dateTimeOffset</span></span>|<span data-ttu-id="0839d-171">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0839d-171">Read only.</span></span> <span data-ttu-id="0839d-172">メッセージ作成時のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="0839d-172">Timestamp of when the message was created.</span></span>|
|<span data-ttu-id="0839d-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0839d-173">lastModifiedDateTime</span></span>|<span data-ttu-id="0839d-174">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0839d-174">dateTimeOffset</span></span>|<span data-ttu-id="0839d-175">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0839d-175">Read only.</span></span> <span data-ttu-id="0839d-176">メッセージが作成または編集されたときのタイムスタンプ (チャネル内のルートメッセージの場合)、または反応が追加または削除されたとき。</span><span class="sxs-lookup"><span data-stu-id="0839d-176">Timestamp of when the message is created or edited, including when a reply is made (if it's a root message in a channel) or a reaction is added or removed.</span></span> |
|<span data-ttu-id="0839d-177">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="0839d-177">deletedDateTime</span></span>|<span data-ttu-id="0839d-178">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0839d-178">dateTimeOffset</span></span>|<span data-ttu-id="0839d-179">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0839d-179">Read only.</span></span> <span data-ttu-id="0839d-180">メッセージが削除された時間のタイムスタンプ、または削除されていない場合は Null です。</span><span class="sxs-lookup"><span data-stu-id="0839d-180">Timestamp at which the message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="0839d-181">件名</span><span class="sxs-lookup"><span data-stu-id="0839d-181">subject</span></span>|<span data-ttu-id="0839d-182">string</span><span class="sxs-lookup"><span data-stu-id="0839d-182">string</span></span>| <span data-ttu-id="0839d-183">プレーン テキストでの、メッセージの件名です。</span><span class="sxs-lookup"><span data-stu-id="0839d-183">The subject of the message, in plaintext.</span></span>|
|<span data-ttu-id="0839d-184">本文</span><span class="sxs-lookup"><span data-stu-id="0839d-184">body</span></span>|[<span data-ttu-id="0839d-185">itemBody</span><span class="sxs-lookup"><span data-stu-id="0839d-185">itemBody</span></span>](itembody.md)|<span data-ttu-id="0839d-186">メッセージのコンテンツのプレーンテキスト/HTML 表記。</span><span class="sxs-lookup"><span data-stu-id="0839d-186">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="0839d-187">表記は、本文内の contentType によって指定されます。</span><span class="sxs-lookup"><span data-stu-id="0839d-187">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="0839d-188">メッセージに [chatMessageMention ](chatmessagemention.md) が含まれている場合、コンテンツは常に HTML で表示されます。</span><span class="sxs-lookup"><span data-stu-id="0839d-188">The content is always in HTML if the message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="0839d-189">summary</span><span class="sxs-lookup"><span data-stu-id="0839d-189">summary</span></span>|<span data-ttu-id="0839d-190">string</span><span class="sxs-lookup"><span data-stu-id="0839d-190">string</span></span>| <span data-ttu-id="0839d-191">プッシュ通知および概要ビューまたはフォールバック ビューに使用できるメッセージの概要テキスト。</span><span class="sxs-lookup"><span data-stu-id="0839d-191">Summary text of the message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="0839d-192">チャット メッセージではなく、チャネル メッセージにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="0839d-192">Only applies to channel messages, not chat messages.</span></span> |
|<span data-ttu-id="0839d-193">attachments</span><span class="sxs-lookup"><span data-stu-id="0839d-193">attachments</span></span>|<span data-ttu-id="0839d-194">[chatMessageAttachment](chatmessageattachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0839d-194">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="0839d-195">添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="0839d-195">Attached files.</span></span> <span data-ttu-id="0839d-196">添付ファイルは現在読み取り専用です。添付ファイルの送信はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0839d-196">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="0839d-197">mentions</span><span class="sxs-lookup"><span data-stu-id="0839d-197">mentions</span></span>|<span data-ttu-id="0839d-198">[chatMessageMention](chatmessagemention.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0839d-198">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="0839d-199">メッセージに記載されているエンティティの一覧。</span><span class="sxs-lookup"><span data-stu-id="0839d-199">List of entities mentioned in the message.</span></span> <span data-ttu-id="0839d-200">現在、user、bot、team、channel がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="0839d-200">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="0839d-201">importance</span><span class="sxs-lookup"><span data-stu-id="0839d-201">importance</span></span>| <span data-ttu-id="0839d-202">chatMessageImportance 度</span><span class="sxs-lookup"><span data-stu-id="0839d-202">chatMessageImportance</span></span> | <span data-ttu-id="0839d-203">メッセージの重要度です。</span><span class="sxs-lookup"><span data-stu-id="0839d-203">The importance of the message.</span></span> <span data-ttu-id="0839d-204">使用可能な値: `normal`、`high`、`urgent`。</span><span class="sxs-lookup"><span data-stu-id="0839d-204">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="0839d-205">reactions</span><span class="sxs-lookup"><span data-stu-id="0839d-205">reactions</span></span>| <span data-ttu-id="0839d-206">[chatMessageReaction](chatmessagereaction.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0839d-206">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="0839d-207">このメッセージに対する反応 (例: いいね!)。</span><span class="sxs-lookup"><span data-stu-id="0839d-207">Reactions for this message (for example, Like).</span></span>|
|<span data-ttu-id="0839d-208">locale</span><span class="sxs-lookup"><span data-stu-id="0839d-208">locale</span></span>|<span data-ttu-id="0839d-209">string</span><span class="sxs-lookup"><span data-stu-id="0839d-209">string</span></span>|<span data-ttu-id="0839d-210">クライアントに設定されたメッセージのロケール。</span><span class="sxs-lookup"><span data-stu-id="0839d-210">Locale of the message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0839d-211">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0839d-211">JSON representation</span></span>

<span data-ttu-id="0839d-212">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0839d-212">The following is a JSON representation of the resource.</span></span>

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
