# <a name="get-outlook-contacts-in-a-shared-folder"></a><span data-ttu-id="d7779-101">共有フォルダーに Outlook の連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="d7779-101">Get Outlook contacts in a shared folder</span></span>

<span data-ttu-id="d7779-102">顧客は Outlook を使用してお互いにフォルダーを共有し、個々の連絡先フォルダーに、「読み取り」、「作成」、「変更」または「削除」のアクセス権を提供することができます。</span><span class="sxs-lookup"><span data-stu-id="d7779-102">Outlook lets customers share folders with one another and provide "read", "create", or "modify" access to individual folders or the entire mailbox.</span></span> <span data-ttu-id="d7779-103">また、Outlook では、別のユーザーが顧客の代理として操作を行い、特定のフォルダーまたは顧客のメールボックス全体にアクセスできるように委任することも、顧客に許可しています。これは、Outlook では「委任」とも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="d7779-103">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="d7779-104">プログラムにより、Microsoft Graph では他のユーザーが共有した連絡先フォルダー内の連絡先を取得したり、共有フォルダー自体を取得することをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="d7779-104">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="d7779-105">このサポートは、委任されたメールボックス内のフォルダーにも適用されます。</span><span class="sxs-lookup"><span data-stu-id="d7779-105">The support also applies to folders in a delegated mailbox.</span></span>

<span data-ttu-id="d7779-106">たとえば、Garth が John とカスタムの連絡先フォルダーを共有し、John に読み取りアクセス権を付与したとします。</span><span class="sxs-lookup"><span data-stu-id="d7779-106">As an example, Garth has shared with John a custom contact folder and given John read access.</span></span> <span data-ttu-id="d7779-107">ここで John がアプリにサインインし、任命を受けたアクセス許可 (Contacts.Read.Shared または Contacts.ReadWrite.Shared) を記述すれば、上記で説明したように、アプリで Garth のカスタム連絡先フォルダーとそのフォルダー内の連絡先にアクセスすることができます。</span><span class="sxs-lookup"><span data-stu-id="d7779-107">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-a-contact-in-the-shared-folder"></a><span data-ttu-id="d7779-108">共有フォルダー内の連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="d7779-108">Get a message in the shared folder</span></span>

<span data-ttu-id="d7779-109">Garth が John と共有したカスタムの連絡先フォルダー内の、特定の連絡先を取得することができます。</span><span class="sxs-lookup"><span data-stu-id="d7779-109">You can get a specific contact in the custom contact folder that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

<span data-ttu-id="d7779-110">正常に完了すれば、HTTP 200 OK と、 Garth [ の 共有連絡先フォルダーから ](../api-reference/v1.0/resources/contact.md) `{id}` によって識別された contact インスタンスが取得されます。</span><span class="sxs-lookup"><span data-stu-id="d7779-110">On successful completion, you'll get HTTP 200 OK and the [message](../api-reference/v1.0/resources/contact.md) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-contacts-in-the-shared-folder"></a><span data-ttu-id="d7779-111">共有フォルダー内のすべての連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="d7779-111">Get all messages in the shared folder</span></span>

<span data-ttu-id="d7779-112">Garth の共有連絡先フォルダー内のすべての連絡先を取得します。</span><span class="sxs-lookup"><span data-stu-id="d7779-112">Get all the contacts in Garth's shared contact folder:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

<span data-ttu-id="d7779-113">正常に完了すれば、HTTP 200 OK と、Garth の共有連絡先フォルダーの [contact](../api-reference/v1.0/resources/contact.md) インスタンスのコレクションが取得されます。</span><span class="sxs-lookup"><span data-stu-id="d7779-113">On successful completion, you'll get HTTP 200 OK and a collection of [message](../api-reference/v1.0/resources/contact.md) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="d7779-114">共有フォルダーを取得</span><span class="sxs-lookup"><span data-stu-id="d7779-114">Get the shared folder</span></span>

<span data-ttu-id="d7779-115">Garth が John と共有した連絡先フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="d7779-115">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

<span data-ttu-id="d7779-116">正常に完了すれば、HTTP 200 OK と、Garth の共有連絡先フォルダーを表す [contactFolder](../api-reference/v1.0/resources/contactfolder.md) インスタンスが取得されます。</span><span class="sxs-lookup"><span data-stu-id="d7779-116">On successful completion, you'll get HTTP 200 OK and a [mailFolder](../api-reference/v1.0/resources/contactfolder.md) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="d7779-117">Garth が John にメールボックス全体を委任していた場合には、同じ GET 機能が適用されます。</span><span class="sxs-lookup"><span data-stu-id="d7779-117">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="d7779-118">Garth が John と連絡先フォルダーを共有していない場合、または John にメールボックスを委任していない場合には、それらの GET 操作で Garth のユーザー ID またはユーザー プリンシパル名を指定すると、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="d7779-118">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="d7779-119">次の手順</span><span class="sxs-lookup"><span data-stu-id="d7779-119">Next steps</span></span>

<span data-ttu-id="d7779-120">詳細情報:</span><span class="sxs-lookup"><span data-stu-id="d7779-120">Find out more about:</span></span>

- [<span data-ttu-id="d7779-121">Outlook 個人用連絡先を統合する理由</span><span class="sxs-lookup"><span data-stu-id="d7779-121">Why integrate with Outlook personal contacts?</span></span>](outlook-contacts-concept-overview.md)
- <span data-ttu-id="d7779-122">Graph v1.0 の [連絡先 API](../api-reference/v1.0/resources/contact.md) です。</span><span class="sxs-lookup"><span data-stu-id="d7779-122">The [contacts API](../api-reference/v1.0/resources/contact.md) in Microsoft Graph v1.0.</span></span>