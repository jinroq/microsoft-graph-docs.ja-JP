---
title: chatMessage リソースの種類
description: チャネルまたはチャット エンティティ内の個別のチャット メッセージを表します。 メッセージは、ルート メッセージまたはメッセージの中の **replyToId** プロパティに定義されているスレッドの一部にすることができます。
localization_priority: Priority
ms.openlocfilehash: f61668d8c3892482043dd7531a6699974a964527
ms.sourcegitcommit: d1a9e7c8e1376a99c5a5416257889ec113613a77
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/07/2019
ms.locfileid: "30458660"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="c286a-104">chatMessage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c286a-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c286a-105">[チャネル](channel.md)またはチャット エンティティ内の個別のチャット メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="c286a-105">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="c286a-106">メッセージは、ルート メッセージまたはメッセージの中の **replyToId** プロパティに定義されているスレッドの一部にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c286a-106">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="c286a-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c286a-107">Methods</span></span>

| <span data-ttu-id="c286a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c286a-108">Method</span></span>       | <span data-ttu-id="c286a-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c286a-109">Return Type</span></span>  |<span data-ttu-id="c286a-110">説明</span><span class="sxs-lookup"><span data-stu-id="c286a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c286a-111">チャネル メッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c286a-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="c286a-112">[chatmessage](chatmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c286a-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="c286a-113">チャネルのすべてのルート メッセージの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="c286a-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="c286a-114">チャネル メッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="c286a-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="c286a-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="c286a-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="c286a-116">チャネルからのルート メッセージを 1 件取得します。</span><span class="sxs-lookup"><span data-stu-id="c286a-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="c286a-117">メッセージへの返信を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c286a-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="c286a-118">[chatmessage](chatmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c286a-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="c286a-119">チャネル内のメッセージへの返信すべての一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="c286a-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="c286a-120">メッセージへの返信を取得する</span><span class="sxs-lookup"><span data-stu-id="c286a-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="c286a-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="c286a-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="c286a-122">チャネル内のメッセージへの返信を 1 件取得します。</span><span class="sxs-lookup"><span data-stu-id="c286a-122">Get a single reply to a message in a channel.</span></span>|
|<span data-ttu-id="c286a-123">[チャネル内でメッセージを送信する](../api/channel-post-chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="c286a-123">Use [Create a message in a channel](../api/channel-post-chatmessage.md) instead.</span></span> | [<span data-ttu-id="c286a-124">chatmessage</span><span class="sxs-lookup"><span data-stu-id="c286a-124">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="c286a-125">チャネル内で新しい最上位レベルのメッセージを作成します。</span><span class="sxs-lookup"><span data-stu-id="c286a-125">Use Create a message in a channel instead.</span></span>|
|<span data-ttu-id="c286a-126">[チャネル内のメッセージに返信する](../api/channel-post-messagereply.md)</span><span class="sxs-lookup"><span data-stu-id="c286a-126">Introduced the [Reply to a message in a channel](../api/channel-post-messagereply.md) API.</span></span> | [<span data-ttu-id="c286a-127">chatmessage</span><span class="sxs-lookup"><span data-stu-id="c286a-127">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="c286a-128">チャネル内の既存メッセージに返信します。</span><span class="sxs-lookup"><span data-stu-id="c286a-128">Reply to an existing message in a channel.</span></span>|


## <a name="properties"></a><span data-ttu-id="c286a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c286a-129">Properties</span></span>
| <span data-ttu-id="c286a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c286a-130">Property</span></span>     | <span data-ttu-id="c286a-131">型</span><span class="sxs-lookup"><span data-stu-id="c286a-131">Type</span></span>   |<span data-ttu-id="c286a-132">説明</span><span class="sxs-lookup"><span data-stu-id="c286a-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c286a-133">id</span><span class="sxs-lookup"><span data-stu-id="c286a-133">id</span></span>|<span data-ttu-id="c286a-134">String</span><span class="sxs-lookup"><span data-stu-id="c286a-134">String</span></span>| <span data-ttu-id="c286a-135">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c286a-135">Read-only.</span></span> <span data-ttu-id="c286a-136">メッセージの一意の ID。</span><span class="sxs-lookup"><span data-stu-id="c286a-136">Unique ID of the message.</span></span>|
|<span data-ttu-id="c286a-137">replyToId</span><span class="sxs-lookup"><span data-stu-id="c286a-137">replyToId</span></span>| <span data-ttu-id="c286a-138">string</span><span class="sxs-lookup"><span data-stu-id="c286a-138">string</span></span> | <span data-ttu-id="c286a-139">スレッドの親メッセージ/ルート メッセージの ID</span><span class="sxs-lookup"><span data-stu-id="c286a-139">Id of the parent message/root message of the thread</span></span> |
|<span data-ttu-id="c286a-140">from</span><span class="sxs-lookup"><span data-stu-id="c286a-140">from</span></span>|[<span data-ttu-id="c286a-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="c286a-141">identitySet</span></span>](identityset.md)| <span data-ttu-id="c286a-142">メッセージの送信者の詳細</span><span class="sxs-lookup"><span data-stu-id="c286a-142">Details of the sender of the message</span></span>|
|<span data-ttu-id="c286a-143">etag</span><span class="sxs-lookup"><span data-stu-id="c286a-143">etag</span></span>| <span data-ttu-id="c286a-144">string</span><span class="sxs-lookup"><span data-stu-id="c286a-144">string</span></span> | <span data-ttu-id="c286a-145">メッセージのバージョン番号</span><span class="sxs-lookup"><span data-stu-id="c286a-145">Version number of the message</span></span> |
|<span data-ttu-id="c286a-146">messageType</span><span class="sxs-lookup"><span data-stu-id="c286a-146">messageType</span></span>|<span data-ttu-id="c286a-147">String</span><span class="sxs-lookup"><span data-stu-id="c286a-147">String</span></span>|<span data-ttu-id="c286a-148">メッセージの種類。現在サポートされている値: message、chatEvent、Typing</span><span class="sxs-lookup"><span data-stu-id="c286a-148">The type of message, current supported values are: message, chatEvent, Typing</span></span>|
|<span data-ttu-id="c286a-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c286a-149">createdDateTime</span></span>|<span data-ttu-id="c286a-150">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c286a-150">dateTimeOffset</span></span>|<span data-ttu-id="c286a-151">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c286a-151">Read only.</span></span> <span data-ttu-id="c286a-152">メッセージ作成時のタイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="c286a-152">Timestamp of when the message was created</span></span>|
|<span data-ttu-id="c286a-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c286a-153">lastModifiedDateTime</span></span>|<span data-ttu-id="c286a-154">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c286a-154">dateTimeOffset</span></span>|<span data-ttu-id="c286a-155">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c286a-155">Read only.</span></span> <span data-ttu-id="c286a-156">メッセージ編集/更新時のタイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="c286a-156">Timestamp of when the message was edited/updated</span></span>|
|<span data-ttu-id="c286a-157">deleted</span><span class="sxs-lookup"><span data-stu-id="c286a-157">deleted</span></span>|<span data-ttu-id="c286a-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="c286a-158">Boolean</span></span>|<span data-ttu-id="c286a-159">メッセージが削除済み (回復可能) かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c286a-159">Indicates whether a message has been soft deleted</span></span>|
|<span data-ttu-id="c286a-160">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="c286a-160">deletedDateTime</span></span>|<span data-ttu-id="c286a-161">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c286a-161">dateTimeOffset</span></span>|<span data-ttu-id="c286a-162">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c286a-162">Read only.</span></span> <span data-ttu-id="c286a-163">メッセージ削除時のタイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="c286a-163">Timestamp at which the message was deleted</span></span> |
|<span data-ttu-id="c286a-164">subject</span><span class="sxs-lookup"><span data-stu-id="c286a-164">subject</span></span>|<span data-ttu-id="c286a-165">string</span><span class="sxs-lookup"><span data-stu-id="c286a-165">string</span></span>|<span data-ttu-id="c286a-166">メッセージの件名。</span><span class="sxs-lookup"><span data-stu-id="c286a-166">Message subject line.</span></span> <span data-ttu-id="c286a-167">省略可能</span><span class="sxs-lookup"><span data-stu-id="c286a-167">Optional</span></span>|
|<span data-ttu-id="c286a-168">body</span><span class="sxs-lookup"><span data-stu-id="c286a-168">body</span></span>|[<span data-ttu-id="c286a-169">itemBody</span><span class="sxs-lookup"><span data-stu-id="c286a-169">itemBody</span></span>](itembody.md)|<span data-ttu-id="c286a-170">メッセージのコンテンツのプレーンテキスト/HTML 表記。</span><span class="sxs-lookup"><span data-stu-id="c286a-170">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="c286a-171">既定ではプレーンテキストを返しますが、クエリ パラメーターの一部としてアプリケーションで HTML を選択できます</span><span class="sxs-lookup"><span data-stu-id="c286a-171">Returns plain text by default, application can choose HTML as part of a query param</span></span>|
|<span data-ttu-id="c286a-172">summary</span><span class="sxs-lookup"><span data-stu-id="c286a-172">summary</span></span>|<span data-ttu-id="c286a-173">string</span><span class="sxs-lookup"><span data-stu-id="c286a-173">string</span></span>|<span data-ttu-id="c286a-174">プッシュ通知および概要ビューまたはフォールバック ビューに使用できるメッセージの概要テキスト</span><span class="sxs-lookup"><span data-stu-id="c286a-174">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="c286a-175">mentions</span><span class="sxs-lookup"><span data-stu-id="c286a-175">mentions</span></span>|<span data-ttu-id="c286a-176">[chatMessageMention](chatmention.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c286a-176">[chatMessageMention](chatmention.md) collection</span></span>| <span data-ttu-id="c286a-177">メッセージに記載されているエンティティの一覧。</span><span class="sxs-lookup"><span data-stu-id="c286a-177">List of entities mentioned in the message.</span></span> <span data-ttu-id="c286a-178">現在、user、bot、team、channel がサポートされています</span><span class="sxs-lookup"><span data-stu-id="c286a-178">Currently supports user, bot, team, channel</span></span>|
|<span data-ttu-id="c286a-179">importance</span><span class="sxs-lookup"><span data-stu-id="c286a-179">importance</span></span>| <span data-ttu-id="c286a-180">string</span><span class="sxs-lookup"><span data-stu-id="c286a-180">string</span></span> | <span data-ttu-id="c286a-181">メッセージの重要度: 通常、高</span><span class="sxs-lookup"><span data-stu-id="c286a-181">The importance of the message: Normal, High</span></span>|
|<span data-ttu-id="c286a-182">reactions</span><span class="sxs-lookup"><span data-stu-id="c286a-182">reactions</span></span>| <span data-ttu-id="c286a-183">[chatMessageReaction](chatreaction.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c286a-183">[chatMessageReaction](chatreaction.md) collection</span></span> | <span data-ttu-id="c286a-184">このメッセージに対する反応 (例: いいね!)</span><span class="sxs-lookup"><span data-stu-id="c286a-184">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="c286a-185">locale</span><span class="sxs-lookup"><span data-stu-id="c286a-185">locale</span></span>|<span data-ttu-id="c286a-186">string</span><span class="sxs-lookup"><span data-stu-id="c286a-186">string</span></span>|<span data-ttu-id="c286a-187">クライアントに設定されたメッセージのロケール</span><span class="sxs-lookup"><span data-stu-id="c286a-187">Locale of the message set by the client</span></span>|
|<span data-ttu-id="c286a-188">attachments</span><span class="sxs-lookup"><span data-stu-id="c286a-188">attachments</span></span>|<span data-ttu-id="c286a-189">[chatMessageAttachment](chatattachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c286a-189">[chatMessageAttachment](chatattachment.md) collection</span></span> |<span data-ttu-id="c286a-190">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="c286a-190">Attached files</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c286a-191">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c286a-191">JSON representation</span></span>

<span data-ttu-id="c286a-192">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c286a-192">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
