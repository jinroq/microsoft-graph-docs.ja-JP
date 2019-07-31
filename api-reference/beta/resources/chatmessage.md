---
title: chatMessage リソースの種類
description: チャネルまたはチャット エンティティ内の個別のチャット メッセージを表します。 メッセージは、ルート メッセージまたはメッセージの中の **replyToId** プロパティに定義されているスレッドの一部にすることができます。
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: f807c45fcff2a5e2ea928105ed970d426cfdc1f3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974032"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="a966e-104">chatMessage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a966e-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a966e-105">[チャネル](channel.md)または[チャット](chat.md)内の個別のチャット メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="a966e-105">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span>
<span data-ttu-id="a966e-106">メッセージは、ルート メッセージまたはメッセージの中の **replyToId** プロパティに定義されているスレッドの一部にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a966e-106">The message can be a root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="a966e-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a966e-107">Methods</span></span>

| <span data-ttu-id="a966e-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a966e-108">Method</span></span>       | <span data-ttu-id="a966e-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a966e-109">Return Type</span></span>  |<span data-ttu-id="a966e-110">説明</span><span class="sxs-lookup"><span data-stu-id="a966e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a966e-111">チャネル メッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a966e-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="a966e-112">[chatMessage](chatmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a966e-112">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="a966e-113">チャネル内のすべてのルートメッセージのリスト。</span><span class="sxs-lookup"><span data-stu-id="a966e-113">List of all root messages in a channel.</span></span>|
|[<span data-ttu-id="a966e-114">チャネル メッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="a966e-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="a966e-115">chatMessage</span><span class="sxs-lookup"><span data-stu-id="a966e-115">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="a966e-116">チャネルからのルート メッセージを 1 件取得します。</span><span class="sxs-lookup"><span data-stu-id="a966e-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="a966e-117">メッセージへの返信を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a966e-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="a966e-118">[chatMessage](chatmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a966e-118">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="a966e-119">チャネル内のメッセージへのすべての返信のリスト。</span><span class="sxs-lookup"><span data-stu-id="a966e-119">List of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="a966e-120">メッセージへの返信を取得する</span><span class="sxs-lookup"><span data-stu-id="a966e-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="a966e-121">chatMessage</span><span class="sxs-lookup"><span data-stu-id="a966e-121">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="a966e-122">チャネル内のメッセージへの返信を 1 件取得します。</span><span class="sxs-lookup"><span data-stu-id="a966e-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="a966e-123">チャネルでの chatMessage の作成</span><span class="sxs-lookup"><span data-stu-id="a966e-123">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="a966e-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="a966e-124">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="a966e-125">チャネル内で新しい最上位レベルのメッセージを作成します。</span><span class="sxs-lookup"><span data-stu-id="a966e-125">Create a new top-level message in a channel.</span></span>|
|[<span data-ttu-id="a966e-126">チャネル内のメッセージに返信する</span><span class="sxs-lookup"><span data-stu-id="a966e-126">Reply to a message in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="a966e-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="a966e-127">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="a966e-128">チャネル内の既存メッセージに返信します。</span><span class="sxs-lookup"><span data-stu-id="a966e-128">Reply to an existing message in a channel.</span></span>|
|[<span data-ttu-id="a966e-129">チャット内のメッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a966e-129">List messages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="a966e-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="a966e-130">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="a966e-131">1:1 またはグループチャットのメッセージを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="a966e-131">List messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="a966e-132">チャット内のメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="a966e-132">Get message in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="a966e-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="a966e-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="a966e-134">チャット内の 1 つのメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="a966e-134">Get a single message in a chat.</span></span> |
|[<span data-ttu-id="a966e-135">ホストされているすべての画像を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a966e-135">List all hosted images</span></span>](../api/chatmessagehostedimage-list-hostedimages.md) | <span data-ttu-id="a966e-136">[Hostedimage](../resources/chatmessagehostedimage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a966e-136">[hostedImage](../resources/chatmessagehostedimage.md) collection</span></span>| <span data-ttu-id="a966e-137">メッセージ内のすべてのホストされた画像を取得します。</span><span class="sxs-lookup"><span data-stu-id="a966e-137">Get all hosted images in a message.</span></span>|
|[<span data-ttu-id="a966e-138">ホストされた画像を取得する</span><span class="sxs-lookup"><span data-stu-id="a966e-138">Get hosted image</span></span>](../api/chatmessagehostedimage-get.md) | [<span data-ttu-id="a966e-139">hostedImage</span><span class="sxs-lookup"><span data-stu-id="a966e-139">hostedImage</span></span>](../resources/chatmessagehostedimage.md) | <span data-ttu-id="a966e-140">メッセージからホストされたイメージを取得します。</span><span class="sxs-lookup"><span data-stu-id="a966e-140">Get a hosted image from a message.</span></span>|
|[<span data-ttu-id="a966e-141">ホストされた画像バイトを取得する</span><span class="sxs-lookup"><span data-stu-id="a966e-141">Get hosted image bytes</span></span>](../api/chatmessagehostedimage-getbytes.md) | <span data-ttu-id="a966e-142">バイナリイメージデータ</span><span class="sxs-lookup"><span data-stu-id="a966e-142">binary image data</span></span> | <span data-ttu-id="a966e-143">メッセージからホストされたイメージのバイナリイメージデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="a966e-143">Get binary image data of a hosted image from a message.</span></span>|

## <a name="properties"></a><span data-ttu-id="a966e-144">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a966e-144">Properties</span></span>

| <span data-ttu-id="a966e-145">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a966e-145">Property</span></span>   | <span data-ttu-id="a966e-146">型</span><span class="sxs-lookup"><span data-stu-id="a966e-146">Type</span></span> |<span data-ttu-id="a966e-147">説明</span><span class="sxs-lookup"><span data-stu-id="a966e-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a966e-148">id</span><span class="sxs-lookup"><span data-stu-id="a966e-148">id</span></span>|<span data-ttu-id="a966e-149">String</span><span class="sxs-lookup"><span data-stu-id="a966e-149">String</span></span>| <span data-ttu-id="a966e-150">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="a966e-150">Read-only.</span></span> <span data-ttu-id="a966e-151">メッセージの一意の Id。</span><span class="sxs-lookup"><span data-stu-id="a966e-151">Unique Id of the message.</span></span>|
|<span data-ttu-id="a966e-152">replyToId</span><span class="sxs-lookup"><span data-stu-id="a966e-152">replyToId</span></span>| <span data-ttu-id="a966e-153">string</span><span class="sxs-lookup"><span data-stu-id="a966e-153">string</span></span> | <span data-ttu-id="a966e-154">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a966e-154">Read-only.</span></span> <span data-ttu-id="a966e-155">スレッドの親メッセージ/ルート メッセージの ID。</span><span class="sxs-lookup"><span data-stu-id="a966e-155">Id of the parent message/root message of the thread.</span></span> <span data-ttu-id="a966e-156">(チャットではなく、チャネルのメッセージにのみ適用)</span><span class="sxs-lookup"><span data-stu-id="a966e-156">(Only applies to messages in channels not chats)</span></span> |
|<span data-ttu-id="a966e-157">差出人</span><span class="sxs-lookup"><span data-stu-id="a966e-157">from</span></span>|[<span data-ttu-id="a966e-158">identitySet</span><span class="sxs-lookup"><span data-stu-id="a966e-158">identitySet</span></span>](identityset.md)| <span data-ttu-id="a966e-159">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a966e-159">Read only.</span></span> <span data-ttu-id="a966e-160">メッセージの送信者の詳細。</span><span class="sxs-lookup"><span data-stu-id="a966e-160">Details of the sender of the message.</span></span>|
|<span data-ttu-id="a966e-161">etag</span><span class="sxs-lookup"><span data-stu-id="a966e-161">etag</span></span>| <span data-ttu-id="a966e-162">string</span><span class="sxs-lookup"><span data-stu-id="a966e-162">string</span></span> | <span data-ttu-id="a966e-163">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a966e-163">Read-only.</span></span> <span data-ttu-id="a966e-164">メッセージのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="a966e-164">Version number of the message.</span></span> |
|<span data-ttu-id="a966e-165">messageType</span><span class="sxs-lookup"><span data-stu-id="a966e-165">messageType</span></span>|<span data-ttu-id="a966e-166">chatMessageType</span><span class="sxs-lookup"><span data-stu-id="a966e-166">chatMessageType</span></span>|<span data-ttu-id="a966e-167">メッセージの種類。</span><span class="sxs-lookup"><span data-stu-id="a966e-167">The type of message.</span></span> <span data-ttu-id="a966e-168">使用可能な値は`message`次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="a966e-168">The possible values are: `message`.</span></span>|
|<span data-ttu-id="a966e-169">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a966e-169">createdDateTime</span></span>|<span data-ttu-id="a966e-170">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a966e-170">dateTimeOffset</span></span>|<span data-ttu-id="a966e-171">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a966e-171">Read only.</span></span> <span data-ttu-id="a966e-172">メッセージ作成時のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="a966e-172">Timestamp of when the message was created.</span></span>|
|<span data-ttu-id="a966e-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a966e-173">lastModifiedDateTime</span></span>|<span data-ttu-id="a966e-174">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a966e-174">dateTimeOffset</span></span>|<span data-ttu-id="a966e-175">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a966e-175">Read only.</span></span> <span data-ttu-id="a966e-176">メッセージが作成または編集されたときのタイムスタンプ (チャネル内のルートメッセージの場合)、または反応が追加または削除されたとき。</span><span class="sxs-lookup"><span data-stu-id="a966e-176">Timestamp of when the message is created or edited, including when a reply is made (if it's a root message in a channel) or a reaction is added or removed.</span></span> |
|<span data-ttu-id="a966e-177">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="a966e-177">deletedDateTime</span></span>|<span data-ttu-id="a966e-178">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a966e-178">dateTimeOffset</span></span>|<span data-ttu-id="a966e-179">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a966e-179">Read only.</span></span> <span data-ttu-id="a966e-180">メッセージが削除された時間のタイムスタンプ、または削除されていない場合は Null です。</span><span class="sxs-lookup"><span data-stu-id="a966e-180">Timestamp at which the message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="a966e-181">件名</span><span class="sxs-lookup"><span data-stu-id="a966e-181">subject</span></span>|<span data-ttu-id="a966e-182">string</span><span class="sxs-lookup"><span data-stu-id="a966e-182">string</span></span>| <span data-ttu-id="a966e-183">プレーン テキストでの、メッセージの件名です。</span><span class="sxs-lookup"><span data-stu-id="a966e-183">The subject of the message, in plaintext.</span></span>|
|<span data-ttu-id="a966e-184">本文</span><span class="sxs-lookup"><span data-stu-id="a966e-184">body</span></span>|[<span data-ttu-id="a966e-185">itemBody</span><span class="sxs-lookup"><span data-stu-id="a966e-185">itemBody</span></span>](itembody.md)|<span data-ttu-id="a966e-186">メッセージのコンテンツのプレーンテキスト/HTML 表記。</span><span class="sxs-lookup"><span data-stu-id="a966e-186">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="a966e-187">表記は、本文内の contentType によって指定されます。</span><span class="sxs-lookup"><span data-stu-id="a966e-187">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="a966e-188">メッセージに [chatMessageMention ](chatmessagemention.md) が含まれている場合、コンテンツは常に HTML で表示されます。</span><span class="sxs-lookup"><span data-stu-id="a966e-188">The content is always in HTML if the message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="a966e-189">summary</span><span class="sxs-lookup"><span data-stu-id="a966e-189">summary</span></span>|<span data-ttu-id="a966e-190">string</span><span class="sxs-lookup"><span data-stu-id="a966e-190">string</span></span>| <span data-ttu-id="a966e-191">プッシュ通知および概要ビューまたはフォールバック ビューに使用できるメッセージの概要テキスト。</span><span class="sxs-lookup"><span data-stu-id="a966e-191">Summary text of the message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="a966e-192">チャット メッセージではなく、チャネル メッセージにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="a966e-192">Only applies to channel messages, not chat messages.</span></span> |
|<span data-ttu-id="a966e-193">attachments</span><span class="sxs-lookup"><span data-stu-id="a966e-193">attachments</span></span>|<span data-ttu-id="a966e-194">[chatMessageAttachment](chatmessageattachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a966e-194">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="a966e-195">添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="a966e-195">Attached files.</span></span> <span data-ttu-id="a966e-196">添付ファイルは現在読み取り専用です。添付ファイルの送信はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a966e-196">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="a966e-197">mentions</span><span class="sxs-lookup"><span data-stu-id="a966e-197">mentions</span></span>|<span data-ttu-id="a966e-198">[chatMessageMention](chatmessagemention.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a966e-198">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="a966e-199">メッセージに記載されているエンティティの一覧。</span><span class="sxs-lookup"><span data-stu-id="a966e-199">List of entities mentioned in the message.</span></span> <span data-ttu-id="a966e-200">現在、user、bot、team、channel がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="a966e-200">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="a966e-201">importance</span><span class="sxs-lookup"><span data-stu-id="a966e-201">importance</span></span>| <span data-ttu-id="a966e-202">chatMessageImportance 度</span><span class="sxs-lookup"><span data-stu-id="a966e-202">chatMessageImportance</span></span> | <span data-ttu-id="a966e-203">メッセージの重要度です。</span><span class="sxs-lookup"><span data-stu-id="a966e-203">The importance of the message.</span></span> <span data-ttu-id="a966e-204">使用可能な値: `normal`、`high`、`urgent`。</span><span class="sxs-lookup"><span data-stu-id="a966e-204">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="a966e-205">reactions</span><span class="sxs-lookup"><span data-stu-id="a966e-205">reactions</span></span>| <span data-ttu-id="a966e-206">[chatMessageReaction](chatmessagereaction.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a966e-206">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="a966e-207">このメッセージに対する反応 (例: いいね!)。</span><span class="sxs-lookup"><span data-stu-id="a966e-207">Reactions for this message (for example, Like).</span></span>|
|<span data-ttu-id="a966e-208">locale</span><span class="sxs-lookup"><span data-stu-id="a966e-208">locale</span></span>|<span data-ttu-id="a966e-209">string</span><span class="sxs-lookup"><span data-stu-id="a966e-209">string</span></span>|<span data-ttu-id="a966e-210">クライアントに設定されたメッセージのロケール。</span><span class="sxs-lookup"><span data-stu-id="a966e-210">Locale of the message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a966e-211">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a966e-211">JSON representation</span></span>

<span data-ttu-id="a966e-212">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a966e-212">The following is a JSON representation of the resource.</span></span>

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
