# <a name="share-outlook-message-folders-between-users"></a><span data-ttu-id="41df6-101">複数ユーザー間での Outlook メッセージ フォルダー共有</span><span class="sxs-lookup"><span data-stu-id="41df6-101">Share Outlook message folders between users</span></span>

<!-- remove similar content in other topics when ready to publish - list messages, get message, get mail folder.
These topics also have similar section - list events, get event, get calendar, list contacts, get contact, get contact folder.
-->

<span data-ttu-id="41df6-102">Outlook では、ユーザーがフォルダーを互いに共有し、個々のフォルダーやメールボックス全体に対する「読み取り」、「作成」、「変更」のアクセス権を提供することができます。</span><span class="sxs-lookup"><span data-stu-id="41df6-102">Outlook lets customers share folders with one another and provide "read", "create", or "modify" access to individual folders or the entire mailbox.</span></span> <span data-ttu-id="41df6-103">これは Outlook で「委任」とも呼ばれています。</span><span class="sxs-lookup"><span data-stu-id="41df6-103">This is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="41df6-104">Microsoft Graph では、他のユーザーと共有するメール フォルダーのメッセージを取得したり、共有フォルダー自体を取得したりする機能がプログラムとしてサポートされています。</span><span class="sxs-lookup"><span data-stu-id="41df6-104">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span>

<span data-ttu-id="41df6-105">たとえば、Garth が John と、Garth の受信トレイへの読み取りアクセスを共有したとします。</span><span class="sxs-lookup"><span data-stu-id="41df6-105">As an example, Garth has shared with John read access to Garth's Inbox.</span></span> <span data-ttu-id="41df6-106">John がアプリにサインインし、委任されたアクセス許可 (Mail.Read.Shared または Mail.ReadWrite.Shared) を提供した場合、アプリでは、下記のようにして Garth のメールおよび Garth の受信トレイにアクセスすることができます。</span><span class="sxs-lookup"><span data-stu-id="41df6-106">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-a-message-in-the-shared-folder"></a><span data-ttu-id="41df6-107">共有フォルダーのメッセージを取得</span><span class="sxs-lookup"><span data-stu-id="41df6-107">Get a message in the shared folder</span></span>

<span data-ttu-id="41df6-108">Garth の受信トレイの特定のメッセージを取得できます:</span><span class="sxs-lookup"><span data-stu-id="41df6-108">You can get a specific message in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

<span data-ttu-id="41df6-109">正常に終了した場合、HTTP 200 OK となり、Garth の受信トレイから `{id}` によって識別される[メッセージ](../api-reference/v1.0/resources/message.md) インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="41df6-109">On successful completion, you'll get HTTP 200 OK and the [message](../api-reference/v1.0/resources/message.md) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-messages-in-the-shared-folder"></a><span data-ttu-id="41df6-110">共有フォルダー内の全メッセージを取得</span><span class="sxs-lookup"><span data-stu-id="41df6-110">Get all messages in the shared folder</span></span>

<span data-ttu-id="41df6-111">Garth の受信トレイの全メッセージを取得:</span><span class="sxs-lookup"><span data-stu-id="41df6-111">Get all the messages in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

<span data-ttu-id="41df6-112">正常に終了すると、HTTP 200 OK となり、Garth の受信トレイの[メッセージ](../api-reference/v1.0/resources/message.md) インスタンスのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="41df6-112">On successful completion, you'll get HTTP 200 OK and a collection of [message](../api-reference/v1.0/resources/message.md) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="41df6-113">共有フォルダーを取得</span><span class="sxs-lookup"><span data-stu-id="41df6-113">Get the shared folder</span></span>

<span data-ttu-id="41df6-114">Garth が John と共有したフォルダー (受信トレイ) を取得します。</span><span class="sxs-lookup"><span data-stu-id="41df6-114">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

<span data-ttu-id="41df6-115">正常に終了すると、HTTP 200 OK となり、Garth の受信トレイ フォルダーを表す [mailFolder](../api-reference/v1.0/resources/mailfolder.md) インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="41df6-115">On successful completion, you'll get HTTP 200 OK and a [mailFolder](../api-reference/v1.0/resources/mailfolder.md) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="41df6-116">Garth が John に対して、Garth の受信トレイへのさらに多くのアクセス権を委任していた場合、または Garth が自分のメールボックス全体を John に委任していた場合も、同じ GET 機能が適用されます。</span><span class="sxs-lookup"><span data-stu-id="41df6-116">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="41df6-117">Garth が John とメッセージ フォルダーを共有していない、もしくはメールボックスを John に委任していない場合、それらの GET 操作に Garth のユーザー ID またはユーザー プリンシパル名を指定すると、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="41df6-117">If Garth has not shared his message folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="41df6-118">次の手順</span><span class="sxs-lookup"><span data-stu-id="41df6-118">Next steps</span></span>

<span data-ttu-id="41df6-119">詳細情報:</span><span class="sxs-lookup"><span data-stu-id="41df6-119">Find out more about deleting items</span></span>

- [<span data-ttu-id="41df6-120">Outlook メールと統合する理由</span><span class="sxs-lookup"><span data-stu-id="41df6-120">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="41df6-121">Microsoft Graph v1.0 の[メール API](../api-reference/v1.0/resources/mail_api_overview.md) とその[用途](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases)</span><span class="sxs-lookup"><span data-stu-id="41df6-121">[Using the mail API](../api-reference/v1.0/resources/mail_api_overview.md) and its [use cases](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) in Microsoft Graph v1.0.</span></span>