---
title: post リソース タイプ
description: ConverstaionThread エンティティ内の個々 の投稿アイテムを表します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 554892bdfed45d0fba9b90a084db67c0bb329486
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519956"
---
# <a name="post-resource-type"></a><span data-ttu-id="b8eb8-103">post リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="b8eb8-103">post resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8eb8-104">[ConverstaionThread](conversationthread.md)エンティティ内の個々 の投稿アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-104">Represents an individual post item within a [converstaionThread](conversationthread.md) entity.</span></span>

<span data-ttu-id="b8eb8-105">投稿を明示的に作成できなくても、次のいずれかの方法で投稿を作成できます。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-105">Even though you cannot explicitly create a post, doing any of the following would create a post:</span></span>

* [<span data-ttu-id="b8eb8-106">既存の投稿に返信する</span><span class="sxs-lookup"><span data-stu-id="b8eb8-106">Reply to an existing post</span></span>](../api/post-reply.md) 
* [<span data-ttu-id="b8eb8-107">既存のスレッドに返信する</span><span class="sxs-lookup"><span data-stu-id="b8eb8-107">Reply to an existing thread</span></span>](../api/conversationthread-reply.md) 
* [<span data-ttu-id="b8eb8-108">新しい会話にスレッドを作成する</span><span class="sxs-lookup"><span data-stu-id="b8eb8-108">Create a thread in a new conversation</span></span>](../api/group-post-threads.md)
* [<span data-ttu-id="b8eb8-109">新しい会話を作成する</span><span class="sxs-lookup"><span data-stu-id="b8eb8-109">Create a new conversation</span></span>](../api/group-post-conversations.md)

<span data-ttu-id="b8eb8-110">このリソースでは、[拡張機能](/graph/extensibility-overview)を使用してカスタム プロパティに独自のデータを追加することができます。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-110">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8eb8-111">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b8eb8-111">JSON representation</span></span>

<span data-ttu-id="b8eb8-112">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="b8eb8-112">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="b8eb8-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8eb8-113">Properties</span></span>
| <span data-ttu-id="b8eb8-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8eb8-114">Property</span></span>     | <span data-ttu-id="b8eb8-115">型</span><span class="sxs-lookup"><span data-stu-id="b8eb8-115">Type</span></span>   |<span data-ttu-id="b8eb8-116">説明</span><span class="sxs-lookup"><span data-stu-id="b8eb8-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8eb8-117">body</span><span class="sxs-lookup"><span data-stu-id="b8eb8-117">body</span></span>|[<span data-ttu-id="b8eb8-118">itemBody</span><span class="sxs-lookup"><span data-stu-id="b8eb8-118">itemBody</span></span>](itembody.md)|<span data-ttu-id="b8eb8-p101">投稿の内容です。これが既定のプロパティです。このプロパティを null にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-p101">The contents of the post. This is a default property. This property can be null.</span></span>|
|<span data-ttu-id="b8eb8-122">categories</span><span class="sxs-lookup"><span data-stu-id="b8eb8-122">categories</span></span>|<span data-ttu-id="b8eb8-123">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b8eb8-123">String collection</span></span>|<span data-ttu-id="b8eb8-124">投稿に関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-124">The categories associated with the post.</span></span> <span data-ttu-id="b8eb8-125">各カテゴリは、ユーザーが定義されている[outlookCategory](outlookcategory.md)の**表示名**のプロパティに対応します。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-125">Each category corresponds to the **displayName** property of an [outlookCategory](outlookcategory.md) that has been defined for a user.</span></span>|
|<span data-ttu-id="b8eb8-126">changeKey</span><span class="sxs-lookup"><span data-stu-id="b8eb8-126">changeKey</span></span>|<span data-ttu-id="b8eb8-127">String</span><span class="sxs-lookup"><span data-stu-id="b8eb8-127">String</span></span>|<span data-ttu-id="b8eb8-p103">投稿のバージョンを識別します。投稿を変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-p103">Identifies the version of the post. Every time the post is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="b8eb8-131">conversationId</span><span class="sxs-lookup"><span data-stu-id="b8eb8-131">conversationId</span></span>|<span data-ttu-id="b8eb8-132">String</span><span class="sxs-lookup"><span data-stu-id="b8eb8-132">String</span></span>|<span data-ttu-id="b8eb8-p104">会話の固有 ID です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-p104">Unique ID of the conversation. Read-only.</span></span>|
|<span data-ttu-id="b8eb8-135">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="b8eb8-135">conversationThreadId</span></span>|<span data-ttu-id="b8eb8-136">String</span><span class="sxs-lookup"><span data-stu-id="b8eb8-136">String</span></span>|<span data-ttu-id="b8eb8-p105">会話スレッドの固有 ID です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-p105">Unique ID of the conversation thread. Read-only.</span></span>|
|<span data-ttu-id="b8eb8-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b8eb8-139">createdDateTime</span></span>|<span data-ttu-id="b8eb8-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8eb8-140">DateTimeOffset</span></span>|<span data-ttu-id="b8eb8-p106">投稿の作成時刻を示します。DateTimeOffset 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b8eb8-p106">Specifies when the post was created. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b8eb8-144">from</span><span class="sxs-lookup"><span data-stu-id="b8eb8-144">from</span></span>|[<span data-ttu-id="b8eb8-145">recipient</span><span class="sxs-lookup"><span data-stu-id="b8eb8-145">recipient</span></span>](recipient.md)|<span data-ttu-id="b8eb8-p107">代理人アクセスのシナリオで使用されます。他のユーザーの代わりにメッセージを投稿したユーザーを示します。これが既定のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-p107">Used in delegate access scenarios. Indicates who posted the message on behalf of another user. This is a default property.</span></span>|
|<span data-ttu-id="b8eb8-149">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="b8eb8-149">hasAttachments</span></span>|<span data-ttu-id="b8eb8-150">ブール値</span><span class="sxs-lookup"><span data-stu-id="b8eb8-150">Boolean</span></span>|<span data-ttu-id="b8eb8-p108">投稿の添付ファイルが 1 つ以上あるかどうかを示します。これが既定のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-p108">Indicates whether the post has at least one attachment. This is a default property.</span></span>|
|<span data-ttu-id="b8eb8-153">id</span><span class="sxs-lookup"><span data-stu-id="b8eb8-153">id</span></span>|<span data-ttu-id="b8eb8-154">String</span><span class="sxs-lookup"><span data-stu-id="b8eb8-154">String</span></span>| <span data-ttu-id="b8eb8-155">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-155">Read-only.</span></span>|
|<span data-ttu-id="b8eb8-156">importance</span><span class="sxs-lookup"><span data-stu-id="b8eb8-156">importance</span></span> | <span data-ttu-id="b8eb8-157">String</span><span class="sxs-lookup"><span data-stu-id="b8eb8-157">String</span></span> | <span data-ttu-id="b8eb8-158">グループのポストの重要性: `low`、 `normal`、 `high`。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-158">The importance of a group post: `low`, `normal`, `high`.</span></span> |
|<span data-ttu-id="b8eb8-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8eb8-159">lastModifiedDateTime</span></span>|<span data-ttu-id="b8eb8-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8eb8-160">DateTimeOffset</span></span>|<span data-ttu-id="b8eb8-p109">投稿が最後に修正された日時を指定します。DateTimeOffset 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b8eb8-p109">Specifies when the post was last modified. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b8eb8-164">newParticipants</span><span class="sxs-lookup"><span data-stu-id="b8eb8-164">newParticipants</span></span>|<span data-ttu-id="b8eb8-165">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="b8eb8-165">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="b8eb8-166">この投稿の一部としてスレッドに追加された会話の参加者です。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-166">Conversation participants that were added to the thread as part of this post.</span></span>|
|<span data-ttu-id="b8eb8-167">receivedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8eb8-167">receivedDateTime</span></span>|<span data-ttu-id="b8eb8-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8eb8-168">DateTimeOffset</span></span>|<span data-ttu-id="b8eb8-p110">投稿の受信時刻を示します。DateTimeOffset 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b8eb8-p110">Specifies when the post was received. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b8eb8-172">sender</span><span class="sxs-lookup"><span data-stu-id="b8eb8-172">sender</span></span>|[<span data-ttu-id="b8eb8-173">recipient</span><span class="sxs-lookup"><span data-stu-id="b8eb8-173">recipient</span></span>](recipient.md)|<span data-ttu-id="b8eb8-p111">送信者のアドレスが含まれます。送信者が指定されていない場合、送信者の値は認証済みユーザーのアドレスと見なされます。これが既定のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-p111">Contains the address of the sender. The value of Sender is assumed to be the address of the authenticated user in the case when Sender is not specified. This is a default property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8eb8-177">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b8eb8-177">Relationships</span></span>
| <span data-ttu-id="b8eb8-178">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b8eb8-178">Relationship</span></span> | <span data-ttu-id="b8eb8-179">型</span><span class="sxs-lookup"><span data-stu-id="b8eb8-179">Type</span></span>   |<span data-ttu-id="b8eb8-180">説明</span><span class="sxs-lookup"><span data-stu-id="b8eb8-180">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8eb8-181">attachments</span><span class="sxs-lookup"><span data-stu-id="b8eb8-181">attachments</span></span>|<span data-ttu-id="b8eb8-182">[Attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b8eb8-182">[Attachment](attachment.md) collection</span></span>|<span data-ttu-id="b8eb8-183">投稿の[fileAttachment](fileattachment.md)、 [itemAttachment](itemattachment.md)、および[referenceAttachment](referenceattachment.md)の添付ファイルのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-183">The collection of [fileAttachment](fileattachment.md), [itemAttachment](itemattachment.md), and [referenceAttachment](referenceattachment.md) attachments for the post.</span></span> <span data-ttu-id="b8eb8-184">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-184">Read-only.</span></span> <span data-ttu-id="b8eb8-185">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-185">Nullable.</span></span>|
|<span data-ttu-id="b8eb8-186">extensions</span><span class="sxs-lookup"><span data-stu-id="b8eb8-186">extensions</span></span>|<span data-ttu-id="b8eb8-187">[Extension](extension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b8eb8-187">[Extension](extension.md) collection</span></span>|<span data-ttu-id="b8eb8-p113">投稿に対して定義されているオープン拡張機能のコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-p113">The collection of open extensions defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="b8eb8-191">inReplyTo</span><span class="sxs-lookup"><span data-stu-id="b8eb8-191">inReplyTo</span></span>|[<span data-ttu-id="b8eb8-192">Post</span><span class="sxs-lookup"><span data-stu-id="b8eb8-192">Post</span></span>](post.md)|<span data-ttu-id="b8eb8-193">[ConversationThread](conversationthread.md)でへこの投稿の返信は、以前の投稿です。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-193">The earlier post that this post is replying to in the [conversationThread](conversationthread.md).</span></span> <span data-ttu-id="b8eb8-194">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-194">Read-only.</span></span>|
|<span data-ttu-id="b8eb8-195">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="b8eb8-195">multiValueExtendedProperties</span></span>|<span data-ttu-id="b8eb8-196">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b8eb8-196">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="b8eb8-p115">その投稿用に定義された、複数値拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-p115">The collection of multi-value extended properties defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="b8eb8-200">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="b8eb8-200">singleValueExtendedProperties</span></span>|<span data-ttu-id="b8eb8-201">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b8eb8-201">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="b8eb8-p116">その投稿用に定義された、単一値拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-p116">The collection of single-value extended properties defined for the post. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="b8eb8-205">メソッド</span><span class="sxs-lookup"><span data-stu-id="b8eb8-205">Methods</span></span>

| <span data-ttu-id="b8eb8-206">メソッド</span><span class="sxs-lookup"><span data-stu-id="b8eb8-206">Method</span></span>           | <span data-ttu-id="b8eb8-207">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b8eb8-207">Return Type</span></span>    |<span data-ttu-id="b8eb8-208">説明</span><span class="sxs-lookup"><span data-stu-id="b8eb8-208">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b8eb8-209">List posts</span><span class="sxs-lookup"><span data-stu-id="b8eb8-209">List posts</span></span>](../api/conversationthread-list-posts.md) | [<span data-ttu-id="b8eb8-210">post</span><span class="sxs-lookup"><span data-stu-id="b8eb8-210">post</span></span>](post.md) |<span data-ttu-id="b8eb8-211">指定したスレッドの投稿を取得します。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-211">Get the posts of the specified thread.</span></span> |
|[<span data-ttu-id="b8eb8-212">Get post</span><span class="sxs-lookup"><span data-stu-id="b8eb8-212">Get post</span></span>](../api/post-get.md) | [<span data-ttu-id="b8eb8-213">post</span><span class="sxs-lookup"><span data-stu-id="b8eb8-213">post</span></span>](post.md) |<span data-ttu-id="b8eb8-214">指定したスレッド内の投稿のプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-214">Get the properties and relationships of a post in a specified thread.</span></span>|
|[<span data-ttu-id="b8eb8-215">Reply</span><span class="sxs-lookup"><span data-stu-id="b8eb8-215">Reply</span></span>](../api/post-reply.md)|<span data-ttu-id="b8eb8-216">なし</span><span class="sxs-lookup"><span data-stu-id="b8eb8-216">None</span></span>|<span data-ttu-id="b8eb8-217">グループ会話の投稿に返信して、指定されたスレッドに新しい投稿を追加します。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-217">Reply to a post and add a new post to the specified thread in a group conversation.</span></span>|
|[<span data-ttu-id="b8eb8-218">Forward</span><span class="sxs-lookup"><span data-stu-id="b8eb8-218">Forward</span></span>](../api/post-forward.md)|<span data-ttu-id="b8eb8-219">なし</span><span class="sxs-lookup"><span data-stu-id="b8eb8-219">None</span></span>|<span data-ttu-id="b8eb8-220">受信者に投稿を転送します。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-220">Forward a post to a recipient.</span></span>|
|<span data-ttu-id="b8eb8-221">**添付ファイル**</span><span class="sxs-lookup"><span data-stu-id="b8eb8-221">**Attachments**</span></span>| | |
|[<span data-ttu-id="b8eb8-222">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b8eb8-222">List attachments</span></span>](../api/post-list-attachments.md) |<span data-ttu-id="b8eb8-223">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b8eb8-223">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="b8eb8-224">投稿のすべての添付ファイルを取得します。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-224">Get all attachments on a post.</span></span>|
|[<span data-ttu-id="b8eb8-225">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="b8eb8-225">Add attachment</span></span>](../api/post-post-attachments.md) |[<span data-ttu-id="b8eb8-226">attachment</span><span class="sxs-lookup"><span data-stu-id="b8eb8-226">attachment</span></span>](attachment.md)| <span data-ttu-id="b8eb8-227">投稿に添付ファイルを追加します。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-227">Add an attachment to a post.</span></span> |
|<span data-ttu-id="b8eb8-228">**オープン拡張機能**</span><span class="sxs-lookup"><span data-stu-id="b8eb8-228">**Open extensions**</span></span>| | |
|[<span data-ttu-id="b8eb8-229">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="b8eb8-229">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="b8eb8-230">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="b8eb8-230">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="b8eb8-231">オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-231">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="b8eb8-232">オープン拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="b8eb8-232">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="b8eb8-233">[openTypeExtension](opentypeextension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b8eb8-233">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="b8eb8-234">拡張機能の名前で識別されるオープン拡張機能を取得します。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-234">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="b8eb8-235">**スキーマ拡張機能**</span><span class="sxs-lookup"><span data-stu-id="b8eb8-235">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="b8eb8-236">スキーマ拡張機能の値を追加する</span><span class="sxs-lookup"><span data-stu-id="b8eb8-236">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="b8eb8-237">スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-237">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="b8eb8-238">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="b8eb8-238">**Extended properties**</span></span>| | |
|[<span data-ttu-id="b8eb8-239">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="b8eb8-239">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="b8eb8-240">post</span><span class="sxs-lookup"><span data-stu-id="b8eb8-240">post</span></span>](post.md)  |<span data-ttu-id="b8eb8-241">新規または既存の投稿に、ひとつまたは複数の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-241">Create one or more single-value extended properties in a new or existing post.</span></span>   |
|[<span data-ttu-id="b8eb8-242">Get post with single-value extended property</span><span class="sxs-lookup"><span data-stu-id="b8eb8-242">Get post with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="b8eb8-243">post</span><span class="sxs-lookup"><span data-stu-id="b8eb8-243">post</span></span>](post.md) | <span data-ttu-id="b8eb8-244">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含む投稿を取得します。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-244">Get posts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="b8eb8-245">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="b8eb8-245">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="b8eb8-246">post</span><span class="sxs-lookup"><span data-stu-id="b8eb8-246">post</span></span>](post.md) | <span data-ttu-id="b8eb8-247">新規または既存の投稿に、ひとつまたは複数の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-247">Create one or more multi-value extended properties in a new or existing post.</span></span>  |
|[<span data-ttu-id="b8eb8-248">Get post with multi-value extended property</span><span class="sxs-lookup"><span data-stu-id="b8eb8-248">Get post with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="b8eb8-249">post</span><span class="sxs-lookup"><span data-stu-id="b8eb8-249">post</span></span>](post.md) | <span data-ttu-id="b8eb8-250">`$expand` を使用して、複数値の拡張プロパティを含む投稿を取得します。</span><span class="sxs-lookup"><span data-stu-id="b8eb8-250">Get a post that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="see-also"></a><span data-ttu-id="b8eb8-251">関連項目</span><span class="sxs-lookup"><span data-stu-id="b8eb8-251">See also</span></span>

- [<span data-ttu-id="b8eb8-252">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="b8eb8-252">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="b8eb8-253">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="b8eb8-253">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="b8eb8-254">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="b8eb8-254">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
