---
title: 共有または委任されたフォルダー内の Outlook メッセージを取得する
description: イベントの一覧表示、イベントの取得、予定表の取得、連絡先の一覧表示、連絡先の取得、連絡先フォルダーの各トピックにも、同様のセクションがあります。
ms.openlocfilehash: d9e04527879cb32f14dc8d74a814a54150c5b2d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092454"
---
# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a><span data-ttu-id="90b7d-103">共有または委任されたフォルダー内の Outlook メッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="90b7d-103">Get Outlook messages in a shared or delegated folder</span></span>

<!-- remove similar content in other topics when ready to publish - list messages, get message, get mail folder.
These topics also have similar section - list events, get event, get calendar, list contacts, get contact, get contact folder.
-->

<span data-ttu-id="90b7d-104">Outlook では、ユーザーがメール フォルダーを互いに共有し、個々のフォルダーに対する "読み取り"、"作成"、"変更"、"削除" のアクセス権を与えることができます。</span><span class="sxs-lookup"><span data-stu-id="90b7d-104">Outlook lets customers share folders with one another and provide "read", "create", or "modify" access to individual folders or the entire mailbox.</span></span> <span data-ttu-id="90b7d-105">また、Outlook では、あるユーザーが別のユーザーの代理人としてふるまい、ユーザーのメールボックス全体の中にある特定のメール フォルダーにアクセスすることもできます。これは Outlook では "委任" とも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="90b7d-105">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific mail folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="90b7d-106">Microsoft Graph では、他のユーザーと共有するメール フォルダーのメッセージを取得したり、共有フォルダー自体を取得したりする機能がプログラムとしてサポートされています。</span><span class="sxs-lookup"><span data-stu-id="90b7d-106">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="90b7d-107">サポートは、委任されたフォルダーにも適用されます。</span><span class="sxs-lookup"><span data-stu-id="90b7d-107">The support also applies to folders that have been delegated.</span></span>

<span data-ttu-id="90b7d-108">たとえば、Garth が自分の受信トレイを John と共有し、読み取りアクセス権を与えたとします。</span><span class="sxs-lookup"><span data-stu-id="90b7d-108">As an example, Garth has shared with John read access to Garth's Inbox.</span></span> <span data-ttu-id="90b7d-109">John がアプリにサインインし、委任されたアクセス許可 (Mail.Read.Shared または Mail.ReadWrite.Shared) を与えた場合、アプリでは、下記のようにして Garth のメールおよび Garth の受信トレイにアクセスすることができます。</span><span class="sxs-lookup"><span data-stu-id="90b7d-109">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-a-message-in-the-shared-folder"></a><span data-ttu-id="90b7d-110">共有フォルダーのメッセージを取得</span><span class="sxs-lookup"><span data-stu-id="90b7d-110">Get a message in the shared folder</span></span>

<span data-ttu-id="90b7d-111">Garth の受信トレイの特定のメッセージを取得できます:</span><span class="sxs-lookup"><span data-stu-id="90b7d-111">You can get a specific message in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

<span data-ttu-id="90b7d-112">正常に終了した場合、HTTP 200 OK となり、Garth の受信トレイから `{id}` によって識別される[メッセージ](/graph/api/resources/message?view=graph-rest-1.0) インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="90b7d-112">On successful completion, you'll get HTTP 200 OK and the [message](/graph/api/resources/message?view=graph-rest-1.0) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-messages-in-the-shared-folder"></a><span data-ttu-id="90b7d-113">共有フォルダー内の全メッセージを取得</span><span class="sxs-lookup"><span data-stu-id="90b7d-113">Get all messages in the shared folder</span></span>

<span data-ttu-id="90b7d-114">Garth の受信トレイの全メッセージを取得:</span><span class="sxs-lookup"><span data-stu-id="90b7d-114">Get all the messages in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

<span data-ttu-id="90b7d-115">正常に終了すると、HTTP 200 OK となり、Garth の受信トレイの[メッセージ](/graph/api/resources/message?view=graph-rest-1.0) インスタンスのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="90b7d-115">On successful completion, you'll get HTTP 200 OK and a collection of [message](/graph/api/resources/message?view=graph-rest-1.0) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="90b7d-116">共有フォルダーを取得</span><span class="sxs-lookup"><span data-stu-id="90b7d-116">Get the shared folder</span></span>

<span data-ttu-id="90b7d-117">Garth が John と共有したフォルダー (受信トレイ) を取得します。</span><span class="sxs-lookup"><span data-stu-id="90b7d-117">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

<span data-ttu-id="90b7d-118">正常に終了すると、HTTP 200 OK となり、Garth の受信トレイ フォルダーを表す [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="90b7d-118">On successful completion, you'll get HTTP 200 OK and a [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="90b7d-119">Garth が John に対して、Garth の受信トレイへのさらに多くのアクセス権を委任していた場合、または Garth が自分のメールボックス全体を John に委任していた場合も、同じ GET 機能が適用されます。</span><span class="sxs-lookup"><span data-stu-id="90b7d-119">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="90b7d-120">Garth が John と受信トレイを共有しておらず、メールボックスを John に委任していない場合、それらの GET 操作に Garth のユーザー ID またはユーザー プリンシパル名を指定すると、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="90b7d-120">If Garth has not shared his message folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="90b7d-121">次のステップ</span><span class="sxs-lookup"><span data-stu-id="90b7d-121">Next steps</span></span>

<span data-ttu-id="90b7d-122">詳細情報:</span><span class="sxs-lookup"><span data-stu-id="90b7d-122">Find out more about:</span></span>

- [<span data-ttu-id="90b7d-123">Outlook メールと統合する理由</span><span class="sxs-lookup"><span data-stu-id="90b7d-123">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="90b7d-124">Microsoft Graph v1.0 の[メール API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) とその[用途](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases)</span><span class="sxs-lookup"><span data-stu-id="90b7d-124">[Using the mail API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) and its [use cases](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) in Microsoft Graph v1.0.</span></span>