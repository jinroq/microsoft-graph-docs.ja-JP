---
title: chatMessage リソースの種類
description: チャネルまたはチャットのエンティティ内で個別のチャット メッセージを表します。 メッセージは、ルートのメッセージまたはメッセージ内の**replyToId**プロパティで定義されているスレッドの一部にできます。
localization_priority: Priority
ms.openlocfilehash: ad381102f7e93a4dcccd7b68435d0687ed6b4837
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855994"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="89307-104">chatMessage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="89307-104">chatMessage resource type</span></span>

> <span data-ttu-id="89307-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="89307-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89307-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89307-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="89307-107">[チャネル](channel.md)またはチャットのエンティティ内で個別のチャット メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="89307-107">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="89307-108">メッセージは、ルートのメッセージまたはメッセージ内の**replyToId**プロパティで定義されているスレッドの一部にできます。</span><span class="sxs-lookup"><span data-stu-id="89307-108">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="89307-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="89307-109">Methods</span></span>

| <span data-ttu-id="89307-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="89307-110">Method</span></span>       | <span data-ttu-id="89307-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="89307-111">Return Type</span></span>  |<span data-ttu-id="89307-112">説明</span><span class="sxs-lookup"><span data-stu-id="89307-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="89307-113">リストのチャネルのメッセージ</span><span class="sxs-lookup"><span data-stu-id="89307-113">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="89307-114">[chatmessage](chatmessage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="89307-114">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="89307-115">チャネルでは、ルートのすべてのメッセージの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="89307-115">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="89307-116">チャネル取得メッセージ</span><span class="sxs-lookup"><span data-stu-id="89307-116">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="89307-117">chatmessage</span><span class="sxs-lookup"><span data-stu-id="89307-117">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="89307-118">チャンネルから 1 つのルートのメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="89307-118">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="89307-119">メッセージに対する返信の一覧</span><span class="sxs-lookup"><span data-stu-id="89307-119">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="89307-120">[chatmessage](chatmessage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="89307-120">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="89307-121">チャネルでのメッセージに対する返信をすべての一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="89307-121">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="89307-122">メッセージへの応答を取得します。</span><span class="sxs-lookup"><span data-stu-id="89307-122">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="89307-123">chatmessage</span><span class="sxs-lookup"><span data-stu-id="89307-123">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="89307-124">チャネル内のメッセージに 1 つの返信を取得します。</span><span class="sxs-lookup"><span data-stu-id="89307-124">Get a single reply to a message in a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="89307-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="89307-125">Properties</span></span>
| <span data-ttu-id="89307-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="89307-126">Property</span></span>     | <span data-ttu-id="89307-127">種類</span><span class="sxs-lookup"><span data-stu-id="89307-127">Type</span></span>   |<span data-ttu-id="89307-128">説明</span><span class="sxs-lookup"><span data-stu-id="89307-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89307-129">ID</span><span class="sxs-lookup"><span data-stu-id="89307-129">id</span></span>|<span data-ttu-id="89307-130">String</span><span class="sxs-lookup"><span data-stu-id="89307-130">String</span></span>| <span data-ttu-id="89307-131">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="89307-131">Read-only.</span></span> <span data-ttu-id="89307-132">メッセージの一意の ID です。</span><span class="sxs-lookup"><span data-stu-id="89307-132">Unique ID of the message.</span></span>|
|<span data-ttu-id="89307-133">replyToId</span><span class="sxs-lookup"><span data-stu-id="89307-133">replyToId</span></span>| <span data-ttu-id="89307-134">文字列</span><span class="sxs-lookup"><span data-stu-id="89307-134">string</span></span> | <span data-ttu-id="89307-135">スレッドの親メッセージとルートのメッセージの id</span><span class="sxs-lookup"><span data-stu-id="89307-135">Id of the parent message/root message of the thread</span></span> |
|<span data-ttu-id="89307-136">from</span><span class="sxs-lookup"><span data-stu-id="89307-136">from</span></span>|[<span data-ttu-id="89307-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="89307-137">identitySet</span></span>](identityset.md)| <span data-ttu-id="89307-138">メッセージの送信者の詳細</span><span class="sxs-lookup"><span data-stu-id="89307-138">Details of the sender of the message</span></span>|
|<span data-ttu-id="89307-139">etag</span><span class="sxs-lookup"><span data-stu-id="89307-139">etag</span></span>| <span data-ttu-id="89307-140">文字列</span><span class="sxs-lookup"><span data-stu-id="89307-140">string</span></span> | <span data-ttu-id="89307-141">メッセージのバージョン番号</span><span class="sxs-lookup"><span data-stu-id="89307-141">Version number of the message</span></span> |
|<span data-ttu-id="89307-142">messageType</span><span class="sxs-lookup"><span data-stu-id="89307-142">messageType</span></span>|<span data-ttu-id="89307-143">String</span><span class="sxs-lookup"><span data-stu-id="89307-143">String</span></span>|<span data-ttu-id="89307-144">サポートされているメッセージでは、現在の type の値: メッセージ、chatEvent を入力します。</span><span class="sxs-lookup"><span data-stu-id="89307-144">The type of message, current supported values are: message, chatEvent, Typing</span></span>|
|<span data-ttu-id="89307-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="89307-145">createdDateTime</span></span>|<span data-ttu-id="89307-146">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89307-146">dateTimeOffset</span></span>|<span data-ttu-id="89307-147">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="89307-147">Read only.</span></span> <span data-ttu-id="89307-148">メッセージが作成された日時のタイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="89307-148">Timestamp of when the message was created</span></span>|
|<span data-ttu-id="89307-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="89307-149">lastModifiedDateTime</span></span>|<span data-ttu-id="89307-150">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89307-150">dateTimeOffset</span></span>|<span data-ttu-id="89307-151">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="89307-151">Read only.</span></span> <span data-ttu-id="89307-152">メッセージが編集更新をされたときのタイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="89307-152">Timestamp of when the message was edited/updated</span></span>|
|<span data-ttu-id="89307-153">isDeleted</span><span class="sxs-lookup"><span data-stu-id="89307-153">isDeleted</span></span>|<span data-ttu-id="89307-154">ブール</span><span class="sxs-lookup"><span data-stu-id="89307-154">boolean</span></span>|<span data-ttu-id="89307-155">メッセージをソフト削除されている場合を表します。</span><span class="sxs-lookup"><span data-stu-id="89307-155">Represents if a message has been soft deleted</span></span>|
|<span data-ttu-id="89307-156">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="89307-156">deletedDateTime</span></span>|<span data-ttu-id="89307-157">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89307-157">dateTimeOffset</span></span>|<span data-ttu-id="89307-158">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="89307-158">Read only.</span></span> <span data-ttu-id="89307-159">タイムスタンプは、メッセージが削除されました</span><span class="sxs-lookup"><span data-stu-id="89307-159">Timestamp at which the message was deleted</span></span> |
|<span data-ttu-id="89307-160">subject</span><span class="sxs-lookup"><span data-stu-id="89307-160">subject</span></span>|<span data-ttu-id="89307-161">文字列</span><span class="sxs-lookup"><span data-stu-id="89307-161">string</span></span>|<span data-ttu-id="89307-162">メッセージの件名です。</span><span class="sxs-lookup"><span data-stu-id="89307-162">Message subject line.</span></span> <span data-ttu-id="89307-163">省略可能</span><span class="sxs-lookup"><span data-stu-id="89307-163">Optional</span></span>|
|<span data-ttu-id="89307-164">body</span><span class="sxs-lookup"><span data-stu-id="89307-164">body</span></span>|[<span data-ttu-id="89307-165">itemBody</span><span class="sxs-lookup"><span data-stu-id="89307-165">itemBody</span></span>](itembody.md)|<span data-ttu-id="89307-166">メッセージのコンテンツのプレーン テキストと HTML 形式です。</span><span class="sxs-lookup"><span data-stu-id="89307-166">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="89307-167">プレーン テキストを返します既定では、アプリケーションは、クエリ パラメーターの一部として HTML を選択できます。</span><span class="sxs-lookup"><span data-stu-id="89307-167">Returns plain text by default, application can choose HTML as part of a query param</span></span>|
|<span data-ttu-id="89307-168">概要</span><span class="sxs-lookup"><span data-stu-id="89307-168">summary</span></span>|<span data-ttu-id="89307-169">文字列</span><span class="sxs-lookup"><span data-stu-id="89307-169">string</span></span>|<span data-ttu-id="89307-170">プッシュ通知し、サマリー ・ ビューまたはフォール バック ・ ビューの使用できるメッセージの概要のテキスト</span><span class="sxs-lookup"><span data-stu-id="89307-170">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="89307-171">mentions</span><span class="sxs-lookup"><span data-stu-id="89307-171">mentions</span></span>|<span data-ttu-id="89307-172">[chatMessageMention](chatmention.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="89307-172">[chatMessageMention](chatmention.md) collection</span></span>| <span data-ttu-id="89307-173">メッセージに記載されているエンティティの一覧です。</span><span class="sxs-lookup"><span data-stu-id="89307-173">List of entities mentioned in the message.</span></span> <span data-ttu-id="89307-174">チャネル、ユーザー、ボット、チームが現在サポートしています</span><span class="sxs-lookup"><span data-stu-id="89307-174">Currently supports user, bot, team, channel</span></span>|
|<span data-ttu-id="89307-175">importance</span><span class="sxs-lookup"><span data-stu-id="89307-175">importance</span></span>| <span data-ttu-id="89307-176">文字列</span><span class="sxs-lookup"><span data-stu-id="89307-176">string</span></span> | <span data-ttu-id="89307-177">メッセージの重要度: 高、通常</span><span class="sxs-lookup"><span data-stu-id="89307-177">The importance of the message: Normal, High</span></span>|
|<span data-ttu-id="89307-178">反力</span><span class="sxs-lookup"><span data-stu-id="89307-178">reactions</span></span>| <span data-ttu-id="89307-179">[chatMessageReaction](chatreaction.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="89307-179">[chatMessageReaction](chatreaction.md) collection</span></span> | <span data-ttu-id="89307-180">このメッセージの反応 (たとえばなど)</span><span class="sxs-lookup"><span data-stu-id="89307-180">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="89307-181">locale</span><span class="sxs-lookup"><span data-stu-id="89307-181">locale</span></span>|<span data-ttu-id="89307-182">文字列</span><span class="sxs-lookup"><span data-stu-id="89307-182">string</span></span>|<span data-ttu-id="89307-183">クライアントが設定するメッセージのロケール</span><span class="sxs-lookup"><span data-stu-id="89307-183">Locale of the message set by the client</span></span>|
|<span data-ttu-id="89307-184">attachments</span><span class="sxs-lookup"><span data-stu-id="89307-184">attachments</span></span>|<span data-ttu-id="89307-185">[chatMessageAttachment](chatattachment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="89307-185">[chatMessageAttachment](chatattachment.md) collection</span></span> |<span data-ttu-id="89307-186">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="89307-186">Attached files</span></span>|


## <a name="json-representation"></a><span data-ttu-id="89307-187">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="89307-187">JSON representation</span></span>

<span data-ttu-id="89307-188">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="89307-188">The following is a JSON representation of the resource.</span></span>

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
