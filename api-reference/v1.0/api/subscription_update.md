# <a name="update-subscription"></a><span data-ttu-id="a72d0-101">サブスクリプションを更新する</span><span class="sxs-lookup"><span data-stu-id="a72d0-101">Update subscription</span></span>

<span data-ttu-id="a72d0-102">サブスクリプションを更新するには、サブスクリプションの有効期限を延長します。</span><span class="sxs-lookup"><span data-stu-id="a72d0-102">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="a72d0-103">サブスクリプションは、リソースの種類によって異なる期間後に期限が切れます。</span><span class="sxs-lookup"><span data-stu-id="a72d0-103">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="a72d0-104">通知の欠落を回避するには、アプリケーションは、その有効期限前にサブスクリプションを更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a72d0-104">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="a72d0-105">各リソースの種類のサブスクリプションの最大長については [サブスクリプション](../resources/subscription.md) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a72d0-105">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="a72d0-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a72d0-106">Permissions</span></span>

<span data-ttu-id="a72d0-p102">次の表に、各リソースに必要な、推奨されるアクセス許可を示します。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a72d0-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="a72d0-109">リソースの種類/項目</span><span class="sxs-lookup"><span data-stu-id="a72d0-109">Resource type / Item</span></span>        | <span data-ttu-id="a72d0-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a72d0-110">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="a72d0-111">連絡先</span><span class="sxs-lookup"><span data-stu-id="a72d0-111">Contacts</span></span>                    | <span data-ttu-id="a72d0-112">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a72d0-112">Contacts.Read</span></span>       |
| <span data-ttu-id="a72d0-113">スレッド</span><span class="sxs-lookup"><span data-stu-id="a72d0-113">Conversations</span></span>               | <span data-ttu-id="a72d0-114">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a72d0-114">Group.Read.All</span></span>      |
| <span data-ttu-id="a72d0-115">イベント</span><span class="sxs-lookup"><span data-stu-id="a72d0-115">Events</span></span>                      | <span data-ttu-id="a72d0-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a72d0-116">Calendars.Read</span></span>      |
| <span data-ttu-id="a72d0-117">メッセージ</span><span class="sxs-lookup"><span data-stu-id="a72d0-117">Messages</span></span>                    | <span data-ttu-id="a72d0-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a72d0-118">Mail.Read</span></span>           |
| <span data-ttu-id="a72d0-119">グループ</span><span class="sxs-lookup"><span data-stu-id="a72d0-119">Groups</span></span>                      | <span data-ttu-id="a72d0-120">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a72d0-120">Group.Read.All</span></span>      |
| <span data-ttu-id="a72d0-121">ユーザー</span><span class="sxs-lookup"><span data-stu-id="a72d0-121">Users</span></span>                       | <span data-ttu-id="a72d0-122">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a72d0-122">User.Read.All</span></span>       |
| <span data-ttu-id="a72d0-123">ドライブ (ユーザーの OneDrive)</span><span class="sxs-lookup"><span data-stu-id="a72d0-123">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="a72d0-124">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a72d0-124">Files.ReadWrite</span></span>     |
| <span data-ttu-id="a72d0-125">ドライブ (SharePoint の共有コンテンツとドライブ)</span><span class="sxs-lookup"><span data-stu-id="a72d0-125">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="a72d0-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a72d0-126">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a72d0-127">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a72d0-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a72d0-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a72d0-128">Request headers</span></span>

| <span data-ttu-id="a72d0-129">名前</span><span class="sxs-lookup"><span data-stu-id="a72d0-129">Name</span></span>       | <span data-ttu-id="a72d0-130">型</span><span class="sxs-lookup"><span data-stu-id="a72d0-130">Type</span></span> | <span data-ttu-id="a72d0-131">説明</span><span class="sxs-lookup"><span data-stu-id="a72d0-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a72d0-132">承認</span><span class="sxs-lookup"><span data-stu-id="a72d0-132">Authorization</span></span>  | <span data-ttu-id="a72d0-133">文字列</span><span class="sxs-lookup"><span data-stu-id="a72d0-133">string</span></span>  | <span data-ttu-id="a72d0-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a72d0-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a72d0-136">応答</span><span class="sxs-lookup"><span data-stu-id="a72d0-136">Response</span></span>

<span data-ttu-id="a72d0-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscription](../resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a72d0-137">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a72d0-138">例</span><span class="sxs-lookup"><span data-stu-id="a72d0-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a72d0-139">要求</span><span class="sxs-lookup"><span data-stu-id="a72d0-139">Request</span></span>

<span data-ttu-id="a72d0-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a72d0-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a><span data-ttu-id="a72d0-141">応答</span><span class="sxs-lookup"><span data-stu-id="a72d0-141">Response</span></span>

<span data-ttu-id="a72d0-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="a72d0-142">Here is an example of the response.</span></span>
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
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
