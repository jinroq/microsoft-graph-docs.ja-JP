---
title: 共有または委任されたフォルダー内の Outlook メッセージを取得する
description: Outlook では、ユーザーがメール フォルダーを互いに共有し、個々のフォルダーに対する読み取り、作成、変更、削除のアクセス権を与えることができます。 Outlook では、あるユーザーが、そのユーザーの代わりに操作する権限を別のユーザーに与えることもできます。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 76f54b5cc2db5395b9ca5e50611c4cea4f18b770
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917392"
---
# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a><span data-ttu-id="06ee9-104">共有または委任されたフォルダー内の Outlook メッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="06ee9-104">Get Outlook messages in a shared or delegated folder</span></span>

<span data-ttu-id="06ee9-105">Outlook では、ユーザーがメール フォルダーを互いに共有し、個々のフォルダーに対する "読み取り"、"作成"、"変更"、"削除" のアクセス権を与えることができます。</span><span class="sxs-lookup"><span data-stu-id="06ee9-105">Outlook lets customers share mail folders with one another and provide "read", "create", "modify", or "delete" access to individual folders.</span></span> <span data-ttu-id="06ee9-106">また、Outlook では、あるユーザーが別のユーザーの代理人としてふるまい、ユーザーのメールボックス全体の中にある特定のメール フォルダーにアクセスすることもできます。これは Outlook では "委任" とも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="06ee9-106">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific mail folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="06ee9-107">Microsoft Graph では、他のユーザーと共有するメール フォルダーのメッセージを取得したり、共有フォルダー自体を取得したりする機能がプログラムとしてサポートされています。</span><span class="sxs-lookup"><span data-stu-id="06ee9-107">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="06ee9-108">サポートは、委任されたフォルダーにも適用されます。</span><span class="sxs-lookup"><span data-stu-id="06ee9-108">The support also applies to folders that have been delegated.</span></span>

<span data-ttu-id="06ee9-109">たとえば、Garth が自分の受信トレイを John と共有し、読み取りアクセス権を与えたとします。</span><span class="sxs-lookup"><span data-stu-id="06ee9-109">As an example, Garth has shared with John and given read access to Garth's Inbox.</span></span> <span data-ttu-id="06ee9-110">John がアプリにサインインし、委任されたアクセス許可 (Mail.Read.Shared または Mail.ReadWrite.Shared) を与えた場合、アプリでは、下記のようにして Garth のメールおよび Garth の受信トレイにアクセスすることができます。</span><span class="sxs-lookup"><span data-stu-id="06ee9-110">If John has signed into your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

> <span data-ttu-id="06ee9-111">**注** 共有アクセス許可 (Mail.Read.Shared または Mail.ReadWrite.Shared) が与えられると、共有または委任されたフォルダーでメッセージを読み書きできます。</span><span class="sxs-lookup"><span data-stu-id="06ee9-111">**Note** The sharing permissions (Mail.Read.Shared or Mail.ReadWrite.Shared) allow you to read or write messages in a shared or delegated folder.</span></span> <span data-ttu-id="06ee9-112">そのようなフォルダーでアイテムの[変更通知をサブスクライブする](webhooks.md)ことはできません。</span><span class="sxs-lookup"><span data-stu-id="06ee9-112">They do not support [subscribing to change notifications](webhooks.md) on items in such folders.</span></span> <span data-ttu-id="06ee9-113">テナントで共有フォルダー、委任フォルダー、その他のユーザーのメール フォルダーに含まれているメッセージに変更通知サブスクリプションを設定するには、アプリケーション アクセス許可の Mail.Read を使用します。</span><span class="sxs-lookup"><span data-stu-id="06ee9-113">To set up change notification subscriptions on messages in a shared, delegated, or any other user's mail folder in the tenant, use the application permission, Mail.Read.</span></span>

## <a name="get-a-message-in-the-shared-folder"></a><span data-ttu-id="06ee9-114">共有フォルダーのメッセージを取得</span><span class="sxs-lookup"><span data-stu-id="06ee9-114">Get a message in the shared folder</span></span>

<span data-ttu-id="06ee9-115">Garth の受信トレイの特定のメッセージを取得できます:</span><span class="sxs-lookup"><span data-stu-id="06ee9-115">You can get a specific message in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

<span data-ttu-id="06ee9-116">正常に終了した場合、HTTP 200 OK となり、Garth の受信トレイから `{id}` によって識別される[メッセージ](/graph/api/resources/message?view=graph-rest-1.0) インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="06ee9-116">On successful completion, you'll get HTTP 200 OK and the [message](/graph/api/resources/message?view=graph-rest-1.0) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-messages-in-the-shared-folder"></a><span data-ttu-id="06ee9-117">共有フォルダー内の全メッセージを取得</span><span class="sxs-lookup"><span data-stu-id="06ee9-117">Get all messages in the shared folder</span></span>

<span data-ttu-id="06ee9-118">Garth の受信トレイの全メッセージを取得:</span><span class="sxs-lookup"><span data-stu-id="06ee9-118">Get all the messages in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

<span data-ttu-id="06ee9-119">正常に終了すると、HTTP 200 OK となり、Garth の受信トレイの[メッセージ](/graph/api/resources/message?view=graph-rest-1.0) インスタンスのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="06ee9-119">On successful completion, you'll get HTTP 200 OK and a collection of [message](/graph/api/resources/message?view=graph-rest-1.0) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="06ee9-120">共有フォルダーを取得</span><span class="sxs-lookup"><span data-stu-id="06ee9-120">Get the shared folder</span></span>

<span data-ttu-id="06ee9-121">Garth が John と共有したフォルダー (受信トレイ) を取得します。</span><span class="sxs-lookup"><span data-stu-id="06ee9-121">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

<span data-ttu-id="06ee9-122">正常に終了すると、HTTP 200 OK となり、Garth の受信トレイ フォルダーを表す [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="06ee9-122">On successful completion, you'll get HTTP 200 OK and a [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="06ee9-123">Garth が John に対して、Garth の受信トレイへのさらに多くのアクセス権を委任していた場合、または Garth が自分のメールボックス全体を John に委任していた場合も、同じ GET 機能が適用されます。</span><span class="sxs-lookup"><span data-stu-id="06ee9-123">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="06ee9-124">Garth が John と受信トレイを共有しておらず、メールボックスを John に委任していない場合、それらの GET 操作に Garth のユーザー ID またはユーザー プリンシパル名を指定すると、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="06ee9-124">If Garth has not shared his Inbox with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="06ee9-125">次のステップ</span><span class="sxs-lookup"><span data-stu-id="06ee9-125">Next steps</span></span>

<span data-ttu-id="06ee9-126">詳細情報:</span><span class="sxs-lookup"><span data-stu-id="06ee9-126">Find out more about:</span></span>

- [<span data-ttu-id="06ee9-127">Outlook メールと統合する理由</span><span class="sxs-lookup"><span data-stu-id="06ee9-127">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="06ee9-128">Microsoft Graph v1.0 の[メール API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) とその[用途](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases)</span><span class="sxs-lookup"><span data-stu-id="06ee9-128">[Using the mail API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) and its [use cases](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) in Microsoft Graph v1.0.</span></span>
