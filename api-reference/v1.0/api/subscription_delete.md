# <a name="delete-subscription"></a><span data-ttu-id="5f2a4-101">サブスクリプションを削除する</span><span class="sxs-lookup"><span data-stu-id="5f2a4-101">Delete subscription</span></span>

<span data-ttu-id="5f2a4-102">サブスクリプションを削除します。</span><span class="sxs-lookup"><span data-stu-id="5f2a4-102">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f2a4-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5f2a4-103">Permissions</span></span>

<span data-ttu-id="5f2a4-p101">次の表に、各リソースに必要な、推奨されるアクセス許可を示します。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5f2a4-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="5f2a4-106">リソースの種類/項目</span><span class="sxs-lookup"><span data-stu-id="5f2a4-106">Resource type / Item</span></span>        | <span data-ttu-id="5f2a4-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5f2a4-107">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="5f2a4-108">連絡先</span><span class="sxs-lookup"><span data-stu-id="5f2a4-108">Contacts</span></span>                    | <span data-ttu-id="5f2a4-109">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5f2a4-109">Contacts.Read</span></span>       |
| <span data-ttu-id="5f2a4-110">スレッド</span><span class="sxs-lookup"><span data-stu-id="5f2a4-110">Conversations</span></span>               | <span data-ttu-id="5f2a4-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f2a4-111">Group.Read.All</span></span>      |
| <span data-ttu-id="5f2a4-112">イベント</span><span class="sxs-lookup"><span data-stu-id="5f2a4-112">Events</span></span>                      | <span data-ttu-id="5f2a4-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5f2a4-113">Calendars.Read</span></span>      |
| <span data-ttu-id="5f2a4-114">メッセージ</span><span class="sxs-lookup"><span data-stu-id="5f2a4-114">Messages</span></span>                    | <span data-ttu-id="5f2a4-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5f2a4-115">Mail.Read</span></span>           |
| <span data-ttu-id="5f2a4-116">ドライブ (ユーザーの OneDrive)</span><span class="sxs-lookup"><span data-stu-id="5f2a4-116">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="5f2a4-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f2a4-117">Files.ReadWrite</span></span>     |
| <span data-ttu-id="5f2a4-118">ドライブ (Sharepoint の共有コンテンツとドライブ)</span><span class="sxs-lookup"><span data-stu-id="5f2a4-118">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="5f2a4-119">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f2a4-119">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f2a4-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5f2a4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /subscriptions/{subscriptionId}
```
## <a name="request-headers"></a><span data-ttu-id="5f2a4-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5f2a4-121">Request headers</span></span>
| <span data-ttu-id="5f2a4-122">名前</span><span class="sxs-lookup"><span data-stu-id="5f2a4-122">Name</span></span>       | <span data-ttu-id="5f2a4-123">型</span><span class="sxs-lookup"><span data-stu-id="5f2a4-123">Type</span></span> | <span data-ttu-id="5f2a4-124">説明</span><span class="sxs-lookup"><span data-stu-id="5f2a4-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5f2a4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f2a4-125">Authorization</span></span>  | <span data-ttu-id="5f2a4-126">string</span><span class="sxs-lookup"><span data-stu-id="5f2a4-126">string</span></span>  | <span data-ttu-id="5f2a4-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5f2a4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f2a4-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="5f2a4-129">Request body</span></span>
<span data-ttu-id="5f2a4-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5f2a4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f2a4-131">応答</span><span class="sxs-lookup"><span data-stu-id="5f2a4-131">Response</span></span>

<span data-ttu-id="5f2a4-132">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="5f2a4-132">If successful, this method returns a `204 No Content` response code.</span></span>
## <a name="example"></a><span data-ttu-id="5f2a4-133">例</span><span class="sxs-lookup"><span data-stu-id="5f2a4-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5f2a4-134">要求</span><span class="sxs-lookup"><span data-stu-id="5f2a4-134">Request</span></span>
<span data-ttu-id="5f2a4-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5f2a4-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <a name="response"></a><span data-ttu-id="5f2a4-136">応答</span><span class="sxs-lookup"><span data-stu-id="5f2a4-136">Response</span></span>
<span data-ttu-id="5f2a4-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="5f2a4-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 204 No Content
```


<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
