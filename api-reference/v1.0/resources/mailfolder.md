---
title: mailFolder リソースの種類
description: 受信トレイや下書きなどの、ユーザーのメールボックス内のメール フォルダーです。 メール フォルダーには、メッセージ、他の Outlook アイテム、子メール フォルダーを含めることができます。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 7e829929df46208ee321f56ae2d9f0144c320d4a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036331"
---
# <a name="mailfolder-resource-type"></a><span data-ttu-id="138c1-104">mailFolder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="138c1-104">mailFolder resource type</span></span>

<span data-ttu-id="138c1-105">受信トレイや下書きなどの、ユーザーのメールボックス内のメール フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="138c1-105">A mail folder in a user's mailbox, such as Inbox and Drafts.</span></span> <span data-ttu-id="138c1-106">メール フォルダーには、メッセージ、他の Outlook アイテム、子メール フォルダーを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="138c1-106">Mail folders can contain messages, other Outlook items, and child mail folders.</span></span>

<span data-ttu-id="138c1-107">このリソースは、[デルタ](../api/mailfolder-delta.md)関数を提供することによって、増分の追加、削除、および更新を追跡するための[デルタ クエリ](/graph/delta-query-overview)の使用をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="138c1-107">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/mailfolder-delta.md) function.</span></span>

<span data-ttu-id="138c1-108">**既知のフォルダー名**</span><span class="sxs-lookup"><span data-stu-id="138c1-108">**Well-known folder names**</span></span>

<span data-ttu-id="138c1-109">Outlookは、デフォルトでユーザー用の特定のフォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="138c1-109">Outlook creates certain folders for users by default.</span></span> <span data-ttu-id="138c1-110">対応するフォルダ**id**値を使用する代わりに、便宜上、これらのフォルダにアクセスするときに、下の表にある既知のフォルダ名を使用できます。</span><span class="sxs-lookup"><span data-stu-id="138c1-110">Instead of using the corresponding folder **id** value, for convenience, you can use the well-known folder names from the table below when accessing these folders.</span></span> <span data-ttu-id="138c1-111">たとえば、次のクエリで、よく知られている名前を使用して[下書き]フォルダを取得できます。</span><span class="sxs-lookup"><span data-stu-id="138c1-111">For example, you can get the Drafts folder using its well-known name with the following query.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

<span data-ttu-id="138c1-112">既知の名前はユーザーのメールボックスのロケールに関係なく機能するため、上記のクエリでは名前の付け方にかかわらず常にユーザーの[下書き]フォルダーが返されます。</span><span class="sxs-lookup"><span data-stu-id="138c1-112">Well-known names work regardless of the locale of the user's mailbox, so the above query will always return the user's Drafts folder regardless of how it is named.</span></span>

| <span data-ttu-id="138c1-113">既知のフォルダー名</span><span class="sxs-lookup"><span data-stu-id="138c1-113">Well-known folder name</span></span> | <span data-ttu-id="138c1-114">説明</span><span class="sxs-lookup"><span data-stu-id="138c1-114">Description</span></span> |
|:-----------------------|:------------|
| <span data-ttu-id="138c1-115">アーカイブ</span><span class="sxs-lookup"><span data-stu-id="138c1-115">archive</span></span> | <span data-ttu-id="138c1-116">アーカイブ フォルダーのメッセージは、対応する Outlook クライアントで One_Click アーカイブ機能を使用するときに送信されます。</span><span class="sxs-lookup"><span data-stu-id="138c1-116">The archive folder messages are sent to when using the One_Click Archive feature in Outlook clients that support it.</span></span> <span data-ttu-id="138c1-117">**注意:** これはExchange Onlineのアーカイブメールボックス機能と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="138c1-117">**Note:** this is not the same as the Archive Mailbox feature of Exchange online.</span></span> |
| <span data-ttu-id="138c1-118">低優先メール</span><span class="sxs-lookup"><span data-stu-id="138c1-118">clutter</span></span> | <span data-ttu-id="138c1-119">[Clutter]機能を使用すると、clutterフォルダに優先順位の低いメッセージがに移動されます。</span><span class="sxs-lookup"><span data-stu-id="138c1-119">The clutter folder low-priority messages are moved to when using the Clutter feature.</span></span> |
| <span data-ttu-id="138c1-120">競合</span><span class="sxs-lookup"><span data-stu-id="138c1-120">conflicts</span></span> | <span data-ttu-id="138c1-121">メールボックス内で競合するアイテムが含まれているフォルダ。</span><span class="sxs-lookup"><span data-stu-id="138c1-121">The folder that contains conflicting items in the mailbox.</span></span> |
| <span data-ttu-id="138c1-122">conversationhistory</span><span class="sxs-lookup"><span data-stu-id="138c1-122">conversationhistory</span></span> | <span data-ttu-id="138c1-123">SkypeがIM会話を保存するフォルダ（Skypeがそうするように設定されている場合）。</span><span class="sxs-lookup"><span data-stu-id="138c1-123">The folder where Skype saves IM conversations (if Skype is configured to do so).</span></span> |
| <span data-ttu-id="138c1-124">deleteditems</span><span class="sxs-lookup"><span data-stu-id="138c1-124">deleteditems</span></span> | <span data-ttu-id="138c1-125">フォルダ項目は、削除されたときに移動されます。</span><span class="sxs-lookup"><span data-stu-id="138c1-125">The folder items are moved to when they are deleted.</span></span> |
| <span data-ttu-id="138c1-126">下書き</span><span class="sxs-lookup"><span data-stu-id="138c1-126">drafts</span></span> | <span data-ttu-id="138c1-127">未送信メッセージが含まれているフォルダ。</span><span class="sxs-lookup"><span data-stu-id="138c1-127">The folder that contains unsent messages.</span></span> |
| <span data-ttu-id="138c1-128">inbox</span><span class="sxs-lookup"><span data-stu-id="138c1-128">inbox</span></span> | <span data-ttu-id="138c1-129">受信トレイ フォルダー。</span><span class="sxs-lookup"><span data-stu-id="138c1-129">The inbox folder.</span></span> |
| <span data-ttu-id="138c1-130">junkemail</span><span class="sxs-lookup"><span data-stu-id="138c1-130">junkemail</span></span> | <span data-ttu-id="138c1-131">[迷惑メール] フォルダー。</span><span class="sxs-lookup"><span data-stu-id="138c1-131">The junk email folder.</span></span> |
| <span data-ttu-id="138c1-132">localfailures</span><span class="sxs-lookup"><span data-stu-id="138c1-132">localfailures</span></span> | <span data-ttu-id="138c1-133">ローカルクライアントに存在するがサーバーにアップロードできなかったアイテムを含むフォルダ。</span><span class="sxs-lookup"><span data-stu-id="138c1-133">The folder that contains items that exist on the local client but could not be uploaded to the server.</span></span> |
| <span data-ttu-id="138c1-134">msgfolderroot</span><span class="sxs-lookup"><span data-stu-id="138c1-134">msgfolderroot</span></span> | <span data-ttu-id="138c1-135">"Top of Information Store" フォルダ。</span><span class="sxs-lookup"><span data-stu-id="138c1-135">The "Top of Information Store" folder.</span></span> <span data-ttu-id="138c1-136">このフォルダは、受信トレイなど、通常のメールクライアントに表示されるフォルダの親フォルダです。</span><span class="sxs-lookup"><span data-stu-id="138c1-136">This folder is the parent folder for folders that are displayed in normal mail clients, such as the inbox.</span></span> |
| <span data-ttu-id="138c1-137">送信トレイ</span><span class="sxs-lookup"><span data-stu-id="138c1-137">outbox</span></span> | <span data-ttu-id="138c1-138">送信トレイ フォルダー。</span><span class="sxs-lookup"><span data-stu-id="138c1-138">The outbox folder.</span></span> |
| <span data-ttu-id="138c1-139">recoverableitemsdeletions</span><span class="sxs-lookup"><span data-stu-id="138c1-139">recoverableitemsdeletions</span></span> | <span data-ttu-id="138c1-140">ソフト削除されたアイテムを含むフォルダ：[削除済みアイテム]フォルダから削除するか、OutlookでShift + Deleteキーを押して削除したアイテム。</span><span class="sxs-lookup"><span data-stu-id="138c1-140">The folder that contains soft-deleted items: deleted either from the Deleted Items folder, or by pressing shift+delete in Outlook.</span></span> <span data-ttu-id="138c1-141">このフォルダはどのOutlook電子メールクライアントにも表示されませんが、エンドユーザーはOutlookまたはWeb上のOutlookの**サーバーから削除済みアイテムを回復**機能を使用して操作できます。</span><span class="sxs-lookup"><span data-stu-id="138c1-141">This folder is not visible in any Outlook email client, but end users can interact with it through the **Recover Deleted Items from Server** feature in Outlook or Outlook on the web.</span></span> |
| <span data-ttu-id="138c1-142">スケジュール済み</span><span class="sxs-lookup"><span data-stu-id="138c1-142">scheduled</span></span> | <span data-ttu-id="138c1-143">iOS用Outlookのスケジュール機能を使用して受信トレイに再表示されるようにスケジュールされているメッセージを含むフォルダ。</span><span class="sxs-lookup"><span data-stu-id="138c1-143">The folder that contains messages that are scheduled to reappear in the inbox using the Schedule feature in Outlook for iOS.</span></span> |
| <span data-ttu-id="138c1-144">searchfolders</span><span class="sxs-lookup"><span data-stu-id="138c1-144">searchfolders</span></span> | <span data-ttu-id="138c1-145">ユーザーのメールボックスに定義されているすべての検索フォルダーの親フォルダー。</span><span class="sxs-lookup"><span data-stu-id="138c1-145">The parent folder for all search folders defined in the user's mailbox.</span></span> |
| <span data-ttu-id="138c1-146">sentitems</span><span class="sxs-lookup"><span data-stu-id="138c1-146">sentitems</span></span> | <span data-ttu-id="138c1-147">送信済みアイテム フォルダー。</span><span class="sxs-lookup"><span data-stu-id="138c1-147">The sent items folder.</span></span> |
| <span data-ttu-id="138c1-148">serverfailures</span><span class="sxs-lookup"><span data-stu-id="138c1-148">serverfailures</span></span> | <span data-ttu-id="138c1-149">サーバー上に存在するがローカルクライアントと同期できなかったアイテムを含むフォルダー。</span><span class="sxs-lookup"><span data-stu-id="138c1-149">The folder that contains items that exist on the server but could not be synchronized to the local client.</span></span> |
| <span data-ttu-id="138c1-150">syncissues</span><span class="sxs-lookup"><span data-stu-id="138c1-150">syncissues</span></span> | <span data-ttu-id="138c1-151">Outlookによって作成された同期ログを含むフォルダー。</span><span class="sxs-lookup"><span data-stu-id="138c1-151">The folder that contains synchronization logs created by Outlook.</span></span> |

## <a name="methods"></a><span data-ttu-id="138c1-152">メソッド</span><span class="sxs-lookup"><span data-stu-id="138c1-152">Methods</span></span>

| <span data-ttu-id="138c1-153">メソッド</span><span class="sxs-lookup"><span data-stu-id="138c1-153">Method</span></span> | <span data-ttu-id="138c1-154">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="138c1-154">Return Type</span></span> | <span data-ttu-id="138c1-155">説明</span><span class="sxs-lookup"><span data-stu-id="138c1-155">Description</span></span> |
|:-------|:------------|:------------|
|[<span data-ttu-id="138c1-156">mailFolder の取得</span><span class="sxs-lookup"><span data-stu-id="138c1-156">Get mailFolder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="138c1-157">mailFolder</span><span class="sxs-lookup"><span data-stu-id="138c1-157">mailFolder</span></span>](mailfolder.md) |<span data-ttu-id="138c1-158">mailFolder オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="138c1-158">Read properties and relationships of mailFolder object.</span></span>|
|[<span data-ttu-id="138c1-159">MailFolder の作成</span><span class="sxs-lookup"><span data-stu-id="138c1-159">Create MailFolder</span></span>](../api/mailfolder-post-childfolders.md) |[<span data-ttu-id="138c1-160">MailFolder</span><span class="sxs-lookup"><span data-stu-id="138c1-160">MailFolder</span></span>](mailfolder.md)| <span data-ttu-id="138c1-161">childFolders コレクションへの投稿により、現在の mailFolder 下に新しい mailFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="138c1-161">Create a new mailFolder under the current one by posting to the childFolders collection.</span></span>|
|[<span data-ttu-id="138c1-162">childFolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="138c1-162">List childFolders</span></span>](../api/mailfolder-list-childfolders.md) |<span data-ttu-id="138c1-163">[MailFolder](mailfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="138c1-163">[MailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="138c1-p107">指定したフォルダーの下のフォルダー コレクションを取得します。`.../me/MailFolders` ショートカットを使用すると、最上位フォルダーのコレクションを取得して、別のフォルダーに移動することができます。</span><span class="sxs-lookup"><span data-stu-id="138c1-p107">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>|
|[<span data-ttu-id="138c1-166">メッセージの作成</span><span class="sxs-lookup"><span data-stu-id="138c1-166">Create Message</span></span>](../api/mailfolder-post-messages.md) |[<span data-ttu-id="138c1-167">Message</span><span class="sxs-lookup"><span data-stu-id="138c1-167">Message</span></span>](message.md)| <span data-ttu-id="138c1-168">メッセージ コレクションへの投稿により、現在の mailFolder に新しいメッセージを作成します。</span><span class="sxs-lookup"><span data-stu-id="138c1-168">Create a new message in the current mailFolder by posting to the messages collection.</span></span>|
|[<span data-ttu-id="138c1-169">List messages</span><span class="sxs-lookup"><span data-stu-id="138c1-169">List messages</span></span>](../api/mailfolder-list-messages.md) |<span data-ttu-id="138c1-170">[Message](message.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="138c1-170">[Message](message.md) collection</span></span>| <span data-ttu-id="138c1-171">サインインしているユーザーのメールボックス内のすべてのメッセージや、メールボックス内の指定したフォルダー内のメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="138c1-171">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>|
|[<span data-ttu-id="138c1-172">更新する</span><span class="sxs-lookup"><span data-stu-id="138c1-172">Update</span></span>](../api/mailfolder-update.md) | [<span data-ttu-id="138c1-173">mailFolder</span><span class="sxs-lookup"><span data-stu-id="138c1-173">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="138c1-174">指定した mailFolder オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="138c1-174">Update the specified mailFolder object.</span></span> |
|[<span data-ttu-id="138c1-175">削除</span><span class="sxs-lookup"><span data-stu-id="138c1-175">Delete</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="138c1-176">なし</span><span class="sxs-lookup"><span data-stu-id="138c1-176">None</span></span> |<span data-ttu-id="138c1-177">指定した mailFolder オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="138c1-177">Delete the specified mailFolder object.</span></span> |
|[<span data-ttu-id="138c1-178">コピー</span><span class="sxs-lookup"><span data-stu-id="138c1-178">copy</span></span>](../api/mailfolder-copy.md)|[<span data-ttu-id="138c1-179">MailFolder</span><span class="sxs-lookup"><span data-stu-id="138c1-179">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="138c1-180">mailFolder とその内容を別の mailFolder にコピーします。</span><span class="sxs-lookup"><span data-stu-id="138c1-180">Copy a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="138c1-181">delta</span><span class="sxs-lookup"><span data-stu-id="138c1-181">delta</span></span>](../api/mailfolder-delta.md)|<span data-ttu-id="138c1-182">[mailFolder](mailfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="138c1-182">[mailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="138c1-183">ユーザーのメールボックスで追加または削除された一連のメール フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="138c1-183">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="138c1-184">move</span><span class="sxs-lookup"><span data-stu-id="138c1-184">move</span></span>](../api/mailfolder-move.md)|[<span data-ttu-id="138c1-185">MailFolder</span><span class="sxs-lookup"><span data-stu-id="138c1-185">MailFolder</span></span>](mailfolder.md)|<span data-ttu-id="138c1-186">mailFolder とその内容を別の mailFolder に移動します。</span><span class="sxs-lookup"><span data-stu-id="138c1-186">Move a mailFolder and its contents to another mailFolder.</span></span>|
|<span data-ttu-id="138c1-187">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="138c1-187">**Extended properties**</span></span>| | |
|[<span data-ttu-id="138c1-188">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="138c1-188">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="138c1-189">mailFolder</span><span class="sxs-lookup"><span data-stu-id="138c1-189">mailFolder</span></span>](mailfolder.md)  |<span data-ttu-id="138c1-190">新規または既存の mailFolder に、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="138c1-190">Create one or more single-value extended properties in a new or existing mailFolder.</span></span>   |
|[<span data-ttu-id="138c1-191">単一値の拡張プロパティを持つ mailFolder の取得</span><span class="sxs-lookup"><span data-stu-id="138c1-191">Get mailFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="138c1-192">mailFolder</span><span class="sxs-lookup"><span data-stu-id="138c1-192">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="138c1-193">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含む mailFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="138c1-193">Get mailFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="138c1-194">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="138c1-194">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="138c1-195">mailFolder</span><span class="sxs-lookup"><span data-stu-id="138c1-195">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="138c1-196">新規または既存の mailFolder の 1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="138c1-196">Create one or more multi-value extended properties in a new or existing mailFolder.</span></span>  |
|[<span data-ttu-id="138c1-197">複数値の拡張プロパティを持つ mailFolder の取得</span><span class="sxs-lookup"><span data-stu-id="138c1-197">Get mailFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="138c1-198">mailFolder</span><span class="sxs-lookup"><span data-stu-id="138c1-198">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="138c1-199">`$expand` を使用して、複数値の拡張プロパティを含む mailFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="138c1-199">Get a mailFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="138c1-200">プロパティ</span><span class="sxs-lookup"><span data-stu-id="138c1-200">Properties</span></span>

| <span data-ttu-id="138c1-201">プロパティ</span><span class="sxs-lookup"><span data-stu-id="138c1-201">Property</span></span> | <span data-ttu-id="138c1-202">型</span><span class="sxs-lookup"><span data-stu-id="138c1-202">Type</span></span> | <span data-ttu-id="138c1-203">説明</span><span class="sxs-lookup"><span data-stu-id="138c1-203">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="138c1-204">childFolderCount</span><span class="sxs-lookup"><span data-stu-id="138c1-204">childFolderCount</span></span>|<span data-ttu-id="138c1-205">Int32</span><span class="sxs-lookup"><span data-stu-id="138c1-205">Int32</span></span>|<span data-ttu-id="138c1-206">現在の mailFolder の直下の子 mailFolder の数。</span><span class="sxs-lookup"><span data-stu-id="138c1-206">The number of immediate child mailFolders in the current mailFolder.</span></span>|
|<span data-ttu-id="138c1-207">displayName</span><span class="sxs-lookup"><span data-stu-id="138c1-207">displayName</span></span>|<span data-ttu-id="138c1-208">String</span><span class="sxs-lookup"><span data-stu-id="138c1-208">String</span></span>|<span data-ttu-id="138c1-209">mailFolder の表示名。</span><span class="sxs-lookup"><span data-stu-id="138c1-209">The mailFolder's display name.</span></span>|
|<span data-ttu-id="138c1-210">id</span><span class="sxs-lookup"><span data-stu-id="138c1-210">id</span></span>|<span data-ttu-id="138c1-211">文字列</span><span class="sxs-lookup"><span data-stu-id="138c1-211">String</span></span>|<span data-ttu-id="138c1-212">mailFolder の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="138c1-212">The mailFolder's unique identifier.</span></span>|
|<span data-ttu-id="138c1-213">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="138c1-213">parentFolderId</span></span>|<span data-ttu-id="138c1-214">String</span><span class="sxs-lookup"><span data-stu-id="138c1-214">String</span></span>|<span data-ttu-id="138c1-215">mailFolder の親 mailFolder の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="138c1-215">The unique identifier for the mailFolder's parent mailFolder.</span></span>|
|<span data-ttu-id="138c1-216">totalItemCount</span><span class="sxs-lookup"><span data-stu-id="138c1-216">totalItemCount</span></span>|<span data-ttu-id="138c1-217">Int32</span><span class="sxs-lookup"><span data-stu-id="138c1-217">Int32</span></span>|<span data-ttu-id="138c1-218">mailFolder に含まれるアイテムの数</span><span class="sxs-lookup"><span data-stu-id="138c1-218">The number of items in the mailFolder.</span></span>|
|<span data-ttu-id="138c1-219">unreadItemCount</span><span class="sxs-lookup"><span data-stu-id="138c1-219">unreadItemCount</span></span>|<span data-ttu-id="138c1-220">Int32</span><span class="sxs-lookup"><span data-stu-id="138c1-220">Int32</span></span>|<span data-ttu-id="138c1-221">mailFolder 内で未読としてマークされているアイテムの数。</span><span class="sxs-lookup"><span data-stu-id="138c1-221">The number of items in the mailFolder marked as unread.</span></span>|

<span data-ttu-id="138c1-222">**アイテム数を効率的に取得する**</span><span class="sxs-lookup"><span data-stu-id="138c1-222">**Access item counts efficiently**</span></span>

<span data-ttu-id="138c1-223">フォルダーの `TotalItemCount`プロパティと `UnreadItemCount` プロパティを使用すると、ファイル内の既読アイテム数を簡単に算出できます。</span><span class="sxs-lookup"><span data-stu-id="138c1-223">The `TotalItemCount` and `UnreadItemCount` properties of a folder allow you to conveniently compute the number of read items in the folder.</span></span>
<span data-ttu-id="138c1-224">大幅な待ち時間を招く可能性がある次のようなクエリを避けることができます。</span><span class="sxs-lookup"><span data-stu-id="138c1-224">They let you avoid queries like the following that can incur significant latency:</span></span>

```http
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

<span data-ttu-id="138c1-225">Outlookのメールフォルダには複数の種類のアイテムを含めることができます。たとえば、受信トレイにはメールアイテムとは異なる会議出席依頼アイテムを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="138c1-225">Mail folders in Outlook can contain more than one type of items, for example, the Inbox can contain meeting request items which are distinct from mail items.</span></span> <span data-ttu-id="138c1-226">`TotalItemCount` と `UnreadItemCount` には、アイテムの種類に関係なく、フォルダー内のアイテム全てが含まれます。</span><span class="sxs-lookup"><span data-stu-id="138c1-226">`TotalItemCount` and `UnreadItemCount` include items in a mail folder irrespective of their item types.</span></span>

## <a name="relationships"></a><span data-ttu-id="138c1-227">関係</span><span class="sxs-lookup"><span data-stu-id="138c1-227">Relationships</span></span>

| <span data-ttu-id="138c1-228">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="138c1-228">Relationship</span></span> | <span data-ttu-id="138c1-229">型</span><span class="sxs-lookup"><span data-stu-id="138c1-229">Type</span></span> | <span data-ttu-id="138c1-230">説明</span><span class="sxs-lookup"><span data-stu-id="138c1-230">Description</span></span> |
|:-------------|:-----|:------------|
|<span data-ttu-id="138c1-231">childFolders</span><span class="sxs-lookup"><span data-stu-id="138c1-231">childFolders</span></span>|<span data-ttu-id="138c1-232">[MailFolder](mailfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="138c1-232">[MailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="138c1-233">mailFolder 内の子フォルダーのコレクション。</span><span class="sxs-lookup"><span data-stu-id="138c1-233">The collection of child folders in the mailFolder.</span></span>|
|<span data-ttu-id="138c1-234">messageRules</span><span class="sxs-lookup"><span data-stu-id="138c1-234">messageRules</span></span> | <span data-ttu-id="138c1-235">[messageRule](messagerule.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="138c1-235">[messageRule](messagerule.md) collection</span></span> | <span data-ttu-id="138c1-236">ユーザーの受信トレイ フォルダーに適用されるルールのコレクション。</span><span class="sxs-lookup"><span data-stu-id="138c1-236">The collection of rules that apply to the user's Inbox folder.</span></span> |
|<span data-ttu-id="138c1-237">messages</span><span class="sxs-lookup"><span data-stu-id="138c1-237">messages</span></span>|<span data-ttu-id="138c1-238">[Message](message.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="138c1-238">[Message](message.md) collection</span></span>|<span data-ttu-id="138c1-239">mailFolder 内のメッセージのコレクション。</span><span class="sxs-lookup"><span data-stu-id="138c1-239">The collection of messages in the mailFolder.</span></span>|
|<span data-ttu-id="138c1-240">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="138c1-240">multiValueExtendedProperties</span></span>|<span data-ttu-id="138c1-241">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="138c1-241">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="138c1-p110">mailFolder に対して定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="138c1-p110">The collection of multi-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="138c1-245">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="138c1-245">singleValueExtendedProperties</span></span>|<span data-ttu-id="138c1-246">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="138c1-246">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="138c1-p111">mailFolder に対して定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="138c1-p111">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="138c1-250">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="138c1-250">JSON representation</span></span>

<span data-ttu-id="138c1-251">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="138c1-251">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messageRules",
    "messages",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.mailFolder",
  "@odata.annotations": [
    {
      "property": "childFolders",
      "capabilities": {
        "changeTracking": false,
        "navigability": "single",
        "searchable": false
      }
    },
    {
      "property": "messageRules",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "messages",
      "capabilities": {
        "changeTracking": true,
        "navigability": "single"
      }
    }
  ]
}-->

```json
{
  "childFolderCount": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "totalItemCount": 1024,
  "unreadItemCount": 1024,
  "childFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "messageRules": [ { "@odata.type": "microsoft.graph.messageRule" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}
```

## <a name="see-also"></a><span data-ttu-id="138c1-252">関連項目</span><span class="sxs-lookup"><span data-stu-id="138c1-252">See also</span></span>

- [<span data-ttu-id="138c1-253">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="138c1-253">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="138c1-254">フォルダー内のメッセージへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="138c1-254">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
