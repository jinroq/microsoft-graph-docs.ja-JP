---
title: 共有フォルダー内にある Outlook の連絡先を取得する
description: Outlook では、ユーザーがフォルダーを互いに共有し、個々の連絡先フォルダーに対する読み取り、作成、変更、削除のアクセス権を与えることができます。 Outlook では、あるユーザーが、そのユーザーの代わりに操作する権限を別のユーザーに与えることもできます。
author: angelgolfer-ms
ms.openlocfilehash: d0dc5be8df709c3d736ff0baa55667926cfc5936
ms.sourcegitcommit: 8feddb85e436be5581557a199f2e46d5b4ebfa21
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/22/2018
ms.locfileid: "27413156"
---
# <a name="get-outlook-contacts-in-a-shared-folder"></a><span data-ttu-id="a6f7d-104">共有フォルダー内にある Outlook の連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="a6f7d-104">Get Outlook contacts in a shared folder</span></span>

<span data-ttu-id="a6f7d-105">Outlook では、ユーザーがフォルダーを互いに共有し、個々の連絡先フォルダーに対する "読み取り"、"作成"、"変更"、"削除" のアクセス権を与えることができます。</span><span class="sxs-lookup"><span data-stu-id="a6f7d-105">Outlook lets customers share folders with one another and provide "read", "create", "modify", or "delete" access to individual contact folders.</span></span> <span data-ttu-id="a6f7d-106">また、Outlook では、あるユーザーが別のユーザーの代理人としてふるまい、ユーザーのメールボックス全体の中にある特定のフォルダーにアクセスすることもできます。これは Outlook では "委任" とも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="a6f7d-106">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="a6f7d-107">Microsoft Graph では、他のユーザーによって共有された連絡先フォルダーの連絡先を取得したり、共有フォルダー自体を取得したりする機能がプログラムとしてサポートされています。</span><span class="sxs-lookup"><span data-stu-id="a6f7d-107">Programmatically, Microsoft Graph supports getting contacts in contact folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="a6f7d-108">また、委任メールボックスのフォルダーにもサポートが適用されます。</span><span class="sxs-lookup"><span data-stu-id="a6f7d-108">The support also applies to folders in a delegated mailbox.</span></span>

<span data-ttu-id="a6f7d-109">たとえば、Garth が John とカスタム連絡先フォルダーを共有し、John に読み取りアクセス権を与えたとします。</span><span class="sxs-lookup"><span data-stu-id="a6f7d-109">As an example, Garth has shared with John a custom contact folder and given John read access.</span></span> <span data-ttu-id="a6f7d-110">John がアプリにサインインし、委任されたアクセス許可 (Contacts.Read.Shared または Contacts.ReadWrite.Shared) を与えた場合、アプリでは、下記のようにして Garth のカスタム連絡先フォルダーと、そのフォルダー内にある連絡先にアクセスすることができます。</span><span class="sxs-lookup"><span data-stu-id="a6f7d-110">If John has signed into your app and provided delegated permissions (Contacts.Read.Shared or Contacts.ReadWrite.Shared), your app will be able to access Garth's custom contact folder and contacts in that folder as described below.</span></span>

> <span data-ttu-id="a6f7d-111">**注** 共有アクセス許可 (Contacts.Read.Shared または Contacts.ReadWrite.Shared) が与えられると、共有または委任されたフォルダーで連絡先を読み書きできます。</span><span class="sxs-lookup"><span data-stu-id="a6f7d-111">**Note** The sharing permissions (Contacts.Read.Shared or Contacts.ReadWrite.Shared) allow you to read or write contacts in a shared or delegated folder.</span></span> <span data-ttu-id="a6f7d-112">そのようなフォルダーでアイテムの[変更通知をサブスクライブする](webhooks.md)ことはできません。</span><span class="sxs-lookup"><span data-stu-id="a6f7d-112">They do not support [subscribing to change notifications](webhooks.md) on items in such folders.</span></span> <span data-ttu-id="a6f7d-113">テナントで共有フォルダー、委任フォルダー、その他のユーザーの連絡先フォルダーに含まれている連絡先に変更通知サブスクリプションを設定するには、アプリケーション アクセス許可の Contacts.Read を使用します。</span><span class="sxs-lookup"><span data-stu-id="a6f7d-113">To set up change notification subscriptions on contacts in a shared, delegated, or any other user's contact folder in the tenant, use the application permission, Contacts.Read.</span></span>

## <a name="get-a-contact-in-the-shared-folder"></a><span data-ttu-id="a6f7d-114">共有フォルダー内の連絡先を取得</span><span class="sxs-lookup"><span data-stu-id="a6f7d-114">Get a contact in the shared folder</span></span>

<span data-ttu-id="a6f7d-115">Garth が John と共有したカスタム連絡先フォルダーの特定の連絡先を取得できます。</span><span class="sxs-lookup"><span data-stu-id="a6f7d-115">You can get a specific contact in the custom contact folder that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

<span data-ttu-id="a6f7d-116">正常に終了すると、HTTP 200 OK となり、Garth の共有連絡先フォルダー`{id}`によって識別される[連絡先](/graph/api/resources/contact?view=graph-rest-1.0)インスタンスが取得されます。</span><span class="sxs-lookup"><span data-stu-id="a6f7d-116">On successful completion, you'll get HTTP 200 OK and the [contact](/graph/api/resources/contact?view=graph-rest-1.0) instance identified by `{id}` from Garth's shared contact folder.</span></span>

## <a name="get-all-contacts-in-the-shared-folder"></a><span data-ttu-id="a6f7d-117">共有フォルダー内の全連絡先を取得</span><span class="sxs-lookup"><span data-stu-id="a6f7d-117">Get all contacts in the shared folder</span></span>

<span data-ttu-id="a6f7d-118">Garth の共有フォルダー内の全連絡先を取得します。</span><span class="sxs-lookup"><span data-stu-id="a6f7d-118">Get all the contacts in Garth's shared contact folder:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

<span data-ttu-id="a6f7d-119">正常に終了すると、HTTP 200 OK となり、Garth の共有連絡先フォルダーにある[連絡先](/graph/api/resources/contact?view=graph-rest-1.0)インスタンスのコレクションが取得されます。</span><span class="sxs-lookup"><span data-stu-id="a6f7d-119">On successful completion, you'll get HTTP 200 OK and a collection of [contact](/graph/api/resources/contact?view=graph-rest-1.0) instances in Garth's shared contact folder.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="a6f7d-120">共有フォルダーを取得</span><span class="sxs-lookup"><span data-stu-id="a6f7d-120">Get the shared folder</span></span>

<span data-ttu-id="a6f7d-121">Garth が John と共有した連絡先フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="a6f7d-121">Get the contact folder that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

<span data-ttu-id="a6f7d-122">正常に終了すると、HTTP 200 OK となり、Garth の共有連絡先フォルダーを表す [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="a6f7d-122">On successful completion, you'll get HTTP 200 OK and a [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) instance that represents Garth's shared contact folder.</span></span>

<span data-ttu-id="a6f7d-123">Garth が John に対して自分のメールボックス全体を John に委任していた場合も、同じ GET 機能が適用されます。</span><span class="sxs-lookup"><span data-stu-id="a6f7d-123">The same GET capabilities apply if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="a6f7d-124">Garth が John と連絡先フォルダーを共有しておらず、自分のメールボックスを John に委任していない場合、それらの GET 操作に Garth のユーザー ID またはユーザー プリンシパル名を指定すると、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="a6f7d-124">If Garth has not shared the contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="a6f7d-125">次のステップ</span><span class="sxs-lookup"><span data-stu-id="a6f7d-125">Next steps</span></span>

<span data-ttu-id="a6f7d-126">詳細情報:</span><span class="sxs-lookup"><span data-stu-id="a6f7d-126">Find out more about:</span></span>

- [<span data-ttu-id="a6f7d-127">Outlook 個人用連絡先を統合する理由</span><span class="sxs-lookup"><span data-stu-id="a6f7d-127">Why integrate with Outlook personal contacts</span></span>](outlook-contacts-concept-overview.md)
- <span data-ttu-id="a6f7d-128">Microsoft Graph v1.0 の[連絡先](/graph/api/resources/contact?view=graph-rest-1.0) API。</span><span class="sxs-lookup"><span data-stu-id="a6f7d-128">The [contacts API](/graph/api/resources/contact?view=graph-rest-1.0) in Microsoft Graph v1.0.</span></span>