# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a><span data-ttu-id="62cd9-101">共有または委任されたフォルダー内の Outlook のメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="62cd9-101">Get Outlook messages in a shared or delegated folder</span></span>

<!-- remove similar content in other topics when ready to publish - list messages, get message, get mail folder.
These topics also have similar section - list events, get event, get calendar, list contacts, get contact, get contact folder.
-->

<span data-ttu-id="62cd9-102">顧客は Outlook を使用してお互いにメールフォルダーを共有し、個々のフォルダーに、「読み取り」、「作成」、「変更」または「削除」のアクセス権を提供することができます。</span><span class="sxs-lookup"><span data-stu-id="62cd9-102">Outlook lets customers share folders with one another and provide "read", "create", or "modify" access to individual folders or the entire mailbox.</span></span> <span data-ttu-id="62cd9-103">また、Outlook では、別のユーザーが顧客の代理として操作を行い、特定のメールフォルダーまたは顧客のメールボックス全体にアクセスできるように委任することも、顧客に許可しています。これは、Outlook では「委任」とも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="62cd9-103">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific mail folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="62cd9-104">Microsoft Graph では、他のユーザーと共有するメール フォルダーのメッセージを取得したり、共有フォルダー自体を取得したりする機能がプログラムとしてサポートされています。</span><span class="sxs-lookup"><span data-stu-id="62cd9-104">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="62cd9-105">サポートは、委任されたフォルダーにも適用されます。</span><span class="sxs-lookup"><span data-stu-id="62cd9-105">The support also applies to folders that have been delegated.</span></span>

<span data-ttu-id="62cd9-106">たとえば、Garth が John と、Garth の受信トレイへの読み取りアクセスを共有したとします。</span><span class="sxs-lookup"><span data-stu-id="62cd9-106">As an example, Garth has shared with John read access to Garth's Inbox.</span></span> <span data-ttu-id="62cd9-107">John がアプリにサインインし、委任されたアクセス許可 (Mail.Read.Shared または Mail.ReadWrite.Shared) を提供した場合、アプリでは、下記のようにして Garth のメールおよび Garth の受信トレイにアクセスすることができます。</span><span class="sxs-lookup"><span data-stu-id="62cd9-107">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-a-message-in-the-shared-folder"></a><span data-ttu-id="62cd9-108">共有フォルダー内のメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="62cd9-108">Get a message in the shared folder</span></span>

<span data-ttu-id="62cd9-109">Garth の受信トレイの特定のメッセージを取得できます:</span><span class="sxs-lookup"><span data-stu-id="62cd9-109">You can get a specific message in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

<span data-ttu-id="62cd9-110">正常に終了した場合、HTTP 200 OK となり、Garth の受信トレイから `{id}` によって識別される[メッセージ](../api-reference/v1.0/resources/message.md) インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="62cd9-110">On successful completion, you'll get HTTP 200 OK and the [message](../api-reference/v1.0/resources/message.md) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-messages-in-the-shared-folder"></a><span data-ttu-id="62cd9-111">共有フォルダー内の全メッセージを取得</span><span class="sxs-lookup"><span data-stu-id="62cd9-111">Get all messages in the shared folder</span></span>

<span data-ttu-id="62cd9-112">Garth の受信トレイの全メッセージを取得:</span><span class="sxs-lookup"><span data-stu-id="62cd9-112">Get all the messages in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

<span data-ttu-id="62cd9-113">正常に終了すると、HTTP 200 OK となり、Garth の受信トレイの[メッセージ](../api-reference/v1.0/resources/message.md) インスタンスのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="62cd9-113">On successful completion, you'll get HTTP 200 OK and a collection of [message](../api-reference/v1.0/resources/message.md) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="62cd9-114">共有フォルダーを取得</span><span class="sxs-lookup"><span data-stu-id="62cd9-114">Get the shared folder</span></span>

<span data-ttu-id="62cd9-115">Garth が John と共有したフォルダー (受信トレイ) を取得します。</span><span class="sxs-lookup"><span data-stu-id="62cd9-115">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

<span data-ttu-id="62cd9-116">正常に終了すると、HTTP 200 OK となり、Garth の受信トレイ フォルダーを表す [mailFolder](../api-reference/v1.0/resources/mailfolder.md) インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="62cd9-116">On successful completion, you'll get HTTP 200 OK and a [mailFolder](../api-reference/v1.0/resources/mailfolder.md) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="62cd9-117">Garth が John に対して、Garth の受信トレイへのさらに多くのアクセス権を委任していた場合、または Garth が自分のメールボックス全体を John に委任していた場合も、同じ GET 機能が適用されます。</span><span class="sxs-lookup"><span data-stu-id="62cd9-117">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="62cd9-118">Garth が John と受信トレイを共有していない、もしくはメールボックスを John に委任していない場合、それらの GET 操作に Garth のユーザー ID またはユーザー プリンシパル名を指定すると、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="62cd9-118">If Garth has not shared his message folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="62cd9-119">次の手順</span><span class="sxs-lookup"><span data-stu-id="62cd9-119">Next steps</span></span>

<span data-ttu-id="62cd9-120">詳細情報:</span><span class="sxs-lookup"><span data-stu-id="62cd9-120">Find out more about:</span></span>

- [<span data-ttu-id="62cd9-121">Outlook メールと統合する理由</span><span class="sxs-lookup"><span data-stu-id="62cd9-121">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="62cd9-122">Microsoft Graph v1.0 の[メール API](../api-reference/v1.0/resources/mail_api_overview.md) とその[用途](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases)</span><span class="sxs-lookup"><span data-stu-id="62cd9-122">[Using the mail API](../api-reference/v1.0/resources/mail_api_overview.md) and its [use cases](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) in Microsoft Graph v1.0.</span></span>