---
title: 共有フォルダー内にある Outlook の連絡先を取得する
description: " 別名 "
ms.openlocfilehash: c8c5b3a2eac49153826113af036146cc4475d9e5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092404"
---
# <a name="get-outlook-contacts-in-a-shared-folder"></a><span data-ttu-id="acc92-103">共有フォルダー内にある Outlook の連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="acc92-103">Get Outlook contacts in a shared folder</span></span>

<span data-ttu-id="acc92-104">Outlook では、ユーザーがフォルダーを互いに共有し、個々の連絡先フォルダーに対する "読み取り"、"作成"、"変更"、"削除" のアクセス権を与えることができます。</span><span class="sxs-lookup"><span data-stu-id="acc92-104">Outlook lets customers share folders with one another and provide "read", "create", or "modify" access to individual folders or the entire mailbox.</span></span> <span data-ttu-id="acc92-105">また、Outlook では、あるユーザーが別のユーザーの代理人としてふるまい、ユーザーのメールボックス全体の中にある特定のフォルダーにアクセスすることもできます。これは Outlook では "委任" とも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="acc92-105">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="acc92-106">Microsoft Graph では、他のユーザーによって共有された連絡先フォルダーの連絡先を取得したり、共有フォルダー自体を取得したりする機能がプログラムとしてサポートされています。</span><span class="sxs-lookup"><span data-stu-id="acc92-106">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="acc92-107">また、委任メールボックスのフォルダーにもサポートが適用されます。</span><span class="sxs-lookup"><span data-stu-id="acc92-107">The support also applies to folders in a delegated mailbox.</span></span>

<span data-ttu-id="acc92-108">たとえば、Garth が John とカスタム連絡先フォルダーを共有し、John に読み取りアクセス権を与えたとします。</span><span class="sxs-lookup"><span data-stu-id="acc92-108">As an example, Garth has shared with John a custom contact folder and given John read access.</span></span> <span data-ttu-id="acc92-109">John がアプリにサインインし、委任されたアクセス許可 (Contacts.Read.Shared または Contacts.ReadWrite.Shared) を与えた場合、アプリでは、下記のようにして Garth のカスタム連絡先フォルダーと、そのフォルダー内にある連絡先にアクセスすることができます。</span><span class="sxs-lookup"><span data-stu-id="acc92-109">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-a-contact-in-the-shared-folder"></a><span data-ttu-id="acc92-110">共有フォルダー内の連絡先を取得</span><span class="sxs-lookup"><span data-stu-id="acc92-110">Get a message in the shared folder</span></span>

<span data-ttu-id="acc92-111">Garth が John と共有したカスタム連絡先フォルダーの特定の連絡先を取得できます。</span><span class="sxs-lookup"><span data-stu-id="acc92-111">You can get a specific contact in the custom contact folder that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

<span data-ttu-id="acc92-112">正常に終了すると、HTTP 200 OK となり、Garth の共有連絡先フォルダー`{id}`によって識別される[連絡先](/graph/api/resources/contact?view=graph-rest-1.0)インスタンスが取得されます。</span><span class="sxs-lookup"><span data-stu-id="acc92-112">On successful completion, you'll get HTTP 200 OK and the [message](/graph/api/resources/contact?view=graph-rest-1.0) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-contacts-in-the-shared-folder"></a><span data-ttu-id="acc92-113">共有フォルダー内の全連絡先を取得</span><span class="sxs-lookup"><span data-stu-id="acc92-113">Get all messages in the shared folder</span></span>

<span data-ttu-id="acc92-114">Garth の共有フォルダー内の全連絡先を取得します。</span><span class="sxs-lookup"><span data-stu-id="acc92-114">Get all the contacts in Garth's shared contact folder:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

<span data-ttu-id="acc92-115">正常に終了すると、HTTP 200 OK となり、Garth の共有連絡先フォルダーにある[連絡先](/graph/api/resources/contact?view=graph-rest-1.0)インスタンスのコレクションが取得されます。</span><span class="sxs-lookup"><span data-stu-id="acc92-115">On successful completion, you'll get HTTP 200 OK and a collection of [message](/graph/api/resources/contact?view=graph-rest-1.0) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="acc92-116">共有フォルダーを取得</span><span class="sxs-lookup"><span data-stu-id="acc92-116">Get the shared folder</span></span>

<span data-ttu-id="acc92-117">Garth が John と共有した連絡先フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="acc92-117">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

<span data-ttu-id="acc92-118">正常に終了すると、HTTP 200 OK となり、Garth の共有連絡先フォルダーを表す [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="acc92-118">On successful completion, you'll get HTTP 200 OK and a [mailFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="acc92-119">Garth が John に対して自分のメールボックス全体を John に委任していた場合も、同じ GET 機能が適用されます。</span><span class="sxs-lookup"><span data-stu-id="acc92-119">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="acc92-120">Garth が John と連絡先フォルダーを共有しておらず、自分のメールボックスを John に委任していない場合、それらの GET 操作に Garth のユーザー ID またはユーザー プリンシパル名を指定すると、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="acc92-120">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="acc92-121">次のステップ</span><span class="sxs-lookup"><span data-stu-id="acc92-121">Next steps</span></span>

<span data-ttu-id="acc92-122">詳細情報:</span><span class="sxs-lookup"><span data-stu-id="acc92-122">Find out more about:</span></span>

- [<span data-ttu-id="acc92-123">Outlook 個人用連絡先を統合する理由</span><span class="sxs-lookup"><span data-stu-id="acc92-123">Why integrate with Outlook personal contacts?</span></span>](outlook-contacts-concept-overview.md)
- <span data-ttu-id="acc92-124">Microsoft Graph v1.0 の[連絡先](/graph/api/resources/contact?view=graph-rest-1.0) API。</span><span class="sxs-lookup"><span data-stu-id="acc92-124">The [contacts API](/graph/api/resources/contact?view=graph-rest-1.0) in Microsoft Graph v1.0.</span></span>