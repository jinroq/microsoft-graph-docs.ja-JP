# <a name="delete-subscription"></a><span data-ttu-id="a85ed-101">サブスクリプションを削除する</span><span class="sxs-lookup"><span data-stu-id="a85ed-101">Delete subscription</span></span>

<span data-ttu-id="a85ed-102">サブスクリプションを削除します。</span><span class="sxs-lookup"><span data-stu-id="a85ed-102">Delete a subscription.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a85ed-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="a85ed-103">Prerequisites</span></span>

<span data-ttu-id="a85ed-104">次の表に、各リソースに必要な、推奨されるアクセス許可を示します。</span><span class="sxs-lookup"><span data-stu-id="a85ed-104">The following table lists the suggested permission needed for each resource.</span></span>

| <span data-ttu-id="a85ed-105">リソースの種類/項目</span><span class="sxs-lookup"><span data-stu-id="a85ed-105">Resource type / Item</span></span>        | <span data-ttu-id="a85ed-106">範囲</span><span class="sxs-lookup"><span data-stu-id="a85ed-106">Scope</span></span>               |
|-----------------------------|---------------------|
| <span data-ttu-id="a85ed-107">連絡先</span><span class="sxs-lookup"><span data-stu-id="a85ed-107">Contacts</span></span>                    | <span data-ttu-id="a85ed-108">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a85ed-108">Contacts.Read</span></span>       |
| <span data-ttu-id="a85ed-109">スレッド</span><span class="sxs-lookup"><span data-stu-id="a85ed-109">Conversations</span></span>               | <span data-ttu-id="a85ed-110">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a85ed-110">Group.Read.All</span></span>      |
| <span data-ttu-id="a85ed-111">イベント</span><span class="sxs-lookup"><span data-stu-id="a85ed-111">Events</span></span>                      | <span data-ttu-id="a85ed-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a85ed-112">Calendars.Read</span></span>      |
| <span data-ttu-id="a85ed-113">メッセージ</span><span class="sxs-lookup"><span data-stu-id="a85ed-113">Messages</span></span>                    | <span data-ttu-id="a85ed-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a85ed-114">Mail.Read</span></span>           |
| <span data-ttu-id="a85ed-115">ドライブ (ユーザーの OneDrive)</span><span class="sxs-lookup"><span data-stu-id="a85ed-115">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="a85ed-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a85ed-116">Files.ReadWrite</span></span>     |
| <span data-ttu-id="a85ed-117">ドライブ (Sharepoint の共有コンテンツとドライブ)</span><span class="sxs-lookup"><span data-stu-id="a85ed-117">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="a85ed-118">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a85ed-118">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a85ed-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a85ed-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /subscriptions/{subscriptionId}
```
## <a name="request-headers"></a><span data-ttu-id="a85ed-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a85ed-120">Request headers</span></span>
| <span data-ttu-id="a85ed-121">名前</span><span class="sxs-lookup"><span data-stu-id="a85ed-121">Name</span></span>       | <span data-ttu-id="a85ed-122">型</span><span class="sxs-lookup"><span data-stu-id="a85ed-122">Type</span></span> | <span data-ttu-id="a85ed-123">説明</span><span class="sxs-lookup"><span data-stu-id="a85ed-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a85ed-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a85ed-124">Authorization</span></span>  | <span data-ttu-id="a85ed-125">string</span><span class="sxs-lookup"><span data-stu-id="a85ed-125">string</span></span>  | <span data-ttu-id="a85ed-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a85ed-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a85ed-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="a85ed-128">Request body</span></span>
<span data-ttu-id="a85ed-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a85ed-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a85ed-130">応答</span><span class="sxs-lookup"><span data-stu-id="a85ed-130">Response</span></span>

<span data-ttu-id="a85ed-131">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="a85ed-131">If successful, this method returns a `204 No Content` response code.</span></span>
## <a name="example"></a><span data-ttu-id="a85ed-132">例</span><span class="sxs-lookup"><span data-stu-id="a85ed-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a85ed-133">要求</span><span class="sxs-lookup"><span data-stu-id="a85ed-133">Request</span></span>
<span data-ttu-id="a85ed-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a85ed-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <a name="response"></a><span data-ttu-id="a85ed-135">応答</span><span class="sxs-lookup"><span data-stu-id="a85ed-135">Response</span></span>
<span data-ttu-id="a85ed-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="a85ed-136">Here is an example of the response.</span></span>
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
