---
title: post リソース タイプ
description: conversationThread エンティティ内の個々の投稿アイテムを表します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 43837b1403b7b213b1b8a30002aeb53b8fa297a1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035099"
---
# <a name="post-resource-type"></a><span data-ttu-id="4eaa3-103">post リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="4eaa3-103">post resource type</span></span>
<span data-ttu-id="4eaa3-104">[conversationThread](conversationthread.md) エンティティ内の個々の投稿アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-104">Represents an individual Post item within a [conversationThread](conversationthread.md) entity.</span></span>

<span data-ttu-id="4eaa3-105">投稿を明示的に作成できなくても、次のいずれかの方法で投稿を作成できます。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-105">Even though you cannot explicitly create a post, doing any of the following would create a post:</span></span>

- [<span data-ttu-id="4eaa3-106">既存の投稿に返信する</span><span class="sxs-lookup"><span data-stu-id="4eaa3-106">Reply to an existing post</span></span>](../api/post-reply.md) 
- [<span data-ttu-id="4eaa3-107">既存のスレッドに返信する</span><span class="sxs-lookup"><span data-stu-id="4eaa3-107">Reply to an existing thread</span></span>](../api/conversationthread-reply.md) 
- [<span data-ttu-id="4eaa3-108">新しい会話にスレッドを作成する</span><span class="sxs-lookup"><span data-stu-id="4eaa3-108">Create a thread in a new conversation</span></span>](../api/group-post-threads.md)
- [<span data-ttu-id="4eaa3-109">新しい会話を作成する</span><span class="sxs-lookup"><span data-stu-id="4eaa3-109">Create a new conversation</span></span>](../api/group-post-conversations.md)

<span data-ttu-id="4eaa3-110">このリソースでは、[拡張機能](/graph/extensibility-overview)を使用してカスタム プロパティに独自のデータを追加することができます。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-110">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="4eaa3-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="4eaa3-111">Methods</span></span>

| <span data-ttu-id="4eaa3-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="4eaa3-112">Method</span></span>       | <span data-ttu-id="4eaa3-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4eaa3-113">Return Type</span></span>  |<span data-ttu-id="4eaa3-114">説明</span><span class="sxs-lookup"><span data-stu-id="4eaa3-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4eaa3-115">List posts</span><span class="sxs-lookup"><span data-stu-id="4eaa3-115">List posts</span></span>](../api/conversationthread-list-posts.md) | [<span data-ttu-id="4eaa3-116">post</span><span class="sxs-lookup"><span data-stu-id="4eaa3-116">post</span></span>](post.md) |<span data-ttu-id="4eaa3-117">指定したスレッドの投稿を取得します。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-117">Get the posts of the specified thread.</span></span> |
|[<span data-ttu-id="4eaa3-118">Get post</span><span class="sxs-lookup"><span data-stu-id="4eaa3-118">Get post</span></span>](../api/post-get.md) | [<span data-ttu-id="4eaa3-119">post</span><span class="sxs-lookup"><span data-stu-id="4eaa3-119">post</span></span>](post.md) |<span data-ttu-id="4eaa3-120">指定したスレッド内の投稿のプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-120">Get the properties and relationships of a post in a specified thread.</span></span>|
|[<span data-ttu-id="4eaa3-121">Reply</span><span class="sxs-lookup"><span data-stu-id="4eaa3-121">Reply</span></span>](../api/post-reply.md)|<span data-ttu-id="4eaa3-122">None</span><span class="sxs-lookup"><span data-stu-id="4eaa3-122">None</span></span>|<span data-ttu-id="4eaa3-123">グループ会話の投稿に返信して、指定されたスレッドに新しい投稿を追加します。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-123">Reply to a post and add a new post to the specified thread in a group conversation.</span></span>|
|[<span data-ttu-id="4eaa3-124">Forward</span><span class="sxs-lookup"><span data-stu-id="4eaa3-124">Forward</span></span>](../api/post-forward.md)|<span data-ttu-id="4eaa3-125">なし</span><span class="sxs-lookup"><span data-stu-id="4eaa3-125">None</span></span>|<span data-ttu-id="4eaa3-126">受信者に投稿を転送します。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-126">Forward a post to a recipient.</span></span>|
|<span data-ttu-id="4eaa3-127">**添付ファイル**</span><span class="sxs-lookup"><span data-stu-id="4eaa3-127">**Attachments**</span></span>| | |
|[<span data-ttu-id="4eaa3-128">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="4eaa3-128">List attachments</span></span>](../api/post-list-attachments.md) |<span data-ttu-id="4eaa3-129">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4eaa3-129">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="4eaa3-130">投稿のすべての添付ファイルを取得します。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-130">Get all attachments on a post.</span></span>|
|[<span data-ttu-id="4eaa3-131">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="4eaa3-131">Add attachment</span></span>](../api/post-post-attachments.md) |[<span data-ttu-id="4eaa3-132">attachment</span><span class="sxs-lookup"><span data-stu-id="4eaa3-132">attachment</span></span>](attachment.md)| <span data-ttu-id="4eaa3-133">投稿に添付ファイルを追加します。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-133">Add an attachment to a post.</span></span> |
|<span data-ttu-id="4eaa3-134">**オープン拡張機能**</span><span class="sxs-lookup"><span data-stu-id="4eaa3-134">**Open extensions**</span></span>| | |
|[<span data-ttu-id="4eaa3-135">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="4eaa3-135">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="4eaa3-136">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="4eaa3-136">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="4eaa3-137">オープン拡張機能を作成し、リソースの新規または既存のインスタンスのカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-137">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="4eaa3-138">オープン拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="4eaa3-138">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="4eaa3-139">[openTypeExtension](opentypeextension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4eaa3-139">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="4eaa3-140">名前や完全修飾名によって識別されたオープン拡張機能オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-140">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="4eaa3-141">**スキーマ拡張機能**</span><span class="sxs-lookup"><span data-stu-id="4eaa3-141">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="4eaa3-142">スキーマ拡張機能の値を追加する</span><span class="sxs-lookup"><span data-stu-id="4eaa3-142">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="4eaa3-143">スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-143">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="4eaa3-144">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="4eaa3-144">**Extended properties**</span></span>| | |
|[<span data-ttu-id="4eaa3-145">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="4eaa3-145">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="4eaa3-146">post</span><span class="sxs-lookup"><span data-stu-id="4eaa3-146">post</span></span>](post.md)  |<span data-ttu-id="4eaa3-147">新規または既存の投稿に、ひとつまたは複数の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-147">Create one or more single-value extended properties in a new or existing post.</span></span>   |
|[<span data-ttu-id="4eaa3-148">Get post with single-value extended property</span><span class="sxs-lookup"><span data-stu-id="4eaa3-148">Get post with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="4eaa3-149">post</span><span class="sxs-lookup"><span data-stu-id="4eaa3-149">post</span></span>](post.md) | <span data-ttu-id="4eaa3-150">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含む投稿を取得します。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-150">Get posts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="4eaa3-151">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="4eaa3-151">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="4eaa3-152">post</span><span class="sxs-lookup"><span data-stu-id="4eaa3-152">post</span></span>](post.md) | <span data-ttu-id="4eaa3-153">新規または既存の投稿に、ひとつまたは複数の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-153">Create one or more multi-value extended properties in a new or existing post.</span></span>  |
|[<span data-ttu-id="4eaa3-154">Get post with multi-value extended property</span><span class="sxs-lookup"><span data-stu-id="4eaa3-154">Get post with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="4eaa3-155">post</span><span class="sxs-lookup"><span data-stu-id="4eaa3-155">post</span></span>](post.md) | <span data-ttu-id="4eaa3-156">`$expand` を使用して、複数値の拡張プロパティを含む投稿を取得します。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-156">Get a post that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="4eaa3-157">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4eaa3-157">Properties</span></span>
| <span data-ttu-id="4eaa3-158">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4eaa3-158">Property</span></span>     | <span data-ttu-id="4eaa3-159">型</span><span class="sxs-lookup"><span data-stu-id="4eaa3-159">Type</span></span>   |<span data-ttu-id="4eaa3-160">説明</span><span class="sxs-lookup"><span data-stu-id="4eaa3-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4eaa3-161">body</span><span class="sxs-lookup"><span data-stu-id="4eaa3-161">body</span></span>|[<span data-ttu-id="4eaa3-162">itemBody</span><span class="sxs-lookup"><span data-stu-id="4eaa3-162">itemBody</span></span>](itembody.md)|<span data-ttu-id="4eaa3-p101">投稿の内容です。これが既定のプロパティです。このプロパティを null にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-p101">The contents of the post. This is a default property. This property can be null.</span></span>|
|<span data-ttu-id="4eaa3-166">categories</span><span class="sxs-lookup"><span data-stu-id="4eaa3-166">categories</span></span>|<span data-ttu-id="4eaa3-167">String collection</span><span class="sxs-lookup"><span data-stu-id="4eaa3-167">String collection</span></span>|<span data-ttu-id="4eaa3-168">投稿に関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-168">The categories associated with the post.</span></span>|
|<span data-ttu-id="4eaa3-169">changeKey</span><span class="sxs-lookup"><span data-stu-id="4eaa3-169">changeKey</span></span>|<span data-ttu-id="4eaa3-170">String</span><span class="sxs-lookup"><span data-stu-id="4eaa3-170">String</span></span>|<span data-ttu-id="4eaa3-p102">投稿のバージョンを識別します。投稿を変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-p102">Identifies the version of the post. Every time the post is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="4eaa3-174">conversationId</span><span class="sxs-lookup"><span data-stu-id="4eaa3-174">conversationId</span></span>|<span data-ttu-id="4eaa3-175">String</span><span class="sxs-lookup"><span data-stu-id="4eaa3-175">String</span></span>|<span data-ttu-id="4eaa3-p103">会話の固有 ID です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-p103">Unique ID of the conversation. Read-only.</span></span>|
|<span data-ttu-id="4eaa3-178">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="4eaa3-178">conversationThreadId</span></span>|<span data-ttu-id="4eaa3-179">String</span><span class="sxs-lookup"><span data-stu-id="4eaa3-179">String</span></span>|<span data-ttu-id="4eaa3-p104">会話スレッドの固有 ID です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-p104">Unique ID of the conversation thread. Read-only.</span></span>|
|<span data-ttu-id="4eaa3-182">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4eaa3-182">createdDateTime</span></span>|<span data-ttu-id="4eaa3-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4eaa3-183">DateTimeOffset</span></span>|<span data-ttu-id="4eaa3-p105">投稿の作成時刻を示します。DateTimeOffset 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4eaa3-p105">Specifies when the post was created. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4eaa3-187">from</span><span class="sxs-lookup"><span data-stu-id="4eaa3-187">from</span></span>|[<span data-ttu-id="4eaa3-188">recipient</span><span class="sxs-lookup"><span data-stu-id="4eaa3-188">recipient</span></span>](recipient.md)|<span data-ttu-id="4eaa3-p106">代理人アクセスのシナリオで使用されます。他のユーザーの代わりにメッセージを投稿したユーザーを示します。これが既定のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-p106">Used in delegate access scenarios. Indicates who posted the message on behalf of another user. This is a default property.</span></span>|
|<span data-ttu-id="4eaa3-192">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="4eaa3-192">hasAttachments</span></span>|<span data-ttu-id="4eaa3-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="4eaa3-193">Boolean</span></span>|<span data-ttu-id="4eaa3-p107">投稿の添付ファイルが 1 つ以上あるかどうかを示します。これが既定のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-p107">Indicates whether the post has at least one attachment. This is a default property.</span></span>|
|<span data-ttu-id="4eaa3-196">id</span><span class="sxs-lookup"><span data-stu-id="4eaa3-196">id</span></span>|<span data-ttu-id="4eaa3-197">String</span><span class="sxs-lookup"><span data-stu-id="4eaa3-197">String</span></span>| <span data-ttu-id="4eaa3-198">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-198">Read-only.</span></span>|
|<span data-ttu-id="4eaa3-199">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4eaa3-199">lastModifiedDateTime</span></span>|<span data-ttu-id="4eaa3-200">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4eaa3-200">DateTimeOffset</span></span>|<span data-ttu-id="4eaa3-p108">投稿が最後に修正された日時を指定します。DateTimeOffset 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4eaa3-p108">Specifies when the post was last modified. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4eaa3-204">newParticipants</span><span class="sxs-lookup"><span data-stu-id="4eaa3-204">newParticipants</span></span>|<span data-ttu-id="4eaa3-205">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="4eaa3-205">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="4eaa3-206">この投稿の一部としてスレッドに追加された会話の参加者です。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-206">Conversation participants that were added to the thread as part of this post.</span></span>|
|<span data-ttu-id="4eaa3-207">receivedDateTime</span><span class="sxs-lookup"><span data-stu-id="4eaa3-207">receivedDateTime</span></span>|<span data-ttu-id="4eaa3-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4eaa3-208">DateTimeOffset</span></span>|<span data-ttu-id="4eaa3-p109">投稿の受信時刻を示します。DateTimeOffset 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4eaa3-p109">Specifies when the post was received. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4eaa3-212">sender</span><span class="sxs-lookup"><span data-stu-id="4eaa3-212">sender</span></span>|[<span data-ttu-id="4eaa3-213">recipient</span><span class="sxs-lookup"><span data-stu-id="4eaa3-213">recipient</span></span>](recipient.md)|<span data-ttu-id="4eaa3-p110">送信者のアドレスが含まれます。送信者が指定されていない場合、送信者の値は認証済みユーザーのアドレスと見なされます。これが既定のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-p110">Contains the address of the sender. The value of Sender is assumed to be the address of the authenticated user in the case when Sender is not specified. This is a default property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4eaa3-217">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4eaa3-217">Relationships</span></span>
| <span data-ttu-id="4eaa3-218">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4eaa3-218">Relationship</span></span> | <span data-ttu-id="4eaa3-219">型</span><span class="sxs-lookup"><span data-stu-id="4eaa3-219">Type</span></span>   |<span data-ttu-id="4eaa3-220">説明</span><span class="sxs-lookup"><span data-stu-id="4eaa3-220">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4eaa3-221">attachments</span><span class="sxs-lookup"><span data-stu-id="4eaa3-221">attachments</span></span>|<span data-ttu-id="4eaa3-222">[Attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4eaa3-222">[Attachment](attachment.md) collection</span></span>| <span data-ttu-id="4eaa3-p111">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-p111">Read-only. Nullable.</span></span>|
|<span data-ttu-id="4eaa3-225">extensions</span><span class="sxs-lookup"><span data-stu-id="4eaa3-225">extensions</span></span>|<span data-ttu-id="4eaa3-226">[Extension](extension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4eaa3-226">[Extension](extension.md) collection</span></span>|<span data-ttu-id="4eaa3-p112">投稿に対して定義されているオープン拡張機能のコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-p112">The collection of open extensions defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="4eaa3-230">inReplyTo</span><span class="sxs-lookup"><span data-stu-id="4eaa3-230">inReplyTo</span></span>|[<span data-ttu-id="4eaa3-231">post</span><span class="sxs-lookup"><span data-stu-id="4eaa3-231">post</span></span>](post.md)| <span data-ttu-id="4eaa3-232">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-232">Read-only.</span></span>|
|<span data-ttu-id="4eaa3-233">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="4eaa3-233">multiValueExtendedProperties</span></span>|<span data-ttu-id="4eaa3-234">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4eaa3-234">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="4eaa3-p113">その投稿用に定義された、複数値拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-p113">The collection of multi-value extended properties defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="4eaa3-238">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="4eaa3-238">singleValueExtendedProperties</span></span>|<span data-ttu-id="4eaa3-239">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4eaa3-239">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="4eaa3-p114">その投稿用に定義された、単一値拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4eaa3-p114">The collection of single-value extended properties defined for the post. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4eaa3-243">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4eaa3-243">JSON representation</span></span>

<span data-ttu-id="4eaa3-244">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="4eaa3-244">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "attachments",
    "inReplyTo",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "baseType": "microsoft.graph.outlookItem",
  "@odata.type": "microsoft.graph.post",
  "@odata.annotations": [
    {
      "property": "attachments",
      "capabilities": {
        "changeTracking": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "extensions",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "inReplyTo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    }
  ]
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
  "lastModifiedDateTime": "String (timestamp)",
  "newParticipants": [{"@odata.type": "microsoft.graph.recipient"}],
  "receivedDateTime": "String (timestamp)",
  "sender": {"@odata.type": "microsoft.graph.recipient"}
}

```

## <a name="see-also"></a><span data-ttu-id="4eaa3-245">関連項目</span><span class="sxs-lookup"><span data-stu-id="4eaa3-245">See also</span></span>

- [<span data-ttu-id="4eaa3-246">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="4eaa3-246">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="4eaa3-247">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="4eaa3-247">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="4eaa3-248">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="4eaa3-248">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
