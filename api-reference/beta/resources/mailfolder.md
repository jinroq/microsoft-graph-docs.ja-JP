---
title: mailFolder リソースの種類
description: 受信トレイや下書きなどの、ユーザーのメールボックス内のメール フォルダーです。 メール フォルダーには、メッセージ、他の Outlook アイテム、子メール フォルダーを含めることができます。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 1cd48c866ea6384aa18631732065380e898b8bf7
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642696"
---
# <a name="mailfolder-resource-type"></a><span data-ttu-id="bc1aa-104">mailFolder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bc1aa-104">mailFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc1aa-105">受信トレイや下書きなどの、ユーザーのメールボックス内のメール フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-105">A mail folder in a user's mailbox, such as Inbox and Drafts.</span></span> <span data-ttu-id="bc1aa-106">メール フォルダーには、メッセージ、他の Outlook アイテム、子メール フォルダーを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-106">Mail folders can contain messages, other Outlook items, and child mail folders.</span></span>

<span data-ttu-id="bc1aa-107">このリソースでは、[デルタ](../api/mailfolder-delta.md)関数を用意すれば、増分の追加、削除、更新に[デルタ クエリ](/graph/delta-query-overview)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-107">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/mailfolder-delta.md) function.</span></span>

<span data-ttu-id="bc1aa-108">**既知のフォルダー名**</span><span class="sxs-lookup"><span data-stu-id="bc1aa-108">**Well-known folder names**</span></span>

<span data-ttu-id="bc1aa-109">Outlook では、既定でユーザー用の特定のフォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-109">Outlook creates certain folders for users by default.</span></span> <span data-ttu-id="bc1aa-110">対応するフォルダーの**id**値を使用して、利便性のため、代わりにこれらのフォルダーにアクセスするときに既知のフォルダー名を次の表からを使用できます。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-110">Instead of using the corresponding folder **id** value, for convenience, you can use the well-known folder names from the table below when accessing these folders.</span></span> <span data-ttu-id="bc1aa-111">たとえば、次のクエリを使用して、既知の名前を使用して、[下書き] フォルダーを取得できます。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-111">For example, you can get the Drafts folder using its well-known name with the following query.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

<span data-ttu-id="bc1aa-112">既知の名前は、上記のクエリは、常に付けの方法に関係なく、ユーザーの [下書き] フォルダーを返しますので、ユーザーのメールボックスのロケールに関係なく動作します。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-112">Well-known names work regardless of the locale of the user's mailbox, so the above query will always return the user's Drafts folder regardless of how it is named.</span></span>

| <span data-ttu-id="bc1aa-113">既知のフォルダー名</span><span class="sxs-lookup"><span data-stu-id="bc1aa-113">Well-known folder name</span></span> | <span data-ttu-id="bc1aa-114">説明</span><span class="sxs-lookup"><span data-stu-id="bc1aa-114">Description</span></span> |
|:-----------------------|:------------|
| <span data-ttu-id="bc1aa-115">アーカイブ</span><span class="sxs-lookup"><span data-stu-id="bc1aa-115">archive</span></span> | <span data-ttu-id="bc1aa-116">アーカイブ フォルダーのメッセージは、サポートしている Outlook クライアントで One_Click のアーカイブ機能を使用する場合に送信されます。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-116">The archive folder messages are sent to when using the One_Click Archive feature in Outlook clients that support it.</span></span> <span data-ttu-id="bc1aa-117">**注:** これは Exchange のメールボックスのアーカイブの機能は、オンラインの場合と同じです。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-117">**Note:** this is not the same as the Archive Mailbox feature of Exchange online.</span></span> |
| <span data-ttu-id="bc1aa-118">散乱</span><span class="sxs-lookup"><span data-stu-id="bc1aa-118">clutter</span></span> | <span data-ttu-id="bc1aa-119">整理フォルダーの優先順位の低いメッセージは、整理機能を使用するときに移動されます。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-119">The clutter folder low-priority messages are moved to when using the Clutter feature.</span></span> |
| <span data-ttu-id="bc1aa-120">競合</span><span class="sxs-lookup"><span data-stu-id="bc1aa-120">conflicts</span></span> | <span data-ttu-id="bc1aa-121">メールボックスにある競合アイテムを含むフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-121">The folder that contains conflicting items in the mailbox.</span></span> |
| <span data-ttu-id="bc1aa-122">conversationhistory</span><span class="sxs-lookup"><span data-stu-id="bc1aa-122">conversationhistory</span></span> | <span data-ttu-id="bc1aa-123">(これを行うには、Skype が構成されている) 場合に、Skype が IM の会話を保存するフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-123">The folder where Skype saves IM conversations (if Skype is configured to do so).</span></span> |
| <span data-ttu-id="bc1aa-124">deleteditems</span><span class="sxs-lookup"><span data-stu-id="bc1aa-124">deleteditems</span></span> | <span data-ttu-id="bc1aa-125">フォルダーのアイテムは、削除するときに移動されます。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-125">The folder items are moved to when they are deleted.</span></span> |
| <span data-ttu-id="bc1aa-126">下書き</span><span class="sxs-lookup"><span data-stu-id="bc1aa-126">drafts</span></span> | <span data-ttu-id="bc1aa-127">未送信のメッセージを格納するフォルダー。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-127">The folder that contains unsent messages.</span></span> |
| <span data-ttu-id="bc1aa-128">[受信トレイ]</span><span class="sxs-lookup"><span data-stu-id="bc1aa-128">inbox</span></span> | <span data-ttu-id="bc1aa-129">[受信トレイ] フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-129">The inbox folder.</span></span> |
| <span data-ttu-id="bc1aa-130">junkemail</span><span class="sxs-lookup"><span data-stu-id="bc1aa-130">junkemail</span></span> | <span data-ttu-id="bc1aa-131">迷惑メールのフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-131">The junk email folder.</span></span> |
| <span data-ttu-id="bc1aa-132">localfailures</span><span class="sxs-lookup"><span data-stu-id="bc1aa-132">localfailures</span></span> | <span data-ttu-id="bc1aa-133">ローカル クライアント上に存在するが、サーバーにアップロードできませんでしたアイテムを含むフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-133">The folder that contains items that exist on the local client but could not be uploaded to the server.</span></span> |
| <span data-ttu-id="bc1aa-134">msgfolderroot</span><span class="sxs-lookup"><span data-stu-id="bc1aa-134">msgfolderroot</span></span> | <span data-ttu-id="bc1aa-135">「インフォメーション ストアの最上位」のフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-135">The "Top of Information Store" folder.</span></span> <span data-ttu-id="bc1aa-136">このフォルダーは、受信トレイなど、通常のメール クライアントで表示されているフォルダーの親フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-136">This folder is the parent folder for folders that are displayed in normal mail clients, such as the inbox.</span></span> |
| <span data-ttu-id="bc1aa-137">[送信トレイ] します。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-137">outbox</span></span> | <span data-ttu-id="bc1aa-138">[送信トレイ] フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-138">The outbox folder.</span></span> |
| <span data-ttu-id="bc1aa-139">recoverableitemsdeletions</span><span class="sxs-lookup"><span data-stu-id="bc1aa-139">recoverableitemsdeletions</span></span> | <span data-ttu-id="bc1aa-140">ソフト削除済みアイテムを含むフォルダー: 削除済みアイテム フォルダーから、または shift キーを押して削除 + では、Outlook を削除します。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-140">The folder that contains soft-deleted items: deleted either from the Deleted Items folder, or by pressing shift+delete in Outlook.</span></span> <span data-ttu-id="bc1aa-141">このフォルダーが、Outlook 電子メール クライアントに表示されないが、エンド ・ ユーザーを操作できます Outlook または Outlook web 上で**サーバーから削除済みアイテムの回復**機能を使用します。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-141">This folder is not visible in any Outlook email client, but end users can interact with it through the **Recover Deleted Items from Server** feature in Outlook or Outlook on the web.</span></span> |
| <span data-ttu-id="bc1aa-142">スケジュール済み</span><span class="sxs-lookup"><span data-stu-id="bc1aa-142">scheduled</span></span> | <span data-ttu-id="bc1aa-143">IOS は、Outlook のスケジュール機能を使用して受信トレイに表示されるようにスケジュールされているメッセージを含むフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-143">The folder that contains messages that are scheduled to reappear in the inbox using the Schedule feature in Outlook for iOS.</span></span> |
| <span data-ttu-id="bc1aa-144">使用して</span><span class="sxs-lookup"><span data-stu-id="bc1aa-144">searchfolders</span></span> | <span data-ttu-id="bc1aa-145">ユーザーのメールボックスで定義されているすべての検索フォルダーの親フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-145">The parent folder for all search folders defined in the user's mailbox.</span></span> |
| <span data-ttu-id="bc1aa-146">送信済みアイテム</span><span class="sxs-lookup"><span data-stu-id="bc1aa-146">sentitems</span></span> | <span data-ttu-id="bc1aa-147">送信済みアイテム フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-147">The sent items folder.</span></span> |
| <span data-ttu-id="bc1aa-148">serverfailures</span><span class="sxs-lookup"><span data-stu-id="bc1aa-148">serverfailures</span></span> | <span data-ttu-id="bc1aa-149">サーバー上に存在するが、ローカル クライアントを同期できませんでしたアイテムを含むフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-149">The folder that contains items that exist on the server but could not be synchronized to the local client.</span></span> |
| <span data-ttu-id="bc1aa-150">syncissues</span><span class="sxs-lookup"><span data-stu-id="bc1aa-150">syncissues</span></span> | <span data-ttu-id="bc1aa-151">Outlook で作成された同期ログを格納するフォルダー。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-151">The folder that contains synchronization logs created by Outlook.</span></span> |

## <a name="methods"></a><span data-ttu-id="bc1aa-152">メソッド</span><span class="sxs-lookup"><span data-stu-id="bc1aa-152">Methods</span></span>

| <span data-ttu-id="bc1aa-153">メソッド</span><span class="sxs-lookup"><span data-stu-id="bc1aa-153">Method</span></span> | <span data-ttu-id="bc1aa-154">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bc1aa-154">Return Type</span></span> | <span data-ttu-id="bc1aa-155">説明</span><span class="sxs-lookup"><span data-stu-id="bc1aa-155">Description</span></span> |
|:-------|:------------|:------------|
|[<span data-ttu-id="bc1aa-156">mailFolder の取得</span><span class="sxs-lookup"><span data-stu-id="bc1aa-156">Get mailFolder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="bc1aa-157">mailFolder</span><span class="sxs-lookup"><span data-stu-id="bc1aa-157">mailFolder</span></span>](mailfolder.md) |<span data-ttu-id="bc1aa-158">mailFolder オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-158">Read properties and relationships of mailFolder object.</span></span>|
|[<span data-ttu-id="bc1aa-159">MailFolder の作成</span><span class="sxs-lookup"><span data-stu-id="bc1aa-159">Create MailFolder</span></span>](../api/mailfolder-post-childfolders.md) |[<span data-ttu-id="bc1aa-160">mailFolder</span><span class="sxs-lookup"><span data-stu-id="bc1aa-160">mailFolder</span></span>](mailfolder.md)| <span data-ttu-id="bc1aa-161">childFolders コレクションへの投稿により、現在の mailFolder 下に新しい mailFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-161">Create a new mailFolder under the current one by posting to the childFolders collection.</span></span>|
|[<span data-ttu-id="bc1aa-162">childFolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="bc1aa-162">List childFolders</span></span>](../api/mailfolder-list-childfolders.md) |<span data-ttu-id="bc1aa-163">[mailFolder](mailfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bc1aa-163">[mailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="bc1aa-p107">指定したフォルダーの下のフォルダー コレクションを取得します。`.../me/MailFolders` ショートカットを使用すると、最上位フォルダーのコレクションを取得して、別のフォルダーに移動することができます。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-p107">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>|
|[<span data-ttu-id="bc1aa-166">メッセージの作成</span><span class="sxs-lookup"><span data-stu-id="bc1aa-166">Create Message</span></span>](../api/mailfolder-post-messages.md) |[<span data-ttu-id="bc1aa-167">message</span><span class="sxs-lookup"><span data-stu-id="bc1aa-167">message</span></span>](message.md)| <span data-ttu-id="bc1aa-168">メッセージ コレクションへの投稿により、現在の mailFolder に新しいメッセージを作成します。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-168">Create a new message in the current mailFolder by posting to the messages collection.</span></span>|
|[<span data-ttu-id="bc1aa-169">List messages</span><span class="sxs-lookup"><span data-stu-id="bc1aa-169">List messages</span></span>](../api/mailfolder-list-messages.md) |<span data-ttu-id="bc1aa-170">[message](message.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bc1aa-170">[message](message.md) collection</span></span>| <span data-ttu-id="bc1aa-171">サインインしているユーザーのメールボックス内のすべてのメッセージや、メールボックス内の指定したフォルダー内のメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-171">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>|
|[<span data-ttu-id="bc1aa-172">更新する</span><span class="sxs-lookup"><span data-stu-id="bc1aa-172">Update</span></span>](../api/mailfolder-update.md) | [<span data-ttu-id="bc1aa-173">mailFolder</span><span class="sxs-lookup"><span data-stu-id="bc1aa-173">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="bc1aa-174">指定した mailFolder オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-174">Update the specified mailFolder object.</span></span> |
|[<span data-ttu-id="bc1aa-175">削除</span><span class="sxs-lookup"><span data-stu-id="bc1aa-175">Delete</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="bc1aa-176">なし</span><span class="sxs-lookup"><span data-stu-id="bc1aa-176">None</span></span> |<span data-ttu-id="bc1aa-177">指定した mailFolder オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-177">Delete the specified mailFolder object.</span></span> |
|[<span data-ttu-id="bc1aa-178">コピー</span><span class="sxs-lookup"><span data-stu-id="bc1aa-178">copy</span></span>](../api/mailfolder-copy.md)|[<span data-ttu-id="bc1aa-179">mailFolder</span><span class="sxs-lookup"><span data-stu-id="bc1aa-179">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="bc1aa-180">mailFolder とその内容を別の mailFolder にコピーします。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-180">Copy a mailFolder and its contents to another mailFolder.</span></span>|
|[<span data-ttu-id="bc1aa-181">delta</span><span class="sxs-lookup"><span data-stu-id="bc1aa-181">delta</span></span>](../api/mailfolder-delta.md)|<span data-ttu-id="bc1aa-182">[mailFolder](mailfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bc1aa-182">[mailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="bc1aa-183">ユーザーのメールボックスで追加または削除された一連のメール フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-183">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="bc1aa-184">move</span><span class="sxs-lookup"><span data-stu-id="bc1aa-184">move</span></span>](../api/mailfolder-move.md)|[<span data-ttu-id="bc1aa-185">mailFolder</span><span class="sxs-lookup"><span data-stu-id="bc1aa-185">mailFolder</span></span>](mailfolder.md)|<span data-ttu-id="bc1aa-186">mailFolder とその内容を別の mailFolder に移動します。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-186">Move a mailFolder and its contents to another mailFolder.</span></span>|
|<span data-ttu-id="bc1aa-187">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="bc1aa-187">**Extended properties**</span></span>| | |
|[<span data-ttu-id="bc1aa-188">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="bc1aa-188">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="bc1aa-189">mailFolder</span><span class="sxs-lookup"><span data-stu-id="bc1aa-189">mailFolder</span></span>](mailfolder.md)  |<span data-ttu-id="bc1aa-190">新規または既存の mailFolder に、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-190">Create one or more single-value extended properties in a new or existing mailFolder.</span></span>   |
|[<span data-ttu-id="bc1aa-191">単一値の拡張プロパティを持つ mailFolder の取得</span><span class="sxs-lookup"><span data-stu-id="bc1aa-191">Get mailFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="bc1aa-192">mailFolder</span><span class="sxs-lookup"><span data-stu-id="bc1aa-192">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="bc1aa-193">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含む mailFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-193">Get mailFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="bc1aa-194">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="bc1aa-194">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="bc1aa-195">mailFolder</span><span class="sxs-lookup"><span data-stu-id="bc1aa-195">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="bc1aa-196">新規または既存の mailFolder の 1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-196">Create one or more multi-value extended properties in a new or existing mailFolder.</span></span>  |
|[<span data-ttu-id="bc1aa-197">複数値の拡張プロパティを持つ mailFolder の取得</span><span class="sxs-lookup"><span data-stu-id="bc1aa-197">Get mailFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="bc1aa-198">mailFolder</span><span class="sxs-lookup"><span data-stu-id="bc1aa-198">mailFolder</span></span>](mailfolder.md) | <span data-ttu-id="bc1aa-199">`$expand` を使用して、複数値の拡張プロパティを含む mailFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-199">Get a mailFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="bc1aa-200">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc1aa-200">Properties</span></span>

| <span data-ttu-id="bc1aa-201">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc1aa-201">Property</span></span> | <span data-ttu-id="bc1aa-202">型</span><span class="sxs-lookup"><span data-stu-id="bc1aa-202">Type</span></span> | <span data-ttu-id="bc1aa-203">説明</span><span class="sxs-lookup"><span data-stu-id="bc1aa-203">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="bc1aa-204">childFolderCount</span><span class="sxs-lookup"><span data-stu-id="bc1aa-204">childFolderCount</span></span>|<span data-ttu-id="bc1aa-205">Int32</span><span class="sxs-lookup"><span data-stu-id="bc1aa-205">Int32</span></span>|<span data-ttu-id="bc1aa-206">現在の mailFolder の直下の子 mailFolder の数。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-206">The number of immediate child mailFolders in the current mailFolder.</span></span>|
|<span data-ttu-id="bc1aa-207">displayName</span><span class="sxs-lookup"><span data-stu-id="bc1aa-207">displayName</span></span>|<span data-ttu-id="bc1aa-208">String</span><span class="sxs-lookup"><span data-stu-id="bc1aa-208">String</span></span>|<span data-ttu-id="bc1aa-209">mailFolder の表示名。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-209">The mailFolder's display name.</span></span>|
|<span data-ttu-id="bc1aa-210">id</span><span class="sxs-lookup"><span data-stu-id="bc1aa-210">id</span></span>|<span data-ttu-id="bc1aa-211">String</span><span class="sxs-lookup"><span data-stu-id="bc1aa-211">String</span></span>|<span data-ttu-id="bc1aa-212">MailFolder の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-212">The mailFolder's unique identifier.</span></span>|
|<span data-ttu-id="bc1aa-213">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="bc1aa-213">parentFolderId</span></span>|<span data-ttu-id="bc1aa-214">String</span><span class="sxs-lookup"><span data-stu-id="bc1aa-214">String</span></span>|<span data-ttu-id="bc1aa-215">mailFolder の親 mailFolder の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-215">The unique identifier for the mailFolder's parent mailFolder.</span></span>|
|<span data-ttu-id="bc1aa-216">totalItemCount</span><span class="sxs-lookup"><span data-stu-id="bc1aa-216">totalItemCount</span></span>|<span data-ttu-id="bc1aa-217">Int32</span><span class="sxs-lookup"><span data-stu-id="bc1aa-217">Int32</span></span>|<span data-ttu-id="bc1aa-218">mailFolder に含まれるアイテムの数</span><span class="sxs-lookup"><span data-stu-id="bc1aa-218">The number of items in the mailFolder.</span></span>|
|<span data-ttu-id="bc1aa-219">unreadItemCount</span><span class="sxs-lookup"><span data-stu-id="bc1aa-219">unreadItemCount</span></span>|<span data-ttu-id="bc1aa-220">Int32</span><span class="sxs-lookup"><span data-stu-id="bc1aa-220">Int32</span></span>|<span data-ttu-id="bc1aa-221">mailFolder 内で未読としてマークされているアイテムの数。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-221">The number of items in the mailFolder marked as unread.</span></span>|
|<span data-ttu-id="bc1aa-222">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="bc1aa-222">wellKnownName</span></span>|<span data-ttu-id="bc1aa-223">String</span><span class="sxs-lookup"><span data-stu-id="bc1aa-223">String</span></span>|<span data-ttu-id="bc1aa-224">フォルダーの既知のフォルダーの名前です。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-224">The well-known folder name for the folder.</span></span> <span data-ttu-id="bc1aa-225">可能な値は、上記に一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-225">The possible values are listed above.</span></span> <span data-ttu-id="bc1aa-226">Outlook で作成された既定のフォルダーには、このプロパティは設定のみです。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-226">This property is only set for default folders created by Outlook.</span></span> <span data-ttu-id="bc1aa-227">その他のフォルダーでは、このプロパティは**null**です。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-227">For other folders, this property is **null**.</span></span>|

<span data-ttu-id="bc1aa-228">**アイテム数を効率的に取得する**</span><span class="sxs-lookup"><span data-stu-id="bc1aa-228">**Access item counts efficiently**</span></span>

<span data-ttu-id="bc1aa-229">`TotalItemCount`と`UnreadItemCount`フォルダーのプロパティを使用すると、簡単にフォルダー内のアイテムの読み取りの数を計算します。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-229">The `TotalItemCount` and `UnreadItemCount` properties of a folder allow you to conveniently compute the number of read items in the folder.</span></span>
<span data-ttu-id="bc1aa-230">これにより、大幅な遅延が発生する可能性がある次のようなクエリを回避できます。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-230">They let you avoid queries like the following that can incur significant latency:</span></span>

```http
https://outlook.office.com/api/beta/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

<span data-ttu-id="bc1aa-231">Outlook のメール フォルダーにアイテムの 1 つ以上の種類を含めることができます、受信トレイを含めることができますたとえば、会議出席依頼アイテムがメール アイテムとは異なる。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-231">Mail folders in Outlook can contain more than one type of items, for example, the Inbox can contain meeting request items which are distinct from mail items.</span></span> <span data-ttu-id="bc1aa-232">`TotalItemCount``UnreadItemCount`の項目の種類に関係なく、[メール] フォルダーにアイテムが含まれます。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-232">`TotalItemCount` and `UnreadItemCount` include items in a mail folder irrespective of their item types.</span></span>

## <a name="relationships"></a><span data-ttu-id="bc1aa-233">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bc1aa-233">Relationships</span></span>

| <span data-ttu-id="bc1aa-234">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bc1aa-234">Relationship</span></span> | <span data-ttu-id="bc1aa-235">型</span><span class="sxs-lookup"><span data-stu-id="bc1aa-235">Type</span></span> | <span data-ttu-id="bc1aa-236">説明</span><span class="sxs-lookup"><span data-stu-id="bc1aa-236">Description</span></span> |
|:-------------|:-----|:------------|
|<span data-ttu-id="bc1aa-237">childFolders</span><span class="sxs-lookup"><span data-stu-id="bc1aa-237">childFolders</span></span>|<span data-ttu-id="bc1aa-238">[MailFolder](mailfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bc1aa-238">[MailFolder](mailfolder.md) collection</span></span>|<span data-ttu-id="bc1aa-239">mailFolder 内の子フォルダーのコレクション。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-239">The collection of child folders in the mailFolder.</span></span>|
|<span data-ttu-id="bc1aa-240">messageRules</span><span class="sxs-lookup"><span data-stu-id="bc1aa-240">messageRules</span></span> | <span data-ttu-id="bc1aa-241">[messageRule](messagerule.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bc1aa-241">[messageRule](messagerule.md) collection</span></span> | <span data-ttu-id="bc1aa-242">ユーザーの受信トレイ フォルダーに適用されるルールのコレクション。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-242">The collection of rules that apply to the user's Inbox folder.</span></span> |
|<span data-ttu-id="bc1aa-243">messages</span><span class="sxs-lookup"><span data-stu-id="bc1aa-243">messages</span></span>|<span data-ttu-id="bc1aa-244">[Message](message.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bc1aa-244">[Message](message.md) collection</span></span>|<span data-ttu-id="bc1aa-245">mailFolder 内のメッセージのコレクション。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-245">The collection of messages in the mailFolder.</span></span>|
|<span data-ttu-id="bc1aa-246">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="bc1aa-246">multiValueExtendedProperties</span></span>|<span data-ttu-id="bc1aa-247">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bc1aa-247">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="bc1aa-p111">mailFolder に対して定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-p111">The collection of multi-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="bc1aa-251">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="bc1aa-251">singleValueExtendedProperties</span></span>|<span data-ttu-id="bc1aa-252">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bc1aa-252">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="bc1aa-p112">mailFolder に対して定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-p112">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bc1aa-256">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bc1aa-256">JSON representation</span></span>

<span data-ttu-id="bc1aa-257">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bc1aa-257">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="bc1aa-258">関連項目</span><span class="sxs-lookup"><span data-stu-id="bc1aa-258">See also</span></span>

- [<span data-ttu-id="bc1aa-259">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="bc1aa-259">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="bc1aa-260">フォルダー内のメッセージへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="bc1aa-260">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mailfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
