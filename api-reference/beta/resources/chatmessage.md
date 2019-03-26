---
title: chatMessage リソースの種類
description: チャネルまたはチャット エンティティ内の個別のチャット メッセージを表します。 メッセージは、ルート メッセージまたはメッセージの中の **replyToId** プロパティに定義されているスレッドの一部にすることができます。
localization_priority: Priority
ms.openlocfilehash: 1f1e38e53a7c7ad1b0452c9facc6d7f97314094e
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/26/2019
ms.locfileid: "30799999"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="af507-104">chatMessage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="af507-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af507-105">[チャネル](channel.md)またはチャット エンティティ内の個別のチャット メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="af507-105">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="af507-106">メッセージは、ルート メッセージまたはメッセージの中の **replyToId** プロパティに定義されているスレッドの一部にすることができます。</span><span class="sxs-lookup"><span data-stu-id="af507-106">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="af507-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="af507-107">Methods</span></span>

| <span data-ttu-id="af507-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="af507-108">Method</span></span>       | <span data-ttu-id="af507-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="af507-109">Return Type</span></span>  |<span data-ttu-id="af507-110">説明</span><span class="sxs-lookup"><span data-stu-id="af507-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="af507-111">チャネル メッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="af507-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="af507-112">[chatmessage](chatmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="af507-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="af507-113">チャネルのすべてのルート メッセージの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="af507-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="af507-114">チャネル メッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="af507-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="af507-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="af507-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="af507-116">チャネルからのルート メッセージを 1 件取得します。</span><span class="sxs-lookup"><span data-stu-id="af507-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="af507-117">メッセージへの返信を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="af507-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="af507-118">[chatmessage](chatmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="af507-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="af507-119">チャネル内のメッセージへの返信すべての一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="af507-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="af507-120">メッセージへの返信を取得する</span><span class="sxs-lookup"><span data-stu-id="af507-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="af507-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="af507-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="af507-122">チャネル内のメッセージへの返信を 1 件取得します。</span><span class="sxs-lookup"><span data-stu-id="af507-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="af507-123">チャネル内でメッセージを送信する</span><span class="sxs-lookup"><span data-stu-id="af507-123">Send a message in a channel</span></span>](../api/channel-post-chatmessage.md) | [<span data-ttu-id="af507-124">chatmessage</span><span class="sxs-lookup"><span data-stu-id="af507-124">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="af507-125">チャネル内で新しい最上位レベルのメッセージを作成します。</span><span class="sxs-lookup"><span data-stu-id="af507-125">Create a new top-level message in a channel.</span></span>|
|[<span data-ttu-id="af507-126">チャネル内のメッセージに返信する</span><span class="sxs-lookup"><span data-stu-id="af507-126">Reply to a message in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="af507-127">chatmessage</span><span class="sxs-lookup"><span data-stu-id="af507-127">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="af507-128">チャネル内の既存メッセージに返信します。</span><span class="sxs-lookup"><span data-stu-id="af507-128">Reply to an existing message in a channel.</span></span>|


## <a name="properties"></a><span data-ttu-id="af507-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="af507-129">Properties</span></span>
| <span data-ttu-id="af507-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="af507-130">Property</span></span>     | <span data-ttu-id="af507-131">型</span><span class="sxs-lookup"><span data-stu-id="af507-131">Type</span></span>   |<span data-ttu-id="af507-132">説明</span><span class="sxs-lookup"><span data-stu-id="af507-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af507-133">id</span><span class="sxs-lookup"><span data-stu-id="af507-133">id</span></span>|<span data-ttu-id="af507-134">String</span><span class="sxs-lookup"><span data-stu-id="af507-134">String</span></span>| <span data-ttu-id="af507-135">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="af507-135">Read-only.</span></span> <span data-ttu-id="af507-136">メッセージの一意の ID。</span><span class="sxs-lookup"><span data-stu-id="af507-136">Unique ID of the message.</span></span>|
|<span data-ttu-id="af507-137">replyToId</span><span class="sxs-lookup"><span data-stu-id="af507-137">replyToId</span></span>| <span data-ttu-id="af507-138">string</span><span class="sxs-lookup"><span data-stu-id="af507-138">string</span></span> | <span data-ttu-id="af507-139">スレッドの親メッセージ/ルート メッセージの ID。</span><span class="sxs-lookup"><span data-stu-id="af507-139">Id of the parent message/root message of the thread.</span></span> |
|<span data-ttu-id="af507-140">from</span><span class="sxs-lookup"><span data-stu-id="af507-140">from</span></span>|[<span data-ttu-id="af507-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="af507-141">identitySet</span></span>](identityset.md)| <span data-ttu-id="af507-142">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="af507-142">Read only.</span></span> <span data-ttu-id="af507-143">メッセージの送信者の詳細。</span><span class="sxs-lookup"><span data-stu-id="af507-143">Details of the sender of the message.</span></span>|
|<span data-ttu-id="af507-144">etag</span><span class="sxs-lookup"><span data-stu-id="af507-144">etag</span></span>| <span data-ttu-id="af507-145">string</span><span class="sxs-lookup"><span data-stu-id="af507-145">string</span></span> | <span data-ttu-id="af507-146">メッセージのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="af507-146">Version number of the message.</span></span> |
|<span data-ttu-id="af507-147">messageType</span><span class="sxs-lookup"><span data-stu-id="af507-147">messageType</span></span>|<span data-ttu-id="af507-148">String</span><span class="sxs-lookup"><span data-stu-id="af507-148">String</span></span>|<span data-ttu-id="af507-149">メッセージの種類。現在サポートされている値は message、chatEvent、Typing。</span><span class="sxs-lookup"><span data-stu-id="af507-149">The type of message, current supported values are: message, chatEvent, Typing.</span></span>|
|<span data-ttu-id="af507-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="af507-150">createdDateTime</span></span>|<span data-ttu-id="af507-151">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af507-151">dateTimeOffset</span></span>|<span data-ttu-id="af507-152">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="af507-152">Read only.</span></span> <span data-ttu-id="af507-153">メッセージ作成時のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="af507-153">Timestamp of when the message was created.</span></span>|
|<span data-ttu-id="af507-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="af507-154">lastModifiedDateTime</span></span>|<span data-ttu-id="af507-155">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af507-155">dateTimeOffset</span></span>|<span data-ttu-id="af507-156">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="af507-156">Read only.</span></span> <span data-ttu-id="af507-157">メッセージ編集/更新時のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="af507-157">Timestamp of when the message was edited/updated.</span></span>|
|<span data-ttu-id="af507-158">deleted</span><span class="sxs-lookup"><span data-stu-id="af507-158">deleted</span></span>|<span data-ttu-id="af507-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="af507-159">Boolean</span></span>|<span data-ttu-id="af507-160">メッセージが削除済み (回復可能) かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="af507-160">Indicates whether a message has been soft deleted.</span></span>|
|<span data-ttu-id="af507-161">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="af507-161">deletedDateTime</span></span>|<span data-ttu-id="af507-162">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af507-162">dateTimeOffset</span></span>|<span data-ttu-id="af507-163">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="af507-163">Read only.</span></span> <span data-ttu-id="af507-164">メッセージが削除された時間のタイムスタンプ、または削除されていない場合は Null です。</span><span class="sxs-lookup"><span data-stu-id="af507-164">Timestamp at which the message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="af507-165">body</span><span class="sxs-lookup"><span data-stu-id="af507-165">body</span></span>|[<span data-ttu-id="af507-166">itemBody</span><span class="sxs-lookup"><span data-stu-id="af507-166">itemBody</span></span>](itembody.md)|<span data-ttu-id="af507-167">メッセージのコンテンツのプレーンテキスト/HTML 表記。</span><span class="sxs-lookup"><span data-stu-id="af507-167">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="af507-168">既定ではプレーンテキストを返しますが、クエリ パラメーターの一部としてアプリケーションで HTML を選択できます</span><span class="sxs-lookup"><span data-stu-id="af507-168">Returns plain text by default, application can choose HTML as part of a query param</span></span>|
|<span data-ttu-id="af507-169">summary</span><span class="sxs-lookup"><span data-stu-id="af507-169">summary</span></span>|<span data-ttu-id="af507-170">string</span><span class="sxs-lookup"><span data-stu-id="af507-170">string</span></span>|<span data-ttu-id="af507-171">プッシュ通知および概要ビューまたはフォールバック ビューに使用できるメッセージの概要テキスト</span><span class="sxs-lookup"><span data-stu-id="af507-171">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="af507-172">mentions</span><span class="sxs-lookup"><span data-stu-id="af507-172">mentions</span></span>|<span data-ttu-id="af507-173">[chatMessageMention](chatmention.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="af507-173">[chatMessageMention](chatmention.md) collection</span></span>| <span data-ttu-id="af507-174">メッセージに記載されているエンティティの一覧。</span><span class="sxs-lookup"><span data-stu-id="af507-174">List of entities mentioned in the message.</span></span> <span data-ttu-id="af507-175">現在、user、bot、team、channel がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="af507-175">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="af507-176">importance</span><span class="sxs-lookup"><span data-stu-id="af507-176">importance</span></span>| <span data-ttu-id="af507-177">string</span><span class="sxs-lookup"><span data-stu-id="af507-177">string</span></span> | <span data-ttu-id="af507-178">メッセージの重要度: 通常、高。</span><span class="sxs-lookup"><span data-stu-id="af507-178">The importance of the message: Normal, High.</span></span>|
|<span data-ttu-id="af507-179">reactions</span><span class="sxs-lookup"><span data-stu-id="af507-179">reactions</span></span>| <span data-ttu-id="af507-180">[chatMessageReaction](chatreaction.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="af507-180">[chatMessageReaction](chatreaction.md) collection</span></span> | <span data-ttu-id="af507-181">このメッセージに対する反応 (例: いいね!)</span><span class="sxs-lookup"><span data-stu-id="af507-181">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="af507-182">locale</span><span class="sxs-lookup"><span data-stu-id="af507-182">locale</span></span>|<span data-ttu-id="af507-183">string</span><span class="sxs-lookup"><span data-stu-id="af507-183">string</span></span>|<span data-ttu-id="af507-184">クライアントに設定されたメッセージのロケール</span><span class="sxs-lookup"><span data-stu-id="af507-184">Locale of the message set by the client</span></span>|
|<span data-ttu-id="af507-185">attachments</span><span class="sxs-lookup"><span data-stu-id="af507-185">attachments</span></span>|<span data-ttu-id="af507-186">[chatMessageAttachment](chatattachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="af507-186">[chatMessageAttachment](chatattachment.md) collection</span></span> |<span data-ttu-id="af507-187">添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="af507-187">Attached files.</span></span> <span data-ttu-id="af507-188">添付ファイルは現在読み取り専用です。添付ファイルの送信はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af507-188">Attachments are currently read-only – sending attachments is not supported.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="af507-189">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="af507-189">JSON representation</span></span>

<span data-ttu-id="af507-190">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="af507-190">The following is a JSON representation of the resource.</span></span>

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
