# <a name="delete-subscription"></a><span data-ttu-id="4fee7-101">サブスクリプションを削除する</span><span class="sxs-lookup"><span data-stu-id="4fee7-101">Delete subscription</span></span>

<span data-ttu-id="4fee7-102">サブスクリプションを削除します。</span><span class="sxs-lookup"><span data-stu-id="4fee7-102">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="4fee7-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4fee7-103">Permissions</span></span>

<span data-ttu-id="4fee7-p101">次の表に、各リソースに必要な、推奨されるアクセス許可を示します。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4fee7-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="4fee7-106">リソースの種類/項目</span><span class="sxs-lookup"><span data-stu-id="4fee7-106">Resource type / Item</span></span>        | <span data-ttu-id="4fee7-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4fee7-107">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="4fee7-108">連絡先</span><span class="sxs-lookup"><span data-stu-id="4fee7-108">Contacts</span></span>                    | <span data-ttu-id="4fee7-109">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="4fee7-109">Contacts.Read</span></span>       |
| <span data-ttu-id="4fee7-110">スレッド</span><span class="sxs-lookup"><span data-stu-id="4fee7-110">Conversations</span></span>               | <span data-ttu-id="4fee7-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fee7-111">Group.Read.All</span></span>      |
| <span data-ttu-id="4fee7-112">イベント</span><span class="sxs-lookup"><span data-stu-id="4fee7-112">Events</span></span>                      | <span data-ttu-id="4fee7-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4fee7-113">Calendars.Read</span></span>      |
| <span data-ttu-id="4fee7-114">メッセージ</span><span class="sxs-lookup"><span data-stu-id="4fee7-114">Messages</span></span>                    | <span data-ttu-id="4fee7-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4fee7-115">Mail.Read</span></span>           |
| <span data-ttu-id="4fee7-116">Groups</span><span class="sxs-lookup"><span data-stu-id="4fee7-116">Groups</span></span>                      | <span data-ttu-id="4fee7-117">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fee7-117">Group.Read.All</span></span>      |
| <span data-ttu-id="4fee7-118">Users</span><span class="sxs-lookup"><span data-stu-id="4fee7-118">Users</span></span>                       | <span data-ttu-id="4fee7-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fee7-119">User.Read.All</span></span>       |
| <span data-ttu-id="4fee7-120">ドライブ (ユーザーの OneDrive)</span><span class="sxs-lookup"><span data-stu-id="4fee7-120">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="4fee7-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4fee7-121">Files.ReadWrite</span></span>     |
| <span data-ttu-id="4fee7-122">ドライブ (共有、SharePoint コンテンツおよびドライブ)</span><span class="sxs-lookup"><span data-stu-id="4fee7-122">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="4fee7-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fee7-123">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="4fee7-124">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="4fee7-124">Security alert</span></span>| <span data-ttu-id="4fee7-125">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fee7-125">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4fee7-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4fee7-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4fee7-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4fee7-127">Request headers</span></span>

| <span data-ttu-id="4fee7-128">名前</span><span class="sxs-lookup"><span data-stu-id="4fee7-128">Name</span></span>       | <span data-ttu-id="4fee7-129">型</span><span class="sxs-lookup"><span data-stu-id="4fee7-129">Type</span></span> | <span data-ttu-id="4fee7-130">説明</span><span class="sxs-lookup"><span data-stu-id="4fee7-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4fee7-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fee7-131">Authorization</span></span>  | <span data-ttu-id="4fee7-132">string</span><span class="sxs-lookup"><span data-stu-id="4fee7-132">string</span></span>  | <span data-ttu-id="4fee7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4fee7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4fee7-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="4fee7-135">Request body</span></span>

<span data-ttu-id="4fee7-136">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4fee7-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4fee7-137">応答</span><span class="sxs-lookup"><span data-stu-id="4fee7-137">Response</span></span>

<span data-ttu-id="4fee7-138">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="4fee7-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4fee7-139">例</span><span class="sxs-lookup"><span data-stu-id="4fee7-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4fee7-140">要求</span><span class="sxs-lookup"><span data-stu-id="4fee7-140">Request</span></span>

<span data-ttu-id="4fee7-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4fee7-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="4fee7-142">応答</span><span class="sxs-lookup"><span data-stu-id="4fee7-142">Response</span></span>

<span data-ttu-id="4fee7-143">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="4fee7-143">Here is an example of the response.</span></span>
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
