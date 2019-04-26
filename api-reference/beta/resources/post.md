---
title: post リソース タイプ
description: converstaionThread エンティティ内の個々の投稿アイテムを表します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: abfd2b19681b9821377830f1696fa6f754afd711
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344239"
---
# <a name="post-resource-type"></a><span data-ttu-id="7b301-103">post リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="7b301-103">post resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b301-104">[converstaionThread](conversationthread.md)エンティティ内の個々の投稿アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="7b301-104">Represents an individual post item within a [converstaionThread](conversationthread.md) entity.</span></span>

<span data-ttu-id="7b301-105">投稿を明示的に作成できなくても、次のいずれかの方法で投稿を作成できます。</span><span class="sxs-lookup"><span data-stu-id="7b301-105">Even though you cannot explicitly create a post, doing any of the following would create a post:</span></span>

* [<span data-ttu-id="7b301-106">既存の投稿に返信する</span><span class="sxs-lookup"><span data-stu-id="7b301-106">Reply to an existing post</span></span>](../api/post-reply.md) 
* [<span data-ttu-id="7b301-107">既存のスレッドに返信する</span><span class="sxs-lookup"><span data-stu-id="7b301-107">Reply to an existing thread</span></span>](../api/conversationthread-reply.md) 
* [<span data-ttu-id="7b301-108">新しい会話にスレッドを作成する</span><span class="sxs-lookup"><span data-stu-id="7b301-108">Create a thread in a new conversation</span></span>](../api/group-post-threads.md)
* [<span data-ttu-id="7b301-109">新しい会話を作成する</span><span class="sxs-lookup"><span data-stu-id="7b301-109">Create a new conversation</span></span>](../api/group-post-conversations.md)

<span data-ttu-id="7b301-110">このリソースでは、[拡張機能](/graph/extensibility-overview)を使用してカスタム プロパティに独自のデータを追加することができます。</span><span class="sxs-lookup"><span data-stu-id="7b301-110">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b301-111">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7b301-111">JSON representation</span></span>

<span data-ttu-id="7b301-112">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="7b301-112">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "extensions",
    "inReplyTo",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
## <a name="properties"></a><span data-ttu-id="7b301-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b301-113">Properties</span></span>
| <span data-ttu-id="7b301-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b301-114">Property</span></span>     | <span data-ttu-id="7b301-115">型</span><span class="sxs-lookup"><span data-stu-id="7b301-115">Type</span></span>   |<span data-ttu-id="7b301-116">説明</span><span class="sxs-lookup"><span data-stu-id="7b301-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b301-117">body</span><span class="sxs-lookup"><span data-stu-id="7b301-117">body</span></span>|[<span data-ttu-id="7b301-118">itemBody</span><span class="sxs-lookup"><span data-stu-id="7b301-118">itemBody</span></span>](itembody.md)|<span data-ttu-id="7b301-p101">投稿の内容です。これが既定のプロパティです。このプロパティを null にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7b301-p101">The contents of the post. This is a default property. This property can be null.</span></span>|
|<span data-ttu-id="7b301-122">categories</span><span class="sxs-lookup"><span data-stu-id="7b301-122">categories</span></span>|<span data-ttu-id="7b301-123">String collection</span><span class="sxs-lookup"><span data-stu-id="7b301-123">String collection</span></span>|<span data-ttu-id="7b301-124">投稿に関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="7b301-124">The categories associated with the post.</span></span> <span data-ttu-id="7b301-125">各カテゴリは、ユーザーに対して定義されている[outlookcategory](outlookcategory.md)の**displayName**プロパティに対応しています。</span><span class="sxs-lookup"><span data-stu-id="7b301-125">Each category corresponds to the **displayName** property of an [outlookCategory](outlookcategory.md) that has been defined for a user.</span></span>|
|<span data-ttu-id="7b301-126">changeKey</span><span class="sxs-lookup"><span data-stu-id="7b301-126">changeKey</span></span>|<span data-ttu-id="7b301-127">String</span><span class="sxs-lookup"><span data-stu-id="7b301-127">String</span></span>|<span data-ttu-id="7b301-p103">投稿のバージョンを識別します。投稿を変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。</span><span class="sxs-lookup"><span data-stu-id="7b301-p103">Identifies the version of the post. Every time the post is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="7b301-131">conversationId</span><span class="sxs-lookup"><span data-stu-id="7b301-131">conversationId</span></span>|<span data-ttu-id="7b301-132">String</span><span class="sxs-lookup"><span data-stu-id="7b301-132">String</span></span>|<span data-ttu-id="7b301-p104">会話の固有 ID です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="7b301-p104">Unique ID of the conversation. Read-only.</span></span>|
|<span data-ttu-id="7b301-135">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="7b301-135">conversationThreadId</span></span>|<span data-ttu-id="7b301-136">String</span><span class="sxs-lookup"><span data-stu-id="7b301-136">String</span></span>|<span data-ttu-id="7b301-p105">会話スレッドの固有 ID です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="7b301-p105">Unique ID of the conversation thread. Read-only.</span></span>|
|<span data-ttu-id="7b301-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7b301-139">createdDateTime</span></span>|<span data-ttu-id="7b301-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b301-140">DateTimeOffset</span></span>|<span data-ttu-id="7b301-p106">投稿の作成時刻を示します。DateTimeOffset 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7b301-p106">Specifies when the post was created. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7b301-144">from</span><span class="sxs-lookup"><span data-stu-id="7b301-144">from</span></span>|[<span data-ttu-id="7b301-145">recipient</span><span class="sxs-lookup"><span data-stu-id="7b301-145">recipient</span></span>](recipient.md)|<span data-ttu-id="7b301-p107">代理人アクセスのシナリオで使用されます。他のユーザーの代わりにメッセージを投稿したユーザーを示します。これが既定のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="7b301-p107">Used in delegate access scenarios. Indicates who posted the message on behalf of another user. This is a default property.</span></span>|
|<span data-ttu-id="7b301-149">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="7b301-149">hasAttachments</span></span>|<span data-ttu-id="7b301-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b301-150">Boolean</span></span>|<span data-ttu-id="7b301-p108">投稿の添付ファイルが 1 つ以上あるかどうかを示します。これが既定のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="7b301-p108">Indicates whether the post has at least one attachment. This is a default property.</span></span>|
|<span data-ttu-id="7b301-153">id</span><span class="sxs-lookup"><span data-stu-id="7b301-153">id</span></span>|<span data-ttu-id="7b301-154">String</span><span class="sxs-lookup"><span data-stu-id="7b301-154">String</span></span>| <span data-ttu-id="7b301-155">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7b301-155">Read-only.</span></span>|
|<span data-ttu-id="7b301-156">importance</span><span class="sxs-lookup"><span data-stu-id="7b301-156">importance</span></span> | <span data-ttu-id="7b301-157">String</span><span class="sxs-lookup"><span data-stu-id="7b301-157">String</span></span> | <span data-ttu-id="7b301-158">グループ投稿の重要度: `low`、 `normal`、。 `high`</span><span class="sxs-lookup"><span data-stu-id="7b301-158">The importance of a group post: `low`, `normal`, `high`.</span></span> |
|<span data-ttu-id="7b301-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b301-159">lastModifiedDateTime</span></span>|<span data-ttu-id="7b301-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b301-160">DateTimeOffset</span></span>|<span data-ttu-id="7b301-p109">投稿が最後に修正された日時を指定します。DateTimeOffset 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7b301-p109">Specifies when the post was last modified. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7b301-164">newparticipants</span><span class="sxs-lookup"><span data-stu-id="7b301-164">newParticipants</span></span>|<span data-ttu-id="7b301-165">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="7b301-165">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="7b301-166">この投稿の一部としてスレッドに追加された会話の参加者です。</span><span class="sxs-lookup"><span data-stu-id="7b301-166">Conversation participants that were added to the thread as part of this post.</span></span>|
|<span data-ttu-id="7b301-167">receivedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b301-167">receivedDateTime</span></span>|<span data-ttu-id="7b301-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b301-168">DateTimeOffset</span></span>|<span data-ttu-id="7b301-p110">投稿の受信時刻を示します。DateTimeOffset 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7b301-p110">Specifies when the post was received. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7b301-172">sender</span><span class="sxs-lookup"><span data-stu-id="7b301-172">sender</span></span>|[<span data-ttu-id="7b301-173">recipient</span><span class="sxs-lookup"><span data-stu-id="7b301-173">recipient</span></span>](recipient.md)|<span data-ttu-id="7b301-p111">送信者のアドレスが含まれます。送信者が指定されていない場合、送信者の値は認証済みユーザーのアドレスと見なされます。これが既定のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="7b301-p111">Contains the address of the sender. The value of Sender is assumed to be the address of the authenticated user in the case when Sender is not specified. This is a default property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b301-177">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7b301-177">Relationships</span></span>
| <span data-ttu-id="7b301-178">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7b301-178">Relationship</span></span> | <span data-ttu-id="7b301-179">型</span><span class="sxs-lookup"><span data-stu-id="7b301-179">Type</span></span>   |<span data-ttu-id="7b301-180">説明</span><span class="sxs-lookup"><span data-stu-id="7b301-180">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b301-181">attachments</span><span class="sxs-lookup"><span data-stu-id="7b301-181">attachments</span></span>|<span data-ttu-id="7b301-182">[Attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7b301-182">[Attachment](attachment.md) collection</span></span>|<span data-ttu-id="7b301-183">投稿の[fileattachment](fileattachment.md)、 [itemattachment](itemattachment.md)、および[referenceattachment](referenceattachment.md)添付ファイルのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="7b301-183">The collection of [fileAttachment](fileattachment.md), [itemAttachment](itemattachment.md), and [referenceAttachment](referenceattachment.md) attachments for the post.</span></span> <span data-ttu-id="7b301-184">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7b301-184">Read-only.</span></span> <span data-ttu-id="7b301-185">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="7b301-185">Nullable.</span></span>|
|<span data-ttu-id="7b301-186">extensions</span><span class="sxs-lookup"><span data-stu-id="7b301-186">extensions</span></span>|<span data-ttu-id="7b301-187">[Extension](extension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7b301-187">[Extension](extension.md) collection</span></span>|<span data-ttu-id="7b301-p113">投稿に対して定義されているオープン拡張機能のコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="7b301-p113">The collection of open extensions defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="7b301-191">inreplyto</span><span class="sxs-lookup"><span data-stu-id="7b301-191">inReplyTo</span></span>|[<span data-ttu-id="7b301-192">Post</span><span class="sxs-lookup"><span data-stu-id="7b301-192">Post</span></span>](post.md)|<span data-ttu-id="7b301-193">この投稿が[conversationThread](conversationthread.md)内で返信する以前の投稿。</span><span class="sxs-lookup"><span data-stu-id="7b301-193">The earlier post that this post is replying to in the [conversationThread](conversationthread.md).</span></span> <span data-ttu-id="7b301-194">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="7b301-194">Read-only.</span></span>|
|<span data-ttu-id="7b301-195">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="7b301-195">multiValueExtendedProperties</span></span>|<span data-ttu-id="7b301-196">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7b301-196">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="7b301-p115">その投稿用に定義された、複数値拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="7b301-p115">The collection of multi-value extended properties defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="7b301-200">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="7b301-200">singleValueExtendedProperties</span></span>|<span data-ttu-id="7b301-201">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7b301-201">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="7b301-p116">その投稿用に定義された、単一値拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="7b301-p116">The collection of single-value extended properties defined for the post. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="7b301-205">メソッド</span><span class="sxs-lookup"><span data-stu-id="7b301-205">Methods</span></span>

| <span data-ttu-id="7b301-206">メソッド</span><span class="sxs-lookup"><span data-stu-id="7b301-206">Method</span></span>           | <span data-ttu-id="7b301-207">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7b301-207">Return Type</span></span>    |<span data-ttu-id="7b301-208">説明</span><span class="sxs-lookup"><span data-stu-id="7b301-208">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7b301-209">List posts</span><span class="sxs-lookup"><span data-stu-id="7b301-209">List posts</span></span>](../api/conversationthread-list-posts.md) | [<span data-ttu-id="7b301-210">post</span><span class="sxs-lookup"><span data-stu-id="7b301-210">post</span></span>](post.md) |<span data-ttu-id="7b301-211">指定したスレッドの投稿を取得します。</span><span class="sxs-lookup"><span data-stu-id="7b301-211">Get the posts of the specified thread.</span></span> |
|[<span data-ttu-id="7b301-212">Get post</span><span class="sxs-lookup"><span data-stu-id="7b301-212">Get post</span></span>](../api/post-get.md) | [<span data-ttu-id="7b301-213">post</span><span class="sxs-lookup"><span data-stu-id="7b301-213">post</span></span>](post.md) |<span data-ttu-id="7b301-214">指定したスレッド内の投稿のプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="7b301-214">Get the properties and relationships of a post in a specified thread.</span></span>|
|[<span data-ttu-id="7b301-215">Reply</span><span class="sxs-lookup"><span data-stu-id="7b301-215">Reply</span></span>](../api/post-reply.md)|<span data-ttu-id="7b301-216">なし</span><span class="sxs-lookup"><span data-stu-id="7b301-216">None</span></span>|<span data-ttu-id="7b301-217">グループ会話の投稿に返信して、指定されたスレッドに新しい投稿を追加します。</span><span class="sxs-lookup"><span data-stu-id="7b301-217">Reply to a post and add a new post to the specified thread in a group conversation.</span></span>|
|[<span data-ttu-id="7b301-218">Forward</span><span class="sxs-lookup"><span data-stu-id="7b301-218">Forward</span></span>](../api/post-forward.md)|<span data-ttu-id="7b301-219">なし</span><span class="sxs-lookup"><span data-stu-id="7b301-219">None</span></span>|<span data-ttu-id="7b301-220">受信者に投稿を転送します。</span><span class="sxs-lookup"><span data-stu-id="7b301-220">Forward a post to a recipient.</span></span>|
|<span data-ttu-id="7b301-221">**Attachments**</span><span class="sxs-lookup"><span data-stu-id="7b301-221">**Attachments**</span></span>| | |
|[<span data-ttu-id="7b301-222">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7b301-222">List attachments</span></span>](../api/post-list-attachments.md) |<span data-ttu-id="7b301-223">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7b301-223">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="7b301-224">投稿のすべての添付ファイルを取得します。</span><span class="sxs-lookup"><span data-stu-id="7b301-224">Get all attachments on a post.</span></span>|
|[<span data-ttu-id="7b301-225">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="7b301-225">Add attachment</span></span>](../api/post-post-attachments.md) |[<span data-ttu-id="7b301-226">attachment</span><span class="sxs-lookup"><span data-stu-id="7b301-226">attachment</span></span>](attachment.md)| <span data-ttu-id="7b301-227">投稿に添付ファイルを追加します。</span><span class="sxs-lookup"><span data-stu-id="7b301-227">Add an attachment to a post.</span></span> |
|<span data-ttu-id="7b301-228">**オープン拡張機能**</span><span class="sxs-lookup"><span data-stu-id="7b301-228">**Open extensions**</span></span>| | |
|[<span data-ttu-id="7b301-229">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="7b301-229">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="7b301-230">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="7b301-230">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="7b301-231">オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="7b301-231">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="7b301-232">オープン拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="7b301-232">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="7b301-233">[openTypeExtension](opentypeextension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7b301-233">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="7b301-234">拡張機能の名前で識別されるオープン拡張機能を取得します。</span><span class="sxs-lookup"><span data-stu-id="7b301-234">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="7b301-235">**スキーマ拡張機能**</span><span class="sxs-lookup"><span data-stu-id="7b301-235">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="7b301-236">スキーマ拡張機能の値を追加する</span><span class="sxs-lookup"><span data-stu-id="7b301-236">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="7b301-237">スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。</span><span class="sxs-lookup"><span data-stu-id="7b301-237">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="7b301-238">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="7b301-238">**Extended properties**</span></span>| | |
|[<span data-ttu-id="7b301-239">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="7b301-239">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="7b301-240">post</span><span class="sxs-lookup"><span data-stu-id="7b301-240">post</span></span>](post.md)  |<span data-ttu-id="7b301-241">新規または既存の投稿に、ひとつまたは複数の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="7b301-241">Create one or more single-value extended properties in a new or existing post.</span></span>   |
|[<span data-ttu-id="7b301-242">Get post with single-value extended property</span><span class="sxs-lookup"><span data-stu-id="7b301-242">Get post with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="7b301-243">post</span><span class="sxs-lookup"><span data-stu-id="7b301-243">post</span></span>](post.md) | <span data-ttu-id="7b301-244">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含む投稿を取得します。</span><span class="sxs-lookup"><span data-stu-id="7b301-244">Get posts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="7b301-245">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="7b301-245">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="7b301-246">post</span><span class="sxs-lookup"><span data-stu-id="7b301-246">post</span></span>](post.md) | <span data-ttu-id="7b301-247">新規または既存の投稿に、ひとつまたは複数の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="7b301-247">Create one or more multi-value extended properties in a new or existing post.</span></span>  |
|[<span data-ttu-id="7b301-248">Get post with multi-value extended property</span><span class="sxs-lookup"><span data-stu-id="7b301-248">Get post with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="7b301-249">post</span><span class="sxs-lookup"><span data-stu-id="7b301-249">post</span></span>](post.md) | <span data-ttu-id="7b301-250">`$expand` を使用して、複数値の拡張プロパティを含む投稿を取得します。</span><span class="sxs-lookup"><span data-stu-id="7b301-250">Get a post that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="see-also"></a><span data-ttu-id="7b301-251">関連項目</span><span class="sxs-lookup"><span data-stu-id="7b301-251">See also</span></span>

- [<span data-ttu-id="7b301-252">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="7b301-252">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7b301-253">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="7b301-253">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="7b301-254">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="7b301-254">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
