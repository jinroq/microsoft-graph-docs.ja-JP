---
title: post リソース タイプ
description: ConverstaionThread エンティティ内の個々 の投稿アイテムを表します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 46e33021d0929e1bd665f8256f0874e8e8c92809
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942417"
---
# <a name="post-resource-type"></a><span data-ttu-id="6d1be-103">post リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="6d1be-103">post resource type</span></span>

> <span data-ttu-id="6d1be-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6d1be-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6d1be-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6d1be-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6d1be-106">[ConverstaionThread](conversationthread.md)エンティティ内の個々 の投稿アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="6d1be-106">Represents an individual post item within a [converstaionThread](conversationthread.md) entity.</span></span>

<span data-ttu-id="6d1be-107">投稿を明示的に作成できなくても、次のいずれかの方法で投稿を作成できます。</span><span class="sxs-lookup"><span data-stu-id="6d1be-107">Even though you cannot explicitly create a post, doing any of the following would create a post:</span></span>

* [<span data-ttu-id="6d1be-108">既存の投稿に返信する</span><span class="sxs-lookup"><span data-stu-id="6d1be-108">Reply to an existing post</span></span>](../api/post-reply.md) 
* [<span data-ttu-id="6d1be-109">既存のスレッドに返信する</span><span class="sxs-lookup"><span data-stu-id="6d1be-109">Reply to an existing thread</span></span>](../api/conversationthread-reply.md) 
* [<span data-ttu-id="6d1be-110">新しい会話にスレッドを作成する</span><span class="sxs-lookup"><span data-stu-id="6d1be-110">Create a thread in a new conversation</span></span>](../api/group-post-threads.md)
* [<span data-ttu-id="6d1be-111">新しい会話を作成する</span><span class="sxs-lookup"><span data-stu-id="6d1be-111">Create a new conversation</span></span>](../api/group-post-conversations.md)

<span data-ttu-id="6d1be-112">このリソースでは、[拡張機能](/graph/extensibility-overview)を使用してカスタム プロパティに独自のデータを追加することができます。</span><span class="sxs-lookup"><span data-stu-id="6d1be-112">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d1be-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6d1be-113">JSON representation</span></span>

<span data-ttu-id="6d1be-114">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="6d1be-114">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "extensions",
    "inReplyTo",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "@odata.type": "microsoft.graph.post"
}-->

```json
{
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "categories": ["string"],
  "changeKey": "string",
  "conversationId": "string",
  "conversationThreadId": "string",
  "createdDateTime": "String (timestamp)",
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "string",
  "lastModifiedDateTime": "String (timestamp)",
  "newParticipants": [{"@odata.type": "microsoft.graph.recipient"}],
  "receivedDateTime": "String (timestamp)",
  "sender": {"@odata.type": "microsoft.graph.recipient"}
}

```
## <a name="properties"></a><span data-ttu-id="6d1be-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6d1be-115">Properties</span></span>
| <span data-ttu-id="6d1be-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6d1be-116">Property</span></span>     | <span data-ttu-id="6d1be-117">型</span><span class="sxs-lookup"><span data-stu-id="6d1be-117">Type</span></span>   |<span data-ttu-id="6d1be-118">説明</span><span class="sxs-lookup"><span data-stu-id="6d1be-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d1be-119">body</span><span class="sxs-lookup"><span data-stu-id="6d1be-119">body</span></span>|[<span data-ttu-id="6d1be-120">itemBody</span><span class="sxs-lookup"><span data-stu-id="6d1be-120">itemBody</span></span>](itembody.md)|<span data-ttu-id="6d1be-p102">投稿の内容です。これが既定のプロパティです。このプロパティを null にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6d1be-p102">The contents of the post. This is a default property. This property can be null.</span></span>|
|<span data-ttu-id="6d1be-124">categories</span><span class="sxs-lookup"><span data-stu-id="6d1be-124">categories</span></span>|<span data-ttu-id="6d1be-125">String コレクション</span><span class="sxs-lookup"><span data-stu-id="6d1be-125">String collection</span></span>|<span data-ttu-id="6d1be-126">投稿に関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="6d1be-126">The categories associated with the post.</span></span> <span data-ttu-id="6d1be-127">各カテゴリは、ユーザーが定義されている[outlookCategory](outlookcategory.md)の**表示名**のプロパティに対応します。</span><span class="sxs-lookup"><span data-stu-id="6d1be-127">Each category corresponds to the **displayName** property of an [outlookCategory](outlookcategory.md) that has been defined for a user.</span></span>|
|<span data-ttu-id="6d1be-128">changeKey</span><span class="sxs-lookup"><span data-stu-id="6d1be-128">changeKey</span></span>|<span data-ttu-id="6d1be-129">String</span><span class="sxs-lookup"><span data-stu-id="6d1be-129">String</span></span>|<span data-ttu-id="6d1be-p104">投稿のバージョンを識別します。投稿を変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。</span><span class="sxs-lookup"><span data-stu-id="6d1be-p104">Identifies the version of the post. Every time the post is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="6d1be-133">conversationId</span><span class="sxs-lookup"><span data-stu-id="6d1be-133">conversationId</span></span>|<span data-ttu-id="6d1be-134">String</span><span class="sxs-lookup"><span data-stu-id="6d1be-134">String</span></span>|<span data-ttu-id="6d1be-p105">会話の固有 ID です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="6d1be-p105">Unique ID of the conversation. Read-only.</span></span>|
|<span data-ttu-id="6d1be-137">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="6d1be-137">conversationThreadId</span></span>|<span data-ttu-id="6d1be-138">String</span><span class="sxs-lookup"><span data-stu-id="6d1be-138">String</span></span>|<span data-ttu-id="6d1be-p106">会話スレッドの固有 ID です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="6d1be-p106">Unique ID of the conversation thread. Read-only.</span></span>|
|<span data-ttu-id="6d1be-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6d1be-141">createdDateTime</span></span>|<span data-ttu-id="6d1be-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d1be-142">DateTimeOffset</span></span>|<span data-ttu-id="6d1be-p107">投稿の作成時刻を示します。DateTimeOffset 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6d1be-p107">Specifies when the post was created. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6d1be-146">from</span><span class="sxs-lookup"><span data-stu-id="6d1be-146">from</span></span>|[<span data-ttu-id="6d1be-147">recipient</span><span class="sxs-lookup"><span data-stu-id="6d1be-147">recipient</span></span>](recipient.md)|<span data-ttu-id="6d1be-p108">代理人アクセスのシナリオで使用されます。他のユーザーの代わりにメッセージを投稿したユーザーを示します。これが既定のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="6d1be-p108">Used in delegate access scenarios. Indicates who posted the message on behalf of another user. This is a default property.</span></span>|
|<span data-ttu-id="6d1be-151">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="6d1be-151">hasAttachments</span></span>|<span data-ttu-id="6d1be-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d1be-152">Boolean</span></span>|<span data-ttu-id="6d1be-p109">投稿の添付ファイルが 1 つ以上あるかどうかを示します。これが既定のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="6d1be-p109">Indicates whether the post has at least one attachment. This is a default property.</span></span>|
|<span data-ttu-id="6d1be-155">id</span><span class="sxs-lookup"><span data-stu-id="6d1be-155">id</span></span>|<span data-ttu-id="6d1be-156">String</span><span class="sxs-lookup"><span data-stu-id="6d1be-156">String</span></span>| <span data-ttu-id="6d1be-157">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="6d1be-157">Read-only.</span></span>|
|<span data-ttu-id="6d1be-158">importance</span><span class="sxs-lookup"><span data-stu-id="6d1be-158">importance</span></span> | <span data-ttu-id="6d1be-159">String</span><span class="sxs-lookup"><span data-stu-id="6d1be-159">String</span></span> | <span data-ttu-id="6d1be-160">グループのポストの重要性: `low`、 `normal`、 `high`。</span><span class="sxs-lookup"><span data-stu-id="6d1be-160">The importance of a group post: `low`, `normal`, `high`.</span></span> |
|<span data-ttu-id="6d1be-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d1be-161">lastModifiedDateTime</span></span>|<span data-ttu-id="6d1be-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d1be-162">DateTimeOffset</span></span>|<span data-ttu-id="6d1be-p110">投稿が最後に修正された日時を指定します。DateTimeOffset 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6d1be-p110">Specifies when the post was last modified. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6d1be-166">newParticipants</span><span class="sxs-lookup"><span data-stu-id="6d1be-166">newParticipants</span></span>|<span data-ttu-id="6d1be-167">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="6d1be-167">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="6d1be-168">この投稿の一部としてスレッドに追加された会話の参加者です。</span><span class="sxs-lookup"><span data-stu-id="6d1be-168">Conversation participants that were added to the thread as part of this post.</span></span>|
|<span data-ttu-id="6d1be-169">receivedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d1be-169">receivedDateTime</span></span>|<span data-ttu-id="6d1be-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d1be-170">DateTimeOffset</span></span>|<span data-ttu-id="6d1be-p111">投稿の受信時刻を示します。DateTimeOffset 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6d1be-p111">Specifies when the post was received. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6d1be-174">sender</span><span class="sxs-lookup"><span data-stu-id="6d1be-174">sender</span></span>|[<span data-ttu-id="6d1be-175">recipient</span><span class="sxs-lookup"><span data-stu-id="6d1be-175">recipient</span></span>](recipient.md)|<span data-ttu-id="6d1be-p112">送信者のアドレスが含まれます。送信者が指定されていない場合、送信者の値は認証済みユーザーのアドレスと見なされます。これが既定のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="6d1be-p112">Contains the address of the sender. The value of Sender is assumed to be the address of the authenticated user in the case when Sender is not specified. This is a default property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d1be-179">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6d1be-179">Relationships</span></span>
| <span data-ttu-id="6d1be-180">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6d1be-180">Relationship</span></span> | <span data-ttu-id="6d1be-181">型</span><span class="sxs-lookup"><span data-stu-id="6d1be-181">Type</span></span>   |<span data-ttu-id="6d1be-182">説明</span><span class="sxs-lookup"><span data-stu-id="6d1be-182">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d1be-183">attachments</span><span class="sxs-lookup"><span data-stu-id="6d1be-183">attachments</span></span>|<span data-ttu-id="6d1be-184">[Attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6d1be-184">[Attachment](attachment.md) collection</span></span>|<span data-ttu-id="6d1be-185">投稿の[fileAttachment](fileattachment.md)、 [itemAttachment](itemattachment.md)、および[referenceAttachment](referenceattachment.md)の添付ファイルのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="6d1be-185">The collection of [fileAttachment](fileattachment.md), [itemAttachment](itemattachment.md), and [referenceAttachment](referenceattachment.md) attachments for the post.</span></span> <span data-ttu-id="6d1be-186">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6d1be-186">Read-only.</span></span> <span data-ttu-id="6d1be-187">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="6d1be-187">Nullable.</span></span>|
|<span data-ttu-id="6d1be-188">extensions</span><span class="sxs-lookup"><span data-stu-id="6d1be-188">extensions</span></span>|<span data-ttu-id="6d1be-189">[Extension](extension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6d1be-189">[Extension](extension.md) collection</span></span>|<span data-ttu-id="6d1be-p114">投稿に対して定義されているオープン拡張機能のコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="6d1be-p114">The collection of open extensions defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="6d1be-193">inReplyTo</span><span class="sxs-lookup"><span data-stu-id="6d1be-193">inReplyTo</span></span>|[<span data-ttu-id="6d1be-194">Post</span><span class="sxs-lookup"><span data-stu-id="6d1be-194">Post</span></span>](post.md)|<span data-ttu-id="6d1be-195">[ConversationThread](conversationthread.md)でへこの投稿の返信は、以前の投稿です。</span><span class="sxs-lookup"><span data-stu-id="6d1be-195">The earlier post that this post is replying to in the [conversationThread](conversationthread.md).</span></span> <span data-ttu-id="6d1be-196">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="6d1be-196">Read-only.</span></span>|
|<span data-ttu-id="6d1be-197">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="6d1be-197">multiValueExtendedProperties</span></span>|<span data-ttu-id="6d1be-198">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6d1be-198">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="6d1be-p116">その投稿用に定義された、複数値拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="6d1be-p116">The collection of multi-value extended properties defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="6d1be-202">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="6d1be-202">singleValueExtendedProperties</span></span>|<span data-ttu-id="6d1be-203">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6d1be-203">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="6d1be-p117">その投稿用に定義された、単一値拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="6d1be-p117">The collection of single-value extended properties defined for the post. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="6d1be-207">メソッド</span><span class="sxs-lookup"><span data-stu-id="6d1be-207">Methods</span></span>

| <span data-ttu-id="6d1be-208">メソッド</span><span class="sxs-lookup"><span data-stu-id="6d1be-208">Method</span></span>           | <span data-ttu-id="6d1be-209">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6d1be-209">Return Type</span></span>    |<span data-ttu-id="6d1be-210">説明</span><span class="sxs-lookup"><span data-stu-id="6d1be-210">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6d1be-211">List posts</span><span class="sxs-lookup"><span data-stu-id="6d1be-211">List posts</span></span>](../api/conversationthread-list-posts.md) | [<span data-ttu-id="6d1be-212">post</span><span class="sxs-lookup"><span data-stu-id="6d1be-212">post</span></span>](post.md) |<span data-ttu-id="6d1be-213">指定したスレッドの投稿を取得します。</span><span class="sxs-lookup"><span data-stu-id="6d1be-213">Get the posts of the specified thread.</span></span> |
|[<span data-ttu-id="6d1be-214">Get post</span><span class="sxs-lookup"><span data-stu-id="6d1be-214">Get post</span></span>](../api/post-get.md) | [<span data-ttu-id="6d1be-215">post</span><span class="sxs-lookup"><span data-stu-id="6d1be-215">post</span></span>](post.md) |<span data-ttu-id="6d1be-216">指定したスレッド内の投稿のプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="6d1be-216">Get the properties and relationships of a post in a specified thread.</span></span>|
|[<span data-ttu-id="6d1be-217">Reply</span><span class="sxs-lookup"><span data-stu-id="6d1be-217">Reply</span></span>](../api/post-reply.md)|<span data-ttu-id="6d1be-218">なし</span><span class="sxs-lookup"><span data-stu-id="6d1be-218">None</span></span>|<span data-ttu-id="6d1be-219">グループ会話の投稿に返信して、指定されたスレッドに新しい投稿を追加します。</span><span class="sxs-lookup"><span data-stu-id="6d1be-219">Reply to a post and add a new post to the specified thread in a group conversation.</span></span>|
|[<span data-ttu-id="6d1be-220">Forward</span><span class="sxs-lookup"><span data-stu-id="6d1be-220">Forward</span></span>](../api/post-forward.md)|<span data-ttu-id="6d1be-221">なし</span><span class="sxs-lookup"><span data-stu-id="6d1be-221">None</span></span>|<span data-ttu-id="6d1be-222">受信者に投稿を転送します。</span><span class="sxs-lookup"><span data-stu-id="6d1be-222">Forward a post to a recipient.</span></span>|
|<span data-ttu-id="6d1be-223">**添付ファイル**</span><span class="sxs-lookup"><span data-stu-id="6d1be-223">**Attachments**</span></span>| | |
|[<span data-ttu-id="6d1be-224">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="6d1be-224">List attachments</span></span>](../api/post-list-attachments.md) |<span data-ttu-id="6d1be-225">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6d1be-225">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="6d1be-226">投稿のすべての添付ファイルを取得します。</span><span class="sxs-lookup"><span data-stu-id="6d1be-226">Get all attachments on a post.</span></span>|
|[<span data-ttu-id="6d1be-227">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="6d1be-227">Add attachment</span></span>](../api/post-post-attachments.md) |[<span data-ttu-id="6d1be-228">attachment</span><span class="sxs-lookup"><span data-stu-id="6d1be-228">attachment</span></span>](attachment.md)| <span data-ttu-id="6d1be-229">投稿に添付ファイルを追加します。</span><span class="sxs-lookup"><span data-stu-id="6d1be-229">Add an attachment to a post.</span></span> |
|<span data-ttu-id="6d1be-230">**オープン拡張機能**</span><span class="sxs-lookup"><span data-stu-id="6d1be-230">**Open extensions**</span></span>| | |
|[<span data-ttu-id="6d1be-231">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="6d1be-231">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="6d1be-232">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="6d1be-232">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="6d1be-233">オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="6d1be-233">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="6d1be-234">オープン拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="6d1be-234">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="6d1be-235">[openTypeExtension](opentypeextension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6d1be-235">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="6d1be-236">拡張機能の名前で識別されるオープン拡張機能を取得します。</span><span class="sxs-lookup"><span data-stu-id="6d1be-236">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="6d1be-237">**スキーマ拡張機能**</span><span class="sxs-lookup"><span data-stu-id="6d1be-237">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="6d1be-238">スキーマ拡張機能の値を追加する</span><span class="sxs-lookup"><span data-stu-id="6d1be-238">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="6d1be-239">スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。</span><span class="sxs-lookup"><span data-stu-id="6d1be-239">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="6d1be-240">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="6d1be-240">**Extended properties**</span></span>| | |
|[<span data-ttu-id="6d1be-241">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="6d1be-241">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="6d1be-242">post</span><span class="sxs-lookup"><span data-stu-id="6d1be-242">post</span></span>](post.md)  |<span data-ttu-id="6d1be-243">新規または既存の投稿に、ひとつまたは複数の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="6d1be-243">Create one or more single-value extended properties in a new or existing post.</span></span>   |
|[<span data-ttu-id="6d1be-244">Get post with single-value extended property</span><span class="sxs-lookup"><span data-stu-id="6d1be-244">Get post with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="6d1be-245">post</span><span class="sxs-lookup"><span data-stu-id="6d1be-245">post</span></span>](post.md) | <span data-ttu-id="6d1be-246">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含む投稿を取得します。</span><span class="sxs-lookup"><span data-stu-id="6d1be-246">Get posts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="6d1be-247">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="6d1be-247">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="6d1be-248">post</span><span class="sxs-lookup"><span data-stu-id="6d1be-248">post</span></span>](post.md) | <span data-ttu-id="6d1be-249">新規または既存の投稿に、ひとつまたは複数の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="6d1be-249">Create one or more multi-value extended properties in a new or existing post.</span></span>  |
|[<span data-ttu-id="6d1be-250">Get post with multi-value extended property</span><span class="sxs-lookup"><span data-stu-id="6d1be-250">Get post with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="6d1be-251">post</span><span class="sxs-lookup"><span data-stu-id="6d1be-251">post</span></span>](post.md) | <span data-ttu-id="6d1be-252">`$expand` を使用して、複数値の拡張プロパティを含む投稿を取得します。</span><span class="sxs-lookup"><span data-stu-id="6d1be-252">Get a post that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="see-also"></a><span data-ttu-id="6d1be-253">関連項目</span><span class="sxs-lookup"><span data-stu-id="6d1be-253">See also</span></span>

- [<span data-ttu-id="6d1be-254">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="6d1be-254">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="6d1be-255">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="6d1be-255">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="6d1be-256">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="6d1be-256">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
