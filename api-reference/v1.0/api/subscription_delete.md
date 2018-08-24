# <a name="delete-subscription"></a><span data-ttu-id="70d78-101">サブスクリプションを削除する</span><span class="sxs-lookup"><span data-stu-id="70d78-101">Delete subscription</span></span>

<span data-ttu-id="70d78-102">サブスクリプションを削除します。</span><span class="sxs-lookup"><span data-stu-id="70d78-102">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="70d78-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="70d78-103">Permissions</span></span>

<span data-ttu-id="70d78-p101">次の表に、各リソースに必要な、推奨されるアクセス許可を示します。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="70d78-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="70d78-106">リソースの種類/項目</span><span class="sxs-lookup"><span data-stu-id="70d78-106">Resource type / Item</span></span>        | <span data-ttu-id="70d78-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="70d78-107">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="70d78-108">連絡先</span><span class="sxs-lookup"><span data-stu-id="70d78-108">Contacts</span></span>                    | <span data-ttu-id="70d78-109">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="70d78-109">Contacts.Read</span></span>       |
| <span data-ttu-id="70d78-110">スレッド</span><span class="sxs-lookup"><span data-stu-id="70d78-110">Conversations</span></span>               | <span data-ttu-id="70d78-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="70d78-111">Group.Read.All</span></span>      |
| <span data-ttu-id="70d78-112">イベント</span><span class="sxs-lookup"><span data-stu-id="70d78-112">Events</span></span>                      | <span data-ttu-id="70d78-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="70d78-113">Calendars.Read</span></span>      |
| <span data-ttu-id="70d78-114">メッセージ</span><span class="sxs-lookup"><span data-stu-id="70d78-114">Messages</span></span>                    | <span data-ttu-id="70d78-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="70d78-115">Mail.Read</span></span>           |
| <span data-ttu-id="70d78-116">グループ</span><span class="sxs-lookup"><span data-stu-id="70d78-116">Groups</span></span>                      | <span data-ttu-id="70d78-117">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="70d78-117">Group.Read.All</span></span>      |
| <span data-ttu-id="70d78-118">ユーザー</span><span class="sxs-lookup"><span data-stu-id="70d78-118">Users</span></span>                       | <span data-ttu-id="70d78-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="70d78-119">User.Read.All</span></span>       |
| <span data-ttu-id="70d78-120">ドライブ (ユーザーの OneDrive)</span><span class="sxs-lookup"><span data-stu-id="70d78-120">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="70d78-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70d78-121">Files.ReadWrite</span></span>     |
| <span data-ttu-id="70d78-122">ドライブ (Sharepoint の共有コンテンツとドライブ)</span><span class="sxs-lookup"><span data-stu-id="70d78-122">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="70d78-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70d78-123">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70d78-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="70d78-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="70d78-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="70d78-125">Request headers</span></span>

| <span data-ttu-id="70d78-126">名前</span><span class="sxs-lookup"><span data-stu-id="70d78-126">Name</span></span>       | <span data-ttu-id="70d78-127">型</span><span class="sxs-lookup"><span data-stu-id="70d78-127">Type</span></span> | <span data-ttu-id="70d78-128">説明</span><span class="sxs-lookup"><span data-stu-id="70d78-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="70d78-129">承認</span><span class="sxs-lookup"><span data-stu-id="70d78-129">Authorization</span></span>  | <span data-ttu-id="70d78-130">文字列</span><span class="sxs-lookup"><span data-stu-id="70d78-130">string</span></span>  | <span data-ttu-id="70d78-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="70d78-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70d78-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="70d78-133">Request body</span></span>

<span data-ttu-id="70d78-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="70d78-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70d78-135">応答</span><span class="sxs-lookup"><span data-stu-id="70d78-135">Response</span></span>

<span data-ttu-id="70d78-136">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="70d78-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="70d78-137">例</span><span class="sxs-lookup"><span data-stu-id="70d78-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="70d78-138">要求</span><span class="sxs-lookup"><span data-stu-id="70d78-138">Request</span></span>

<span data-ttu-id="70d78-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="70d78-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="70d78-140">応答</span><span class="sxs-lookup"><span data-stu-id="70d78-140">Response</span></span>

<span data-ttu-id="70d78-141">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="70d78-141">Here is an example of the response.</span></span>
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
