# <a name="delete-a-driveitem"></a><span data-ttu-id="6fa5d-101">DriveItem を削除する</span><span class="sxs-lookup"><span data-stu-id="6fa5d-101">Delete a DriveItem</span></span>

<span data-ttu-id="6fa5d-p101">[DriveItem](../resources/driveitem.md) を、ID またはパスを使用して削除します。このメソッドを使用して項目を削除すると、アイテムは完全に削除されず、ごみ箱に移動するだけであることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="6fa5d-p101">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="6fa5d-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6fa5d-104">Permissions</span></span>
<span data-ttu-id="6fa5d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6fa5d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6fa5d-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6fa5d-107">Permission type</span></span>      | <span data-ttu-id="6fa5d-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6fa5d-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6fa5d-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6fa5d-109">Delegated (work or school account)</span></span> | <span data-ttu-id="6fa5d-110">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fa5d-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6fa5d-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6fa5d-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fa5d-112">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fa5d-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="6fa5d-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6fa5d-113">Application</span></span> | <span data-ttu-id="6fa5d-114">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fa5d-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6fa5d-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6fa5d-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```
DELETE /me/drive/items/{item-id}
DELETE /me/drive/root:/{item-path}
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="6fa5d-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6fa5d-116">Request headers</span></span>

| <span data-ttu-id="6fa5d-117">名前</span><span class="sxs-lookup"><span data-stu-id="6fa5d-117">Name</span></span>          | <span data-ttu-id="6fa5d-118">型</span><span class="sxs-lookup"><span data-stu-id="6fa5d-118">Type</span></span>   | <span data-ttu-id="6fa5d-119">説明</span><span class="sxs-lookup"><span data-stu-id="6fa5d-119">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6fa5d-120">if-match</span><span class="sxs-lookup"><span data-stu-id="6fa5d-120">if-match</span></span>      | <span data-ttu-id="6fa5d-121">String</span><span class="sxs-lookup"><span data-stu-id="6fa5d-121">String</span></span> | <span data-ttu-id="6fa5d-122">この要求ヘッダーが含まれていて、指定された eTag (または cTag) が項目の現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、項目は削除されません。</span><span class="sxs-lookup"><span data-stu-id="6fa5d-122">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6fa5d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="6fa5d-123">Request body</span></span>
<span data-ttu-id="6fa5d-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6fa5d-124">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="6fa5d-125">例</span><span class="sxs-lookup"><span data-stu-id="6fa5d-125">Example</span></span>

<span data-ttu-id="6fa5d-126">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="6fa5d-126">Here is an example of how to call this API.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-item"
}-->
```
DELETE https://graph.microsoft.com/v1.0/me/drive/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="6fa5d-127">応答</span><span class="sxs-lookup"><span data-stu-id="6fa5d-127">Response</span></span>

<span data-ttu-id="6fa5d-128">成功した場合、この呼び出しはリソースが削除され返すものがなかったことを示す `204 No Content` 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="6fa5d-128">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

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
