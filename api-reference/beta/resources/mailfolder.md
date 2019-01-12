---
title: mailFolder リソースの種類
description: 受信トレイや下書きなどの、ユーザーのメールボックス内のメール フォルダーです。 メール フォルダーには、メッセージ、他の Outlook アイテム、子メール フォルダーを含めることができます。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: eaccaf02a3d81d184b3c0bf9eae737790c2709d7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923258"
---
# <a name="mailfolder-resource-type"></a><span data-ttu-id="bc5a4-104">mailFolder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bc5a4-104">mailFolder resource type</span></span>

> <span data-ttu-id="bc5a4-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc5a4-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bc5a4-107">受信トレイや下書きなどの、ユーザーのメールボックス内のメール フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-107">A mail folder in a user's mailbox, such as Inbox and Drafts.</span></span> <span data-ttu-id="bc5a4-108">メール フォルダーには、メッセージ、他の Outlook アイテム、子メール フォルダーを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-108">Mail folders can contain messages, other Outlook items, and child mail folders.</span></span>

<span data-ttu-id="bc5a4-109">このリソースでは、[デルタ](../api/mailfolder-delta.md)関数を用意すれば、増分の追加、削除、更新に[デルタ クエリ](/graph/delta-query-overview)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-109">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/mailfolder-delta.md) function.</span></span>

<span data-ttu-id="bc5a4-110">**既知のフォルダー名**</span><span class="sxs-lookup"><span data-stu-id="bc5a4-110">**Well-known folder names**</span></span>

<span data-ttu-id="bc5a4-111">Outlook では、既定でユーザー用の特定のフォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-111">Outlook creates certain folders for users by default.</span></span> <span data-ttu-id="bc5a4-112">対応するフォルダーの**id**値を使用して、利便性のため、代わりにこれらのフォルダーにアクセスするときに既知のフォルダー名を次の表からを使用できます。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-112">Instead of using the corresponding folder **id** value, for convenience, you can use the well-known folder names from the table below when accessing these folders.</span></span> <span data-ttu-id="bc5a4-113">たとえば、次のクエリを使用して、既知の名前を使用して、[下書き] フォルダーを取得できます。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-113">For example, you can get the Drafts folder using its well-known name with the following query.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

<span data-ttu-id="bc5a4-114">既知の名前は、上記のクエリは、常に付けの方法に関係なく、ユーザーの [下書き] フォルダーを返しますので、ユーザーのメールボックスのロケールに関係なく動作します。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-114">Well-known names work regardless of the locale of the user's mailbox, so the above query will always return the user's Drafts folder regardless of how it is named.</span></span>

| <span data-ttu-id="bc5a4-115">既知のフォルダー名</span><span class="sxs-lookup"><span data-stu-id="bc5a4-115">Well-known folder name</span></span> | <span data-ttu-id="bc5a4-116">説明</span><span class="sxs-lookup"><span data-stu-id="bc5a4-116">Description</span></span> |
|:-----------------------|:------------|
| <span data-ttu-id="bc5a4-117">アーカイブ</span><span class="sxs-lookup"><span data-stu-id="bc5a4-117">archive</span></span> | <span data-ttu-id="bc5a4-118">アーカイブ フォルダーのメッセージは、サポートしている Outlook クライアントで One_Click のアーカイブ機能を使用する場合に送信されます。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-118">The archive folder messages are sent to when using the One_Click Archive feature in Outlook clients that support it.</span></span> <span data-ttu-id="bc5a4-119">**注:** これは Exchange のメールボックスのアーカイブの機能は、オンラインの場合と同じです。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-119">**Note:** this is not the same as the Archive Mailbox feature of Exchange online.</span></span> |
| <span data-ttu-id="bc5a4-120">散乱</span><span class="sxs-lookup"><span data-stu-id="bc5a4-120">clutter</span></span> | <span data-ttu-id="bc5a4-121">整理フォルダーの優先順位の低いメッセージは、整理機能を使用するときに移動されます。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-121">The clutter folder low-priority messages are moved to when using the Clutter feature.</span></span> |
| <span data-ttu-id="bc5a4-122">競合</span><span class="sxs-lookup"><span data-stu-id="bc5a4-122">conflicts</span></span> | <span data-ttu-id="bc5a4-123">メールボックスにある競合アイテムを含むフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-123">The folder that contains conflicting items in the mailbox.</span></span> |
| <span data-ttu-id="bc5a4-124">conversationhistory</span><span class="sxs-lookup"><span data-stu-id="bc5a4-124">conversationhistory</span></span> | <span data-ttu-id="bc5a4-125">(これを行うには、Skype が構成されている) 場合に、Skype が IM の会話を保存するフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-125">The folder where Skype saves IM conversations (if Skype is configured to do so).</span></span> |
| <span data-ttu-id="bc5a4-126">deleteditems</span><span class="sxs-lookup"><span data-stu-id="bc5a4-126">deleteditems</span></span> | <span data-ttu-id="bc5a4-127">フォルダーのアイテムは、削除するときに移動されます。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-127">The folder items are moved to when they are deleted.</span></span> |
| <span data-ttu-id="bc5a4-128">下書き</span><span class="sxs-lookup"><span data-stu-id="bc5a4-128">drafts</span></span> | <span data-ttu-id="bc5a4-129">未送信のメッセージを格納するフォルダー。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-129">The folder that contains unsent messages.</span></span> |
| <span data-ttu-id="bc5a4-130">[受信トレイ]</span><span class="sxs-lookup"><span data-stu-id="bc5a4-130">inbox</span></span> | <span data-ttu-id="bc5a4-131">[受信トレイ] フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-131">The inbox folder.</span></span> |
| <span data-ttu-id="bc5a4-132">junkemail</span><span class="sxs-lookup"><span data-stu-id="bc5a4-132">junkemail</span></span> | <span data-ttu-id="bc5a4-133">迷惑メールのフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-133">The junk email folder.</span></span> |
| <span data-ttu-id="bc5a4-134">localfailures</span><span class="sxs-lookup"><span data-stu-id="bc5a4-134">localfailures</span></span> | <span data-ttu-id="bc5a4-135">ローカル クライアント上に存在するが、サーバーにアップロードできませんでしたアイテムを含むフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-135">The folder that contains items that exist on the local client but could not be uploaded to the server.</span></span> |
| <span data-ttu-id="bc5a4-136">msgfolderroot</span><span class="sxs-lookup"><span data-stu-id="bc5a4-136">msgfolderroot</span></span> | <span data-ttu-id="bc5a4-137">「インフォメーション ストアの最上位」のフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-137">The "Top of Information Store" folder.</span></span> <span data-ttu-id="bc5a4-138">このフォルダーは、受信トレイなど、通常のメール クライアントで表示されているフォルダーの親フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-138">This folder is the parent folder for folders that are displayed in normal mail clients, such as the inbox.</span></span> |
| <span data-ttu-id="bc5a4-139">[送信トレイ] します。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-139">outbox</span></span> | <span data-ttu-id="bc5a4-140">[送信トレイ] フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-140">The outbox folder.</span></span> |
| <span data-ttu-id="bc5a4-141">recoverableitemsdeletions</span><span class="sxs-lookup"><span data-stu-id="bc5a4-141">recoverableitemsdeletions</span></span> | <span data-ttu-id="bc5a4-142">ソフト削除済みアイテムを含むフォルダー: 削除済みアイテム フォルダーから、または shift キーを押して削除 + では、Outlook を削除します。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-142">The folder that contains soft-deleted items: deleted either from the Deleted Items folder, or by pressing shift+delete in Outlook.</span></span> <span data-ttu-id="bc5a4-143">このフォルダーが、Outlook 電子メール クライアントに表示されないが、エンド ・ ユーザーを操作できます Outlook または Outlook web 上で**サーバーから削除済みアイテムの回復**機能を使用します。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-143">This folder is not visible in any Outlook email client, but end users can interact with it through the **Recover Deleted Items from Server** feature in Outlook or Outlook on the web.</span></span> |
| <span data-ttu-id="bc5a4-144">スケジュール済み</span><span class="sxs-lookup"><span data-stu-id="bc5a4-144">scheduled</span></span> | <span data-ttu-id="bc5a4-145">IOS は、Outlook のスケジュール機能を使用して受信トレイに表示されるようにスケジュールされているメッセージを含むフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-145">The folder that contains messages that are scheduled to reappear in the inbox using the Schedule feature in Outlook for iOS.</span></span> |
| <span data-ttu-id="bc5a4-146">使用して</span><span class="sxs-lookup"><span data-stu-id="bc5a4-146">searchfolders</span></span> | <span data-ttu-id="bc5a4-147">ユーザーのメールボックスで定義されているすべての検索フォルダーの親フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-147">The parent folder for all search folders defined in the user's mailbox.</span></span> |
| <span data-ttu-id="bc5a4-148">送信済みアイテム</span><span class="sxs-lookup"><span data-stu-id="bc5a4-148">sentitems</span></span> | <span data-ttu-id="bc5a4-149">送信済みアイテム フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-149">The sent items folder.</span></span> |
| <span data-ttu-id="bc5a4-150">serverfailures</span><span class="sxs-lookup"><span data-stu-id="bc5a4-150">serverfailures</span></span> | <span data-ttu-id="bc5a4-151">サーバー上に存在するが、ローカル クライアントを同期できませんでしたアイテムを含むフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-151">The folder that contains items that exist on the server but could not be synchronized to the local client.</span></span> |
| <span data-ttu-id="bc5a4-152">syncissues</span><span class="sxs-lookup"><span data-stu-id="bc5a4-152">syncissues</span></span> | <span data-ttu-id="bc5a4-153">Outlook で作成された同期ログを格納するフォルダー。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-153">The folder that contains synchronization logs created by Outlook.</span></span> |

## <a name="methods"></a><span data-ttu-id="bc5a4-154">メソッド</span><span class="sxs-lookup"><span data-stu-id="bc5a4-154">Methods</span></span>

| <span data-ttu-id="bc5a4-155">メソッド</span><span class="sxs-lookup"><span data-stu-id="bc5a4-155">Method</span></span> | <span data-ttu-id="bc5a4-156">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bc5a4-156">Return Type</span></span> | <span data-ttu-id="bc5a4-157">説明</span><span class="sxs-lookup"><span data-stu-id="bc5a4-157">Description</span></span> |
|:-------|:------------|:------------|
|[<span data-ttu-id="bc5a4-158">mailFolder の取得</span><span class="sxs-lookup"><span data-stu-id="bc5a4-158">Get mailFolder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="bc5a4-159">mailFolder</span><span class="sxs-lookup"><span data-stu-id="bc5a4-159">mailFolder</span></span>](mailfolder.md) |<span data-ttu-id="bc5a4-160">mailFolder オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-160">Read properties and relationships of mailFolder object.</span></span>|
|[<span data-ttu-id="bc5a4-161">MailFolder の作成</span><span class="sxs-lookup"><span data-stu-id="bc5a4-161">Create MailFolder</span></span>](../api/mailfolder-post-childfolders.md) |[<span data-ttu-id="bc5a4-162">mailFolder</span><span class="sxs-lookup"><span data-stu-id="bc5a4-162">mailFolder</span></span>](mailfolder.md)| <span data-ttu-id="bc5a4-163">childFolders コレクションへの投稿により、現在の mailFolder 下に新しい mailFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-163">Create a new mailFolder under the current one by posting to the childFolders collection.</span></span>|
|[<span data-ttu-id="bc5a4-164">childFolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="bc5a4-164">List childFolders</span></span>](../api/mailfolder-list-childfolders.md) |<span data-ttu-id="bc5a4-165">[mailFolder](mailfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bc5a4-165">[mailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="bc5a4-p108">指定したフォルダーの下のフォルダー コレクションを取得します。`.../me/MailFolders` ショートカットを使用すると、最上位フォルダーのコレクションを取得して、別のフォルダーに移動することができます。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-p108">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>|
|[<span data-ttu-id="bc5a4-168">メッセージの作成</span><span class="sxs-lookup"><span data-stu-id="bc5a4-168">Create Message</span></span>](../api/mailfolder-post-messages.md) |[<span data-ttu-id="bc5a4-169">message</span><span class="sxs-lookup"><span data-stu-id="bc5a4-169">message</span></span>](message.md)| <span data-ttu-id="bc5a4-170">メッセージ コレクションへの投稿により、現在の mailFolder に新しいメッセージを作成します。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-170">Create a new message in the current mailFolder by posting to the messages collection.</span></span>|
|[<span data-ttu-id="bc5a4-171">List messages</span><span class="sxs-lookup"><span data-stu-id="bc5a4-171">List messages</span></span>](../api/mailfolder-list-messages.md) |<span data-ttu-id="bc5a4-172">[message](message.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bc5a4-172">[message](message.md) collection</span></span>| <span data-ttu-id="bc5a4-173">サインインしているユーザーのメールボックス内のすべてのメッセージや、メールボックス内の指定したフォルダー内のメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-173">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>|
|[<span data-ttu-id="bc5a4-174">更新する</span><span class="sxs-lookup"><span data-stu-id="bc5a4-174">Update</span></span>](../api/mailfolder-update.md) | [<span data-ttu-id="bc5a4-175">mailFolder</span><span class="sxs-lookup"><span data-stu-id="bc5a4-175">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="bc5a4-176">指定した mailFolder オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-176">Update the specified mailFolder object.</span></span> |
|[<span data-ttu-id="bc5a4-177">削除</span><span class="sxs-lookup"><span data-stu-id="bc5a4-177">Delete</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="bc5a4-178">なし</span><span class="sxs-lookup"><span data-stu-id="bc5a4-178">None</span></span> |<span data-ttu-id="bc5a4-179">指定した mailFolder オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-179">Delete the specified mailFolder object.</span></span> |
|[<span data-ttu-id="bc5a4-180">コピー</span><span class="sxs-lookup"><span data-stu-id="bc5a4-180">copy</span></span>](../api/mailfolder-copy.md)|[<span data-ttu-id="bc5a4-181">mailFolder</span><span class="sxs-lookup"><span data-stu-id="bc5a4-181">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="bc5a4-182">mailFolder とその内容を別の mailFolder にコピーします。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-182">Copy a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="bc5a4-183">delta</span><span class="sxs-lookup"><span data-stu-id="bc5a4-183">delta</span></span>](../api/mailfolder-delta.md)|<span data-ttu-id="bc5a4-184">[mailFolder](mailfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bc5a4-184">[mailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="bc5a4-185">ユーザーのメールボックスで追加または削除された一連のメール フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-185">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="bc5a4-186">move</span><span class="sxs-lookup"><span data-stu-id="bc5a4-186">move</span></span>](../api/mailfolder-move.md)|[<span data-ttu-id="bc5a4-187">mailFolder</span><span class="sxs-lookup"><span data-stu-id="bc5a4-187">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="bc5a4-188">mailFolder とその内容を別の mailFolder に移動します。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-188">Move a mailFolder and its contents to another mailFolder.</span></span>|
|<span data-ttu-id="bc5a4-189">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="bc5a4-189">**Extended properties**</span></span>| | |
|[<span data-ttu-id="bc5a4-190">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="bc5a4-190">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="bc5a4-191">mailFolder</span><span class="sxs-lookup"><span data-stu-id="bc5a4-191">mailFolder</span></span>](mailfolder.md)  |<span data-ttu-id="bc5a4-192">新規または既存の mailFolder に、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-192">Create one or more single-value extended properties in a new or existing mailFolder.</span></span>   |
|[<span data-ttu-id="bc5a4-193">単一値の拡張プロパティを持つ mailFolder の取得</span><span class="sxs-lookup"><span data-stu-id="bc5a4-193">Get mailFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="bc5a4-194">mailFolder</span><span class="sxs-lookup"><span data-stu-id="bc5a4-194">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="bc5a4-195">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含む mailFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-195">Get mailFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="bc5a4-196">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="bc5a4-196">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="bc5a4-197">mailFolder</span><span class="sxs-lookup"><span data-stu-id="bc5a4-197">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="bc5a4-198">新規または既存の mailFolder の 1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-198">Create one or more multi-value extended properties in a new or existing mailFolder.</span></span>  |
|[<span data-ttu-id="bc5a4-199">複数値の拡張プロパティを持つ mailFolder の取得</span><span class="sxs-lookup"><span data-stu-id="bc5a4-199">Get mailFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="bc5a4-200">mailFolder</span><span class="sxs-lookup"><span data-stu-id="bc5a4-200">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="bc5a4-201">`$expand` を使用して、複数値の拡張プロパティを含む mailFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-201">Get a mailFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="bc5a4-202">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc5a4-202">Properties</span></span>

| <span data-ttu-id="bc5a4-203">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc5a4-203">Property</span></span> | <span data-ttu-id="bc5a4-204">型</span><span class="sxs-lookup"><span data-stu-id="bc5a4-204">Type</span></span> | <span data-ttu-id="bc5a4-205">説明</span><span class="sxs-lookup"><span data-stu-id="bc5a4-205">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="bc5a4-206">childFolderCount</span><span class="sxs-lookup"><span data-stu-id="bc5a4-206">childFolderCount</span></span>|<span data-ttu-id="bc5a4-207">Int32</span><span class="sxs-lookup"><span data-stu-id="bc5a4-207">Int32</span></span>|<span data-ttu-id="bc5a4-208">現在の mailFolder の直下の子 mailFolder の数。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-208">The number of immediate child mailFolders in the current mailFolder.</span></span>|
|<span data-ttu-id="bc5a4-209">displayName</span><span class="sxs-lookup"><span data-stu-id="bc5a4-209">displayName</span></span>|<span data-ttu-id="bc5a4-210">String</span><span class="sxs-lookup"><span data-stu-id="bc5a4-210">String</span></span>|<span data-ttu-id="bc5a4-211">mailFolder の表示名。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-211">The mailFolder's display name.</span></span>|
|<span data-ttu-id="bc5a4-212">id</span><span class="sxs-lookup"><span data-stu-id="bc5a4-212">id</span></span>|<span data-ttu-id="bc5a4-213">String</span><span class="sxs-lookup"><span data-stu-id="bc5a4-213">String</span></span>|<span data-ttu-id="bc5a4-214">MailFolder の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-214">The mailFolder's unique identifier.</span></span>|
|<span data-ttu-id="bc5a4-215">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="bc5a4-215">parentFolderId</span></span>|<span data-ttu-id="bc5a4-216">String</span><span class="sxs-lookup"><span data-stu-id="bc5a4-216">String</span></span>|<span data-ttu-id="bc5a4-217">mailFolder の親 mailFolder の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-217">The unique identifier for the mailFolder's parent mailFolder.</span></span>|
|<span data-ttu-id="bc5a4-218">totalItemCount</span><span class="sxs-lookup"><span data-stu-id="bc5a4-218">totalItemCount</span></span>|<span data-ttu-id="bc5a4-219">Int32</span><span class="sxs-lookup"><span data-stu-id="bc5a4-219">Int32</span></span>|<span data-ttu-id="bc5a4-220">mailFolder に含まれるアイテムの数</span><span class="sxs-lookup"><span data-stu-id="bc5a4-220">The number of items in the mailFolder.</span></span>|
|<span data-ttu-id="bc5a4-221">unreadItemCount</span><span class="sxs-lookup"><span data-stu-id="bc5a4-221">unreadItemCount</span></span>|<span data-ttu-id="bc5a4-222">Int32</span><span class="sxs-lookup"><span data-stu-id="bc5a4-222">Int32</span></span>|<span data-ttu-id="bc5a4-223">mailFolder 内で未読としてマークされているアイテムの数。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-223">The number of items in the mailFolder marked as unread.</span></span>|
|<span data-ttu-id="bc5a4-224">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="bc5a4-224">wellKnownName</span></span>|<span data-ttu-id="bc5a4-225">String</span><span class="sxs-lookup"><span data-stu-id="bc5a4-225">String</span></span>|<span data-ttu-id="bc5a4-226">フォルダーの既知のフォルダーの名前です。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-226">The well-known folder name for the folder.</span></span> <span data-ttu-id="bc5a4-227">可能な値は、上記に一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-227">The possible values are listed above.</span></span> <span data-ttu-id="bc5a4-228">Outlook で作成された既定のフォルダーには、このプロパティは設定のみです。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-228">This property is only set for default folders created by Outlook.</span></span> <span data-ttu-id="bc5a4-229">その他のフォルダーでは、このプロパティは**null**です。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-229">For other folders, this property is **null**.</span></span>|

<span data-ttu-id="bc5a4-230">**アイテム数を効率的に取得する**</span><span class="sxs-lookup"><span data-stu-id="bc5a4-230">**Access item counts efficiently**</span></span>

<span data-ttu-id="bc5a4-231">`TotalItemCount`と`UnreadItemCount`フォルダーのプロパティを使用すると、簡単にフォルダー内のアイテムの読み取りの数を計算します。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-231">The `TotalItemCount` and `UnreadItemCount` properties of a folder allow you to conveniently compute the number of read items in the folder.</span></span>
<span data-ttu-id="bc5a4-232">これにより、大幅な遅延が発生する可能性がある次のようなクエリを回避できます。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-232">They let you avoid queries like the following that can incur significant latency:</span></span>

```http
https://outlook.office.com/api/beta/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

<span data-ttu-id="bc5a4-233">Outlook のメール フォルダーにアイテムの 1 つ以上の種類を含めることができます、受信トレイを含めることができますたとえば、会議出席依頼アイテムがメール アイテムとは異なる。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-233">Mail folders in Outlook can contain more than one type of items, for example, the Inbox can contain meeting request items which are distinct from mail items.</span></span> <span data-ttu-id="bc5a4-234">`TotalItemCount``UnreadItemCount`の項目の種類に関係なく、[メール] フォルダーにアイテムが含まれます。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-234">`TotalItemCount` and `UnreadItemCount` include items in a mail folder irrespective of their item types.</span></span>

## <a name="relationships"></a><span data-ttu-id="bc5a4-235">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bc5a4-235">Relationships</span></span>

| <span data-ttu-id="bc5a4-236">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bc5a4-236">Relationship</span></span> | <span data-ttu-id="bc5a4-237">型</span><span class="sxs-lookup"><span data-stu-id="bc5a4-237">Type</span></span> | <span data-ttu-id="bc5a4-238">説明</span><span class="sxs-lookup"><span data-stu-id="bc5a4-238">Description</span></span> |
|:-------------|:-----|:------------|
|<span data-ttu-id="bc5a4-239">childFolders</span><span class="sxs-lookup"><span data-stu-id="bc5a4-239">childFolders</span></span>|<span data-ttu-id="bc5a4-240">[MailFolder](mailfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bc5a4-240">[MailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="bc5a4-241">mailFolder 内の子フォルダーのコレクション。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-241">The collection of child folders in the mailFolder.</span></span>|
|<span data-ttu-id="bc5a4-242">messageRules</span><span class="sxs-lookup"><span data-stu-id="bc5a4-242">messageRules</span></span> | <span data-ttu-id="bc5a4-243">[messageRule](messagerule.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bc5a4-243">[messageRule](messagerule.md) collection</span></span> | <span data-ttu-id="bc5a4-244">ユーザーの受信トレイ フォルダーに適用されるルールのコレクション。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-244">The collection of rules that apply to the user's Inbox folder.</span></span> |
|<span data-ttu-id="bc5a4-245">messages</span><span class="sxs-lookup"><span data-stu-id="bc5a4-245">messages</span></span>|<span data-ttu-id="bc5a4-246">[Message](message.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bc5a4-246">[Message](message.md) collection</span></span>|<span data-ttu-id="bc5a4-247">mailFolder 内のメッセージのコレクション。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-247">The collection of messages in the mailFolder.</span></span>|
|<span data-ttu-id="bc5a4-248">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="bc5a4-248">multiValueExtendedProperties</span></span>|<span data-ttu-id="bc5a4-249">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="bc5a4-249">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="bc5a4-p112">mailFolder に対して定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-p112">The collection of multi-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="bc5a4-253">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="bc5a4-253">singleValueExtendedProperties</span></span>|<span data-ttu-id="bc5a4-254">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="bc5a4-254">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="bc5a4-p113">mailFolder に対して定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-p113">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bc5a4-258">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bc5a4-258">JSON representation</span></span>

<span data-ttu-id="bc5a4-259">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bc5a4-259">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messageRules",
    "messages",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mailFolder"
}-->

```json
{
  "childFolderCount": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "totalItemCount": 1024,
  "unreadItemCount": 1024,
  "wellKnownName": "string",
  "childFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "messageRules": [ { "@odata.type": "microsoft.graph.messageRule" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}
```

## <a name="see-also"></a><span data-ttu-id="bc5a4-260">関連項目</span><span class="sxs-lookup"><span data-stu-id="bc5a4-260">See also</span></span>

- [<span data-ttu-id="bc5a4-261">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="bc5a4-261">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="bc5a4-262">フォルダー内のメッセージへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="bc5a4-262">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
