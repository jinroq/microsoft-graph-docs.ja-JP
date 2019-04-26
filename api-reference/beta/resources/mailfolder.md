---
title: mailFolder リソースの種類
description: 受信トレイや下書きなどの、ユーザーのメールボックス内のメール フォルダーです。 メール フォルダーには、メッセージ、他の Outlook アイテム、子メール フォルダーを含めることができます。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 294f2a9a6b4775ad30165352dec5520fb0efa804
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342774"
---
# <a name="mailfolder-resource-type"></a><span data-ttu-id="630e6-104">mailFolder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="630e6-104">mailFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="630e6-105">受信トレイや下書きなどの、ユーザーのメールボックス内のメール フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="630e6-105">A mail folder in a user's mailbox, such as Inbox and Drafts.</span></span> <span data-ttu-id="630e6-106">メール フォルダーには、メッセージ、他の Outlook アイテム、子メール フォルダーを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="630e6-106">Mail folders can contain messages, other Outlook items, and child mail folders.</span></span>

<span data-ttu-id="630e6-107">このリソースでは、[デルタ](../api/mailfolder-delta.md)関数を用意すれば、増分の追加、削除、更新に[デルタ クエリ](/graph/delta-query-overview)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="630e6-107">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/mailfolder-delta.md) function.</span></span>

<span data-ttu-id="630e6-108">**既知のフォルダー名**</span><span class="sxs-lookup"><span data-stu-id="630e6-108">**Well-known folder names**</span></span>

<span data-ttu-id="630e6-109">Outlook では、既定でユーザー用の特定のフォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="630e6-109">Outlook creates certain folders for users by default.</span></span> <span data-ttu-id="630e6-110">このようなフォルダーにアクセスする場合は、対応するフォルダー **id**値を使用する代わりに、以下の表にある、既知のフォルダー名を使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="630e6-110">Instead of using the corresponding folder **id** value, for convenience, you can use the well-known folder names from the table below when accessing these folders.</span></span> <span data-ttu-id="630e6-111">たとえば、次のクエリを使用して、既知の名前を使用して [下書き] フォルダーを取得できます。</span><span class="sxs-lookup"><span data-stu-id="630e6-111">For example, you can get the Drafts folder using its well-known name with the following query.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

<span data-ttu-id="630e6-112">既知の名前は、ユーザーのメールボックスのロケールに関係なく動作するので、上記のクエリは、名前の指定に関係なく、常にユーザーの [下書き] フォルダーを返します。</span><span class="sxs-lookup"><span data-stu-id="630e6-112">Well-known names work regardless of the locale of the user's mailbox, so the above query will always return the user's Drafts folder regardless of how it is named.</span></span>

| <span data-ttu-id="630e6-113">既知のフォルダー名</span><span class="sxs-lookup"><span data-stu-id="630e6-113">Well-known folder name</span></span> | <span data-ttu-id="630e6-114">説明</span><span class="sxs-lookup"><span data-stu-id="630e6-114">Description</span></span> |
|:-----------------------|:------------|
| <span data-ttu-id="630e6-115">・</span><span class="sxs-lookup"><span data-stu-id="630e6-115">archive</span></span> | <span data-ttu-id="630e6-116">アーカイブフォルダーのメッセージは、それをサポートする Outlook クライアントで One_Click アーカイブ機能を使用するときに送信されます。</span><span class="sxs-lookup"><span data-stu-id="630e6-116">The archive folder messages are sent to when using the One_Click Archive feature in Outlook clients that support it.</span></span> <span data-ttu-id="630e6-117">**注:** これは、Exchange online のアーカイブメールボックス機能と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="630e6-117">**Note:** this is not the same as the Archive Mailbox feature of Exchange online.</span></span> |
| <span data-ttu-id="630e6-118">整頓</span><span class="sxs-lookup"><span data-stu-id="630e6-118">clutter</span></span> | <span data-ttu-id="630e6-119">低優先メール機能フォルダー低優先度のメッセージは、低優先メール機能を使用している場合に移動されます。</span><span class="sxs-lookup"><span data-stu-id="630e6-119">The clutter folder low-priority messages are moved to when using the Clutter feature.</span></span> |
| <span data-ttu-id="630e6-120">解消</span><span class="sxs-lookup"><span data-stu-id="630e6-120">conflicts</span></span> | <span data-ttu-id="630e6-121">メールボックス内の競合するアイテムを含むフォルダー。</span><span class="sxs-lookup"><span data-stu-id="630e6-121">The folder that contains conflicting items in the mailbox.</span></span> |
| <span data-ttu-id="630e6-122">conversationhistory</span><span class="sxs-lookup"><span data-stu-id="630e6-122">conversationhistory</span></span> | <span data-ttu-id="630e6-123">skype が IM 会話を保存するフォルダー (skype が設定されている場合)。</span><span class="sxs-lookup"><span data-stu-id="630e6-123">The folder where Skype saves IM conversations (if Skype is configured to do so).</span></span> |
| <span data-ttu-id="630e6-124">deleteditems</span><span class="sxs-lookup"><span data-stu-id="630e6-124">deleteditems</span></span> | <span data-ttu-id="630e6-125">フォルダーアイテムは、削除されたときに移動されます。</span><span class="sxs-lookup"><span data-stu-id="630e6-125">The folder items are moved to when they are deleted.</span></span> |
| <span data-ttu-id="630e6-126">未公開</span><span class="sxs-lookup"><span data-stu-id="630e6-126">drafts</span></span> | <span data-ttu-id="630e6-127">未送信メッセージを含むフォルダー。</span><span class="sxs-lookup"><span data-stu-id="630e6-127">The folder that contains unsent messages.</span></span> |
| <span data-ttu-id="630e6-128">ボックス</span><span class="sxs-lookup"><span data-stu-id="630e6-128">inbox</span></span> | <span data-ttu-id="630e6-129">受信トレイフォルダー。</span><span class="sxs-lookup"><span data-stu-id="630e6-129">The inbox folder.</span></span> |
| <span data-ttu-id="630e6-130">junkemail</span><span class="sxs-lookup"><span data-stu-id="630e6-130">junkemail</span></span> | <span data-ttu-id="630e6-131">迷惑メールフォルダー。</span><span class="sxs-lookup"><span data-stu-id="630e6-131">The junk email folder.</span></span> |
| <span data-ttu-id="630e6-132">localfailures</span><span class="sxs-lookup"><span data-stu-id="630e6-132">localfailures</span></span> | <span data-ttu-id="630e6-133">ローカルクライアント上に存在するが、サーバーにアップロードできないアイテムを含むフォルダー。</span><span class="sxs-lookup"><span data-stu-id="630e6-133">The folder that contains items that exist on the local client but could not be uploaded to the server.</span></span> |
| <span data-ttu-id="630e6-134">msgfolderroot</span><span class="sxs-lookup"><span data-stu-id="630e6-134">msgfolderroot</span></span> | <span data-ttu-id="630e6-135">"インフォメーションストアのトップ" フォルダー</span><span class="sxs-lookup"><span data-stu-id="630e6-135">The "Top of Information Store" folder.</span></span> <span data-ttu-id="630e6-136">このフォルダーは、受信トレイなど、通常のメールクライアントに表示されるフォルダーの親フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="630e6-136">This folder is the parent folder for folders that are displayed in normal mail clients, such as the inbox.</span></span> |
| <span data-ttu-id="630e6-137">送信トレイ</span><span class="sxs-lookup"><span data-stu-id="630e6-137">outbox</span></span> | <span data-ttu-id="630e6-138">送信トレイフォルダー。</span><span class="sxs-lookup"><span data-stu-id="630e6-138">The outbox folder.</span></span> |
| <span data-ttu-id="630e6-139">recoverableitemsdeletions</span><span class="sxs-lookup"><span data-stu-id="630e6-139">recoverableitemsdeletions</span></span> | <span data-ttu-id="630e6-140">削除済みアイテムフォルダーから削除された、または Outlook で shift + del キーを押して削除されたアイテムを含むフォルダー。</span><span class="sxs-lookup"><span data-stu-id="630e6-140">The folder that contains soft-deleted items: deleted either from the Deleted Items folder, or by pressing shift+delete in Outlook.</span></span> <span data-ttu-id="630e6-141">このフォルダーは、outlook 電子メールクライアントでは表示されませんが、エンドユーザーは、outlook または web 上の outlook の [**サーバーからの削除済みアイテムを復元**する] 機能を使用して操作できます。</span><span class="sxs-lookup"><span data-stu-id="630e6-141">This folder is not visible in any Outlook email client, but end users can interact with it through the **Recover Deleted Items from Server** feature in Outlook or Outlook on the web.</span></span> |
| <span data-ttu-id="630e6-142">スケジュール済み</span><span class="sxs-lookup"><span data-stu-id="630e6-142">scheduled</span></span> | <span data-ttu-id="630e6-143">iOS 版 Outlook のスケジュール機能を使用して、受信トレイに再表示するようにスケジュールされたメッセージを含むフォルダー。</span><span class="sxs-lookup"><span data-stu-id="630e6-143">The folder that contains messages that are scheduled to reappear in the inbox using the Schedule feature in Outlook for iOS.</span></span> |
| <span data-ttu-id="630e6-144">searchfolders</span><span class="sxs-lookup"><span data-stu-id="630e6-144">searchfolders</span></span> | <span data-ttu-id="630e6-145">ユーザーのメールボックスに定義されているすべての検索フォルダーの親フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="630e6-145">The parent folder for all search folders defined in the user's mailbox.</span></span> |
| <span data-ttu-id="630e6-146">sentitems</span><span class="sxs-lookup"><span data-stu-id="630e6-146">sentitems</span></span> | <span data-ttu-id="630e6-147">送信済みアイテムフォルダー。</span><span class="sxs-lookup"><span data-stu-id="630e6-147">The sent items folder.</span></span> |
| <span data-ttu-id="630e6-148">serverfailures</span><span class="sxs-lookup"><span data-stu-id="630e6-148">serverfailures</span></span> | <span data-ttu-id="630e6-149">サーバー上に存在するが、ローカルクライアントに同期できなかったアイテムを含むフォルダー。</span><span class="sxs-lookup"><span data-stu-id="630e6-149">The folder that contains items that exist on the server but could not be synchronized to the local client.</span></span> |
| <span data-ttu-id="630e6-150">syncissues 問題</span><span class="sxs-lookup"><span data-stu-id="630e6-150">syncissues</span></span> | <span data-ttu-id="630e6-151">Outlook によって作成された同期ログが格納されているフォルダー。</span><span class="sxs-lookup"><span data-stu-id="630e6-151">The folder that contains synchronization logs created by Outlook.</span></span> |

## <a name="methods"></a><span data-ttu-id="630e6-152">メソッド</span><span class="sxs-lookup"><span data-stu-id="630e6-152">Methods</span></span>

| <span data-ttu-id="630e6-153">メソッド</span><span class="sxs-lookup"><span data-stu-id="630e6-153">Method</span></span> | <span data-ttu-id="630e6-154">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="630e6-154">Return Type</span></span> | <span data-ttu-id="630e6-155">説明</span><span class="sxs-lookup"><span data-stu-id="630e6-155">Description</span></span> |
|:-------|:------------|:------------|
|[<span data-ttu-id="630e6-156">mailFolder の取得</span><span class="sxs-lookup"><span data-stu-id="630e6-156">Get mailFolder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="630e6-157">mailFolder</span><span class="sxs-lookup"><span data-stu-id="630e6-157">mailFolder</span></span>](mailfolder.md) |<span data-ttu-id="630e6-158">mailFolder オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="630e6-158">Read properties and relationships of mailFolder object.</span></span>|
|[<span data-ttu-id="630e6-159">MailFolder の作成</span><span class="sxs-lookup"><span data-stu-id="630e6-159">Create MailFolder</span></span>](../api/mailfolder-post-childfolders.md) |[<span data-ttu-id="630e6-160">mailFolder</span><span class="sxs-lookup"><span data-stu-id="630e6-160">mailFolder</span></span>](mailfolder.md)| <span data-ttu-id="630e6-161">childFolders コレクションへの投稿により、現在の mailFolder 下に新しい mailFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="630e6-161">Create a new mailFolder under the current one by posting to the childFolders collection.</span></span>|
|[<span data-ttu-id="630e6-162">childFolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="630e6-162">List childFolders</span></span>](../api/mailfolder-list-childfolders.md) |<span data-ttu-id="630e6-163">[mailFolder](mailfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="630e6-163">[mailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="630e6-p107">指定したフォルダーの下のフォルダー コレクションを取得します。`.../me/MailFolders` ショートカットを使用すると、最上位フォルダーのコレクションを取得して、別のフォルダーに移動することができます。</span><span class="sxs-lookup"><span data-stu-id="630e6-p107">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>|
|[<span data-ttu-id="630e6-166">メッセージの作成</span><span class="sxs-lookup"><span data-stu-id="630e6-166">Create Message</span></span>](../api/mailfolder-post-messages.md) |[<span data-ttu-id="630e6-167">message</span><span class="sxs-lookup"><span data-stu-id="630e6-167">message</span></span>](message.md)| <span data-ttu-id="630e6-168">メッセージ コレクションへの投稿により、現在の mailFolder に新しいメッセージを作成します。</span><span class="sxs-lookup"><span data-stu-id="630e6-168">Create a new message in the current mailFolder by posting to the messages collection.</span></span>|
|[<span data-ttu-id="630e6-169">List messages</span><span class="sxs-lookup"><span data-stu-id="630e6-169">List messages</span></span>](../api/mailfolder-list-messages.md) |<span data-ttu-id="630e6-170">[message](message.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="630e6-170">[message](message.md) collection</span></span>| <span data-ttu-id="630e6-171">サインインしているユーザーのメールボックス内のすべてのメッセージや、メールボックス内の指定したフォルダー内のメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="630e6-171">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>|
|[<span data-ttu-id="630e6-172">更新する</span><span class="sxs-lookup"><span data-stu-id="630e6-172">Update</span></span>](../api/mailfolder-update.md) | [<span data-ttu-id="630e6-173">mailFolder</span><span class="sxs-lookup"><span data-stu-id="630e6-173">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="630e6-174">指定した mailFolder オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="630e6-174">Update the specified mailFolder object.</span></span> |
|[<span data-ttu-id="630e6-175">削除</span><span class="sxs-lookup"><span data-stu-id="630e6-175">Delete</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="630e6-176">なし</span><span class="sxs-lookup"><span data-stu-id="630e6-176">None</span></span> |<span data-ttu-id="630e6-177">指定した mailFolder オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="630e6-177">Delete the specified mailFolder object.</span></span> |
|[<span data-ttu-id="630e6-178">コピー</span><span class="sxs-lookup"><span data-stu-id="630e6-178">copy</span></span>](../api/mailfolder-copy.md)|[<span data-ttu-id="630e6-179">mailFolder</span><span class="sxs-lookup"><span data-stu-id="630e6-179">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="630e6-180">mailFolder とその内容を別の mailFolder にコピーします。</span><span class="sxs-lookup"><span data-stu-id="630e6-180">Copy a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="630e6-181">delta</span><span class="sxs-lookup"><span data-stu-id="630e6-181">delta</span></span>](../api/mailfolder-delta.md)|<span data-ttu-id="630e6-182">[mailFolder](mailfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="630e6-182">[mailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="630e6-183">ユーザーのメールボックスで追加または削除された一連のメール フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="630e6-183">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="630e6-184">move</span><span class="sxs-lookup"><span data-stu-id="630e6-184">move</span></span>](../api/mailfolder-move.md)|[<span data-ttu-id="630e6-185">mailFolder</span><span class="sxs-lookup"><span data-stu-id="630e6-185">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="630e6-186">mailFolder とその内容を別の mailFolder に移動します。</span><span class="sxs-lookup"><span data-stu-id="630e6-186">Move a mailFolder and its contents to another mailFolder.</span></span>|
|<span data-ttu-id="630e6-187">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="630e6-187">**Extended properties**</span></span>| | |
|[<span data-ttu-id="630e6-188">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="630e6-188">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="630e6-189">mailFolder</span><span class="sxs-lookup"><span data-stu-id="630e6-189">mailFolder</span></span>](mailfolder.md)  |<span data-ttu-id="630e6-190">新規または既存の mailFolder に、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="630e6-190">Create one or more single-value extended properties in a new or existing mailFolder.</span></span>   |
|[<span data-ttu-id="630e6-191">単一値の拡張プロパティを持つ mailFolder の取得</span><span class="sxs-lookup"><span data-stu-id="630e6-191">Get mailFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="630e6-192">mailFolder</span><span class="sxs-lookup"><span data-stu-id="630e6-192">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="630e6-193">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含む mailFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="630e6-193">Get mailFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="630e6-194">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="630e6-194">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="630e6-195">mailFolder</span><span class="sxs-lookup"><span data-stu-id="630e6-195">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="630e6-196">新規または既存の mailFolder の 1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="630e6-196">Create one or more multi-value extended properties in a new or existing mailFolder.</span></span>  |
|[<span data-ttu-id="630e6-197">複数値の拡張プロパティを持つ mailFolder の取得</span><span class="sxs-lookup"><span data-stu-id="630e6-197">Get mailFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="630e6-198">mailFolder</span><span class="sxs-lookup"><span data-stu-id="630e6-198">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="630e6-199">`$expand` を使用して、複数値の拡張プロパティを含む mailFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="630e6-199">Get a mailFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="630e6-200">プロパティ</span><span class="sxs-lookup"><span data-stu-id="630e6-200">Properties</span></span>

| <span data-ttu-id="630e6-201">プロパティ</span><span class="sxs-lookup"><span data-stu-id="630e6-201">Property</span></span> | <span data-ttu-id="630e6-202">型</span><span class="sxs-lookup"><span data-stu-id="630e6-202">Type</span></span> | <span data-ttu-id="630e6-203">説明</span><span class="sxs-lookup"><span data-stu-id="630e6-203">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="630e6-204">childFolderCount</span><span class="sxs-lookup"><span data-stu-id="630e6-204">childFolderCount</span></span>|<span data-ttu-id="630e6-205">Int32</span><span class="sxs-lookup"><span data-stu-id="630e6-205">Int32</span></span>|<span data-ttu-id="630e6-206">現在の mailFolder の直下の子 mailFolder の数。</span><span class="sxs-lookup"><span data-stu-id="630e6-206">The number of immediate child mailFolders in the current mailFolder.</span></span>|
|<span data-ttu-id="630e6-207">displayName</span><span class="sxs-lookup"><span data-stu-id="630e6-207">displayName</span></span>|<span data-ttu-id="630e6-208">文字列</span><span class="sxs-lookup"><span data-stu-id="630e6-208">String</span></span>|<span data-ttu-id="630e6-209">mailFolder の表示名。</span><span class="sxs-lookup"><span data-stu-id="630e6-209">The mailFolder's display name.</span></span>|
|<span data-ttu-id="630e6-210">id</span><span class="sxs-lookup"><span data-stu-id="630e6-210">id</span></span>|<span data-ttu-id="630e6-211">String</span><span class="sxs-lookup"><span data-stu-id="630e6-211">String</span></span>|<span data-ttu-id="630e6-212">mailfolder の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="630e6-212">The mailFolder's unique identifier.</span></span>|
|<span data-ttu-id="630e6-213">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="630e6-213">parentFolderId</span></span>|<span data-ttu-id="630e6-214">String</span><span class="sxs-lookup"><span data-stu-id="630e6-214">String</span></span>|<span data-ttu-id="630e6-215">mailFolder の親 mailFolder の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="630e6-215">The unique identifier for the mailFolder's parent mailFolder.</span></span>|
|<span data-ttu-id="630e6-216">totalItemCount</span><span class="sxs-lookup"><span data-stu-id="630e6-216">totalItemCount</span></span>|<span data-ttu-id="630e6-217">Int32</span><span class="sxs-lookup"><span data-stu-id="630e6-217">Int32</span></span>|<span data-ttu-id="630e6-218">mailFolder に含まれるアイテムの数</span><span class="sxs-lookup"><span data-stu-id="630e6-218">The number of items in the mailFolder.</span></span>|
|<span data-ttu-id="630e6-219">unreadItemCount</span><span class="sxs-lookup"><span data-stu-id="630e6-219">unreadItemCount</span></span>|<span data-ttu-id="630e6-220">Int32</span><span class="sxs-lookup"><span data-stu-id="630e6-220">Int32</span></span>|<span data-ttu-id="630e6-221">mailFolder 内で未読としてマークされているアイテムの数。</span><span class="sxs-lookup"><span data-stu-id="630e6-221">The number of items in the mailFolder marked as unread.</span></span>|
|<span data-ttu-id="630e6-222">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="630e6-222">wellKnownName</span></span>|<span data-ttu-id="630e6-223">String</span><span class="sxs-lookup"><span data-stu-id="630e6-223">String</span></span>|<span data-ttu-id="630e6-224">フォルダーの既知のフォルダー名。</span><span class="sxs-lookup"><span data-stu-id="630e6-224">The well-known folder name for the folder.</span></span> <span data-ttu-id="630e6-225">指定できる値は、上記のとおりです。</span><span class="sxs-lookup"><span data-stu-id="630e6-225">The possible values are listed above.</span></span> <span data-ttu-id="630e6-226">このプロパティは、Outlook によって作成された既定のフォルダーに対してのみ設定されます。</span><span class="sxs-lookup"><span data-stu-id="630e6-226">This property is only set for default folders created by Outlook.</span></span> <span data-ttu-id="630e6-227">その他のフォルダーの場合、このプロパティは**null**になります。</span><span class="sxs-lookup"><span data-stu-id="630e6-227">For other folders, this property is **null**.</span></span>|

<span data-ttu-id="630e6-228">**アイテム数の効率的な取得**</span><span class="sxs-lookup"><span data-stu-id="630e6-228">**Access item counts efficiently**</span></span>

<span data-ttu-id="630e6-229">フォルダー `TotalItemCount`の`UnreadItemCount`プロパティとプロパティを使用すると、フォルダー内の閲覧アイテムの数を簡単に計算できます。</span><span class="sxs-lookup"><span data-stu-id="630e6-229">The `TotalItemCount` and `UnreadItemCount` properties of a folder allow you to conveniently compute the number of read items in the folder.</span></span>
<span data-ttu-id="630e6-230">これにより、大幅な遅延が発生する可能性がある次のようなクエリを回避できます。</span><span class="sxs-lookup"><span data-stu-id="630e6-230">They let you avoid queries like the following that can incur significant latency:</span></span>

```http
https://outlook.office.com/api/beta/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

<span data-ttu-id="630e6-231">Outlook のメールフォルダーには、複数の種類のアイテムを含めることができます。たとえば、受信トレイには、メールアイテムとは異なる会議出席依頼アイテムを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="630e6-231">Mail folders in Outlook can contain more than one type of items, for example, the Inbox can contain meeting request items which are distinct from mail items.</span></span> <span data-ttu-id="630e6-232">`TotalItemCount`アイテム`UnreadItemCount`の種類に関係なく、メールフォルダーにアイテムを追加します。</span><span class="sxs-lookup"><span data-stu-id="630e6-232">`TotalItemCount` and `UnreadItemCount` include items in a mail folder irrespective of their item types.</span></span>

## <a name="relationships"></a><span data-ttu-id="630e6-233">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="630e6-233">Relationships</span></span>

| <span data-ttu-id="630e6-234">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="630e6-234">Relationship</span></span> | <span data-ttu-id="630e6-235">型</span><span class="sxs-lookup"><span data-stu-id="630e6-235">Type</span></span> | <span data-ttu-id="630e6-236">説明</span><span class="sxs-lookup"><span data-stu-id="630e6-236">Description</span></span> |
|:-------------|:-----|:------------|
|<span data-ttu-id="630e6-237">childFolders</span><span class="sxs-lookup"><span data-stu-id="630e6-237">childFolders</span></span>|<span data-ttu-id="630e6-238">[MailFolder](mailfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="630e6-238">[MailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="630e6-239">mailFolder 内の子フォルダーのコレクション。</span><span class="sxs-lookup"><span data-stu-id="630e6-239">The collection of child folders in the mailFolder.</span></span>|
|<span data-ttu-id="630e6-240">messageRules</span><span class="sxs-lookup"><span data-stu-id="630e6-240">messageRules</span></span> | <span data-ttu-id="630e6-241">[messageRule](messagerule.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="630e6-241">[messageRule](messagerule.md) collection</span></span> | <span data-ttu-id="630e6-242">ユーザーの受信トレイ フォルダーに適用されるルールのコレクション。</span><span class="sxs-lookup"><span data-stu-id="630e6-242">The collection of rules that apply to the user's Inbox folder.</span></span> |
|<span data-ttu-id="630e6-243">messages</span><span class="sxs-lookup"><span data-stu-id="630e6-243">messages</span></span>|<span data-ttu-id="630e6-244">[Message](message.md) collection</span><span class="sxs-lookup"><span data-stu-id="630e6-244">[Message](message.md) collection</span></span>|<span data-ttu-id="630e6-245">mailFolder 内のメッセージのコレクション。</span><span class="sxs-lookup"><span data-stu-id="630e6-245">The collection of messages in the mailFolder.</span></span>|
|<span data-ttu-id="630e6-246">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="630e6-246">multiValueExtendedProperties</span></span>|<span data-ttu-id="630e6-247">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="630e6-247">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="630e6-p111">mailFolder に対して定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="630e6-p111">The collection of multi-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="630e6-251">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="630e6-251">singleValueExtendedProperties</span></span>|<span data-ttu-id="630e6-252">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="630e6-252">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="630e6-p112">mailFolder に対して定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="630e6-p112">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="630e6-256">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="630e6-256">JSON representation</span></span>

<span data-ttu-id="630e6-257">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="630e6-257">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="630e6-258">関連項目</span><span class="sxs-lookup"><span data-stu-id="630e6-258">See also</span></span>

- [<span data-ttu-id="630e6-259">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="630e6-259">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="630e6-260">フォルダー内のメッセージへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="630e6-260">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
