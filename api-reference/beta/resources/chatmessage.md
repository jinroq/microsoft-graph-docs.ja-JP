---
title: chatMessage リソースの種類
description: チャネルまたはチャット エンティティ内の個別のチャット メッセージを表します。 メッセージは、ルート メッセージまたはメッセージの中の **replyToId** プロパティに定義されているスレッドの一部にすることができます。
localization_priority: Priority
ms.openlocfilehash: ef91281eff0cc61f992f659bd33debec03841bb4
ms.sourcegitcommit: a1f1e59ee568340bfabdb524e01cff7860bcc862
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/05/2019
ms.locfileid: "29735580"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="0cd9a-104">chatMessage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0cd9a-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cd9a-105">[チャネル](channel.md)またはチャット エンティティ内の個別のチャット メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="0cd9a-105">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="0cd9a-106">メッセージは、ルート メッセージまたはメッセージの中の **replyToId** プロパティに定義されているスレッドの一部にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0cd9a-106">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="0cd9a-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0cd9a-107">Methods</span></span>

| <span data-ttu-id="0cd9a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0cd9a-108">Method</span></span>       | <span data-ttu-id="0cd9a-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0cd9a-109">Return Type</span></span>  |<span data-ttu-id="0cd9a-110">説明</span><span class="sxs-lookup"><span data-stu-id="0cd9a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0cd9a-111">チャネル メッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="0cd9a-111">List channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="0cd9a-112">[chatmessage](chatmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0cd9a-112">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="0cd9a-113">チャネルのすべてのルート メッセージの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="0cd9a-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="0cd9a-114">チャネル メッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="0cd9a-114">Get channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="0cd9a-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="0cd9a-115">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="0cd9a-116">チャネルからのルート メッセージを 1 件取得します。</span><span class="sxs-lookup"><span data-stu-id="0cd9a-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="0cd9a-117">メッセージへの返信を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="0cd9a-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="0cd9a-118">[chatmessage](chatmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0cd9a-118">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="0cd9a-119">チャネル内のメッセージへの返信すべての一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="0cd9a-119">Get the list of all replies to a message in channel.</span></span>|
|<span data-ttu-id="0cd9a-120">[メッセージへの返信を取得する](../api/channel-get-messagereply.md)</span><span class="sxs-lookup"><span data-stu-id="0cd9a-120">Added [Get reply to a message API](../api/channel-get-messagereply.md)</span></span> | [<span data-ttu-id="0cd9a-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="0cd9a-121">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="0cd9a-122">チャネル内のメッセージへの返信を 1 件取得します。</span><span class="sxs-lookup"><span data-stu-id="0cd9a-122">Get a single reply to a message in a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="0cd9a-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0cd9a-123">Properties</span></span>
| <span data-ttu-id="0cd9a-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0cd9a-124">Property</span></span>     | <span data-ttu-id="0cd9a-125">型</span><span class="sxs-lookup"><span data-stu-id="0cd9a-125">Type</span></span>   |<span data-ttu-id="0cd9a-126">説明</span><span class="sxs-lookup"><span data-stu-id="0cd9a-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0cd9a-127">id</span><span class="sxs-lookup"><span data-stu-id="0cd9a-127">id</span></span>|<span data-ttu-id="0cd9a-128">String</span><span class="sxs-lookup"><span data-stu-id="0cd9a-128">String</span></span>| <span data-ttu-id="0cd9a-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0cd9a-129">Read-only.</span></span> <span data-ttu-id="0cd9a-130">メッセージの一意の ID。</span><span class="sxs-lookup"><span data-stu-id="0cd9a-130">Unique ID of the message.</span></span>|
|<span data-ttu-id="0cd9a-131">replyToId</span><span class="sxs-lookup"><span data-stu-id="0cd9a-131">replyToId</span></span>| <span data-ttu-id="0cd9a-132">string</span><span class="sxs-lookup"><span data-stu-id="0cd9a-132">string</span></span> | <span data-ttu-id="0cd9a-133">スレッドの親メッセージ/ルート メッセージの ID</span><span class="sxs-lookup"><span data-stu-id="0cd9a-133">Id of the parent message/root message of the thread</span></span> |
|<span data-ttu-id="0cd9a-134">from</span><span class="sxs-lookup"><span data-stu-id="0cd9a-134">from</span></span>|[<span data-ttu-id="0cd9a-135">identitySet</span><span class="sxs-lookup"><span data-stu-id="0cd9a-135">identitySet</span></span>](identityset.md)| <span data-ttu-id="0cd9a-136">メッセージの送信者の詳細</span><span class="sxs-lookup"><span data-stu-id="0cd9a-136">Details of the sender of the message</span></span>|
|<span data-ttu-id="0cd9a-137">etag</span><span class="sxs-lookup"><span data-stu-id="0cd9a-137">etag</span></span>| <span data-ttu-id="0cd9a-138">string</span><span class="sxs-lookup"><span data-stu-id="0cd9a-138">string</span></span> | <span data-ttu-id="0cd9a-139">メッセージのバージョン番号</span><span class="sxs-lookup"><span data-stu-id="0cd9a-139">Version number of the presentation.</span></span> |
|<span data-ttu-id="0cd9a-140">messageType</span><span class="sxs-lookup"><span data-stu-id="0cd9a-140">messageType</span></span>|<span data-ttu-id="0cd9a-141">String</span><span class="sxs-lookup"><span data-stu-id="0cd9a-141">String</span></span>|<span data-ttu-id="0cd9a-142">メッセージの種類。現在サポートされている値: message、chatEvent、Typing</span><span class="sxs-lookup"><span data-stu-id="0cd9a-142">The type of message, current supported values are: message, chatEvent, Typing</span></span>|
|<span data-ttu-id="0cd9a-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0cd9a-143">createdDateTime</span></span>|<span data-ttu-id="0cd9a-144">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cd9a-144">dateTimeOffset</span></span>|<span data-ttu-id="0cd9a-145">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0cd9a-145">Read only.</span></span> <span data-ttu-id="0cd9a-146">メッセージ作成時のタイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="0cd9a-146">Timestamp of when the group was created.</span></span>|
|<span data-ttu-id="0cd9a-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0cd9a-147">lastModifiedDateTime</span></span>|<span data-ttu-id="0cd9a-148">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cd9a-148">dateTimeOffset</span></span>|<span data-ttu-id="0cd9a-149">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0cd9a-149">Read only.</span></span> <span data-ttu-id="0cd9a-150">メッセージ編集/更新時のタイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="0cd9a-150">Timestamp of when the message was edited/updated</span></span>|
|<span data-ttu-id="0cd9a-151">deleted</span><span class="sxs-lookup"><span data-stu-id="0cd9a-151">deleted</span></span>|<span data-ttu-id="0cd9a-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cd9a-152">Boolean</span></span>|<span data-ttu-id="0cd9a-153">メッセージが削除済み (回復可能) かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0cd9a-153">Indicates whether a message has been soft deleted</span></span>|
|<span data-ttu-id="0cd9a-154">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="0cd9a-154">deletedDateTime</span></span>|<span data-ttu-id="0cd9a-155">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cd9a-155">dateTimeOffset</span></span>|<span data-ttu-id="0cd9a-156">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0cd9a-156">Read only.</span></span> <span data-ttu-id="0cd9a-157">メッセージ削除時のタイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="0cd9a-157">Timestamp at which the message was deleted</span></span> |
|<span data-ttu-id="0cd9a-158">subject</span><span class="sxs-lookup"><span data-stu-id="0cd9a-158">subject</span></span>|<span data-ttu-id="0cd9a-159">string</span><span class="sxs-lookup"><span data-stu-id="0cd9a-159">string</span></span>|<span data-ttu-id="0cd9a-160">メッセージの件名。</span><span class="sxs-lookup"><span data-stu-id="0cd9a-160">Message subject line.</span></span> <span data-ttu-id="0cd9a-161">省略可能</span><span class="sxs-lookup"><span data-stu-id="0cd9a-161">Optional</span></span>|
|<span data-ttu-id="0cd9a-162">body</span><span class="sxs-lookup"><span data-stu-id="0cd9a-162">body</span></span>|[<span data-ttu-id="0cd9a-163">itemBody</span><span class="sxs-lookup"><span data-stu-id="0cd9a-163">itemBody</span></span>](itembody.md)|<span data-ttu-id="0cd9a-164">メッセージのコンテンツのプレーンテキスト/HTML 表記。</span><span class="sxs-lookup"><span data-stu-id="0cd9a-164">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="0cd9a-165">既定ではプレーンテキストを返しますが、クエリ パラメーターの一部としてアプリケーションで HTML を選択できます</span><span class="sxs-lookup"><span data-stu-id="0cd9a-165">Returns plain text by default, application can choose HTML as part of a query param</span></span>|
|<span data-ttu-id="0cd9a-166">summary</span><span class="sxs-lookup"><span data-stu-id="0cd9a-166">Summary</span></span>|<span data-ttu-id="0cd9a-167">string</span><span class="sxs-lookup"><span data-stu-id="0cd9a-167">string</span></span>|<span data-ttu-id="0cd9a-168">プッシュ通知および概要ビューまたはフォールバック ビューに使用できるメッセージの概要テキスト</span><span class="sxs-lookup"><span data-stu-id="0cd9a-168">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="0cd9a-169">mentions</span><span class="sxs-lookup"><span data-stu-id="0cd9a-169">mentions</span></span>|<span data-ttu-id="0cd9a-170">[chatMessageMention](chatmention.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0cd9a-170">[chatMessageMention](chatmention.md) collection</span></span>| <span data-ttu-id="0cd9a-171">メッセージに記載されているエンティティの一覧。</span><span class="sxs-lookup"><span data-stu-id="0cd9a-171">List of entities mentioned in the message.</span></span> <span data-ttu-id="0cd9a-172">現在、user、bot、team、channel がサポートされています</span><span class="sxs-lookup"><span data-stu-id="0cd9a-172">Currently supports user, bot, team, channel</span></span>|
|<span data-ttu-id="0cd9a-173">importance</span><span class="sxs-lookup"><span data-stu-id="0cd9a-173">importance</span></span>| <span data-ttu-id="0cd9a-174">string</span><span class="sxs-lookup"><span data-stu-id="0cd9a-174">string</span></span> | <span data-ttu-id="0cd9a-175">メッセージの重要度: 通常、高</span><span class="sxs-lookup"><span data-stu-id="0cd9a-175">The importance of the message: Low = 0, Normal = 1, High = 2.</span></span>|
|<span data-ttu-id="0cd9a-176">reactions</span><span class="sxs-lookup"><span data-stu-id="0cd9a-176">reactions</span></span>| <span data-ttu-id="0cd9a-177">[chatMessageReaction](chatreaction.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0cd9a-177">[chatMessageReaction](chatreaction.md) collection</span></span> | <span data-ttu-id="0cd9a-178">このメッセージに対する反応 (例: いいね!)</span><span class="sxs-lookup"><span data-stu-id="0cd9a-178">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="0cd9a-179">locale</span><span class="sxs-lookup"><span data-stu-id="0cd9a-179">locale</span></span>|<span data-ttu-id="0cd9a-180">string</span><span class="sxs-lookup"><span data-stu-id="0cd9a-180">string</span></span>|<span data-ttu-id="0cd9a-181">クライアントに設定されたメッセージのロケール</span><span class="sxs-lookup"><span data-stu-id="0cd9a-181">Locale of the message set by the client</span></span>|
|<span data-ttu-id="0cd9a-182">attachments</span><span class="sxs-lookup"><span data-stu-id="0cd9a-182">attachments</span></span>|<span data-ttu-id="0cd9a-183">[chatMessageAttachment](chatattachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0cd9a-183">[chatMessageAttachment](chatattachment.md) collection</span></span> |<span data-ttu-id="0cd9a-184">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="0cd9a-184">Attached files and messages</span></span>|


## <a name="json-representation"></a><span data-ttu-id="0cd9a-185">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0cd9a-185">JSON representation</span></span>

<span data-ttu-id="0cd9a-186">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0cd9a-186">The following is a JSON representation of the resource.</span></span>

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
