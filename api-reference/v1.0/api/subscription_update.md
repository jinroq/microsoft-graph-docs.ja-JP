# <a name="update-subscription"></a><span data-ttu-id="69334-101">サブスクリプションを更新する</span><span class="sxs-lookup"><span data-stu-id="69334-101">Update subscription</span></span>

<span data-ttu-id="69334-102">サブスクリプションを更新するには、サブスクリプションの有効期限を延長します。</span><span class="sxs-lookup"><span data-stu-id="69334-102">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="69334-p101">リソースのサブスクリプションは、個々のリソースの種類で規定された日付になると有効期限が切れます。通知を見逃さないようにするため、有効期限よりも前にサブスクリプションを更新する必要があります。個々の有効期限の日付については、[サブスクリプション](../resources/subscription.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="69334-p101">Subscriptions to resources expire at dates proscribed by the individual resource types.  In order not to miss notifications, subscriptions should be renewed well in advance of their expiry date.  See [subscription](../resources/subscription.md) for individual expiry dates.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69334-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="69334-106">Prerequisites</span></span>

<span data-ttu-id="69334-107">次の表に、各リソースに必要な、推奨されるアクセス許可を示します。</span><span class="sxs-lookup"><span data-stu-id="69334-107">The following table lists the suggested permission needed for each resource.</span></span>

| <span data-ttu-id="69334-108">リソースの種類/項目</span><span class="sxs-lookup"><span data-stu-id="69334-108">Resource type / Item</span></span>        | <span data-ttu-id="69334-109">範囲</span><span class="sxs-lookup"><span data-stu-id="69334-109">Scope</span></span>               |
|-----------------------------|---------------------|
| <span data-ttu-id="69334-110">連絡先</span><span class="sxs-lookup"><span data-stu-id="69334-110">Contacts</span></span>                    | <span data-ttu-id="69334-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="69334-111">Contacts.Read</span></span>       |
| <span data-ttu-id="69334-112">スレッド</span><span class="sxs-lookup"><span data-stu-id="69334-112">Conversations</span></span>               | <span data-ttu-id="69334-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="69334-113">Group.Read.All</span></span>      |
| <span data-ttu-id="69334-114">イベント</span><span class="sxs-lookup"><span data-stu-id="69334-114">Events</span></span>                      | <span data-ttu-id="69334-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="69334-115">Calendars.Read</span></span>      |
| <span data-ttu-id="69334-116">メッセージ</span><span class="sxs-lookup"><span data-stu-id="69334-116">Messages</span></span>                    | <span data-ttu-id="69334-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="69334-117">Mail.Read</span></span>           |
| <span data-ttu-id="69334-118">ドライブ (ユーザーの OneDrive)</span><span class="sxs-lookup"><span data-stu-id="69334-118">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="69334-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69334-119">Files.ReadWrite</span></span>     |
| <span data-ttu-id="69334-120">ドライブ (Sharepoint の共有コンテンツとドライブ)</span><span class="sxs-lookup"><span data-stu-id="69334-120">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="69334-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69334-121">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="69334-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="69334-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /subscriptions/{subscriptionId}
```

## <a name="request-headers"></a><span data-ttu-id="69334-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="69334-123">Request headers</span></span>
| <span data-ttu-id="69334-124">名前</span><span class="sxs-lookup"><span data-stu-id="69334-124">Name</span></span>       | <span data-ttu-id="69334-125">型</span><span class="sxs-lookup"><span data-stu-id="69334-125">Type</span></span> | <span data-ttu-id="69334-126">説明</span><span class="sxs-lookup"><span data-stu-id="69334-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="69334-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="69334-127">Authorization</span></span>  | <span data-ttu-id="69334-128">string</span><span class="sxs-lookup"><span data-stu-id="69334-128">string</span></span>  | <span data-ttu-id="69334-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="69334-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="69334-131">応答</span><span class="sxs-lookup"><span data-stu-id="69334-131">Response</span></span>

<span data-ttu-id="69334-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscription](../resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="69334-132">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="69334-133">例</span><span class="sxs-lookup"><span data-stu-id="69334-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="69334-134">要求</span><span class="sxs-lookup"><span data-stu-id="69334-134">Request</span></span>
<span data-ttu-id="69334-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="69334-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a><span data-ttu-id="69334-136">応答</span><span class="sxs-lookup"><span data-stu-id="69334-136">Response</span></span>
<span data-ttu-id="69334-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="69334-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "changeType":"created,updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```


<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
