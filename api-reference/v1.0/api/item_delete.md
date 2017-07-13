<span data-ttu-id="dd367-p101">[DriveItem](../resources/driveitem.md) を、ID またはパスを使用して削除します。このメソッドを使用して項目を削除すると、アイテムは完全に削除されず、ごみ箱に移動するだけであることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="dd367-p101">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

[DriveItem](../resources/driveitem.md) を、ID またはパスを使用して削除します。このメソッドを使用して項目を削除すると、アイテムは完全に削除されず、ごみ箱に移動するだけであることに注意してください。

## <span data-ttu-id="dd367-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="dd367-104">Prerequisites</span></span>
<a id="prerequisites" class="xliff"></a>
<span data-ttu-id="dd367-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。</span><span class="sxs-lookup"><span data-stu-id="dd367-105">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="dd367-106">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd367-106">Files.ReadWrite</span></span>
* <span data-ttu-id="dd367-107">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd367-107">Files.ReadWrite.All</span></span>
* <span data-ttu-id="dd367-108">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd367-108">Sites.ReadWrite.All</span></span>

## <span data-ttu-id="dd367-109">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dd367-109">HTTP request</span></span>
<a id="http-request" class="xliff"></a>

<!-- { "blockType": "ignored" } -->
```
DELETE /me/drive/items/{item-id}
DELETE /me/drive/root:/{item-path}
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
```

## <span data-ttu-id="dd367-110">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dd367-110">Request headers</span></span>
<a id="request-headers" class="xliff"></a>

| <span data-ttu-id="dd367-111">名前</span><span class="sxs-lookup"><span data-stu-id="dd367-111">Name</span></span>          | <span data-ttu-id="dd367-112">型</span><span class="sxs-lookup"><span data-stu-id="dd367-112">Type</span></span>   | <span data-ttu-id="dd367-113">説明</span><span class="sxs-lookup"><span data-stu-id="dd367-113">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="dd367-114">if-match</span><span class="sxs-lookup"><span data-stu-id="dd367-114">if-match</span></span>      | <span data-ttu-id="dd367-115">String</span><span class="sxs-lookup"><span data-stu-id="dd367-115">String</span></span> | <span data-ttu-id="dd367-116">この要求ヘッダーが含まれていて、指定された eTag (または cTag) が項目の現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、項目は削除されません。</span><span class="sxs-lookup"><span data-stu-id="dd367-116">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <span data-ttu-id="dd367-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="dd367-117">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="dd367-118">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dd367-118">Do not supply a request body for this method.</span></span>

## <span data-ttu-id="dd367-119">例</span><span class="sxs-lookup"><span data-stu-id="dd367-119">Example</span></span>
<a id="example" class="xliff"></a>

<span data-ttu-id="dd367-120">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="dd367-120">Here is an example of how to call this API.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-item"
}-->
```
DELETE https://graph.microsoft.com/v1.0/me/drive/items/{item-id}
```

## <span data-ttu-id="dd367-121">応答</span><span class="sxs-lookup"><span data-stu-id="dd367-121">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="dd367-122">成功した場合、この呼び出しはリソースが削除され返すものがなかったことを示す `204 No Content` 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="dd367-122">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete item",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Delete item"
}-->
