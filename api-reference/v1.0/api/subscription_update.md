# <a name="update-subscription"></a><span data-ttu-id="33603-101">サブスクリプションを更新する</span><span class="sxs-lookup"><span data-stu-id="33603-101">Update subscription</span></span>

<span data-ttu-id="33603-102">サブスクリプションを更新するには、サブスクリプションの有効期限を延長します。</span><span class="sxs-lookup"><span data-stu-id="33603-102">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="33603-p101">リソースのサブスクリプションは、個々のリソースの種類で規定された日付になると有効期限が切れます。通知を見逃さないようにするため、有効期限よりも前にサブスクリプションを更新する必要があります。個々の有効期限の日付については、[サブスクリプション](../resources/subscription.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="33603-p101">Subscriptions to resources expire at dates proscribed by the individual resource types.  In order not to miss notifications, subscriptions should be renewed well in advance of their expiry date.  See [subscription](../resources/subscription.md) for individual expiry dates.</span></span>

## <a name="permissions"></a><span data-ttu-id="33603-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="33603-106">Permissions</span></span>

<span data-ttu-id="33603-p102">次の表に、各リソースに必要な、推奨されるアクセス許可を示します。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="33603-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="33603-109">リソースの種類/項目</span><span class="sxs-lookup"><span data-stu-id="33603-109">Resource type / Item</span></span>        | <span data-ttu-id="33603-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="33603-110">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="33603-111">連絡先</span><span class="sxs-lookup"><span data-stu-id="33603-111">Contacts</span></span>                    | <span data-ttu-id="33603-112">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="33603-112">Contacts.Read</span></span>       |
| <span data-ttu-id="33603-113">スレッド</span><span class="sxs-lookup"><span data-stu-id="33603-113">Conversations</span></span>               | <span data-ttu-id="33603-114">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="33603-114">Group.Read.All</span></span>      |
| <span data-ttu-id="33603-115">イベント</span><span class="sxs-lookup"><span data-stu-id="33603-115">Events</span></span>                      | <span data-ttu-id="33603-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="33603-116">Calendars.Read</span></span>      |
| <span data-ttu-id="33603-117">メッセージ</span><span class="sxs-lookup"><span data-stu-id="33603-117">Messages</span></span>                    | <span data-ttu-id="33603-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="33603-118">Mail.Read</span></span>           |
| <span data-ttu-id="33603-119">ドライブ (ユーザーの OneDrive)</span><span class="sxs-lookup"><span data-stu-id="33603-119">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="33603-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33603-120">Files.ReadWrite</span></span>     |
| <span data-ttu-id="33603-121">ドライブ (Sharepoint の共有コンテンツとドライブ)</span><span class="sxs-lookup"><span data-stu-id="33603-121">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="33603-122">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33603-122">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33603-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="33603-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /subscriptions/{subscriptionId}
```

## <a name="request-headers"></a><span data-ttu-id="33603-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33603-124">Request headers</span></span>
| <span data-ttu-id="33603-125">名前</span><span class="sxs-lookup"><span data-stu-id="33603-125">Name</span></span>       | <span data-ttu-id="33603-126">型</span><span class="sxs-lookup"><span data-stu-id="33603-126">Type</span></span> | <span data-ttu-id="33603-127">説明</span><span class="sxs-lookup"><span data-stu-id="33603-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="33603-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="33603-128">Authorization</span></span>  | <span data-ttu-id="33603-129">string</span><span class="sxs-lookup"><span data-stu-id="33603-129">string</span></span>  | <span data-ttu-id="33603-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="33603-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="33603-132">応答</span><span class="sxs-lookup"><span data-stu-id="33603-132">Response</span></span>

<span data-ttu-id="33603-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscription](../resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="33603-133">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="33603-134">例</span><span class="sxs-lookup"><span data-stu-id="33603-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="33603-135">要求</span><span class="sxs-lookup"><span data-stu-id="33603-135">Request</span></span>
<span data-ttu-id="33603-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="33603-136">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="33603-137">応答</span><span class="sxs-lookup"><span data-stu-id="33603-137">Response</span></span>
<span data-ttu-id="33603-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="33603-138">Here is an example of the response.</span></span>
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
