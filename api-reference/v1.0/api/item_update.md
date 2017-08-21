# <a name="update-driveitem-properties"></a><span data-ttu-id="6f6f0-101">DriveItem プロパティを更新する</span><span class="sxs-lookup"><span data-stu-id="6f6f0-101">Update DriveItem properties</span></span>

<span data-ttu-id="6f6f0-102">[DriveItem](../resources/driveitem.md) のメタデータを、ID またはパスで更新します。</span><span class="sxs-lookup"><span data-stu-id="6f6f0-102">Update the metadata for a [DriveItem](../resources/driveitem.md) by ID or path.</span></span>

<span data-ttu-id="6f6f0-103">アイテムの **parentReference** プロパティを更新することで、他の親への [項目の移動](item_move.md) に更新を使うこともできます。</span><span class="sxs-lookup"><span data-stu-id="6f6f0-103">You can also use update to [move an item](item_move.md) to another parent by updating the item's **parentReference** property.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f6f0-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="6f6f0-104">Prerequisites</span></span>
<span data-ttu-id="6f6f0-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。</span><span class="sxs-lookup"><span data-stu-id="6f6f0-105">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="6f6f0-106">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6f6f0-106">Files.ReadWrite</span></span>
* <span data-ttu-id="6f6f0-107">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f6f0-107">Files.ReadWrite.All</span></span>
* <span data-ttu-id="6f6f0-108">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f6f0-108">Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="6f6f0-109">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6f6f0-109">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{item-id}
PATCH /me/drive/root:/{item-path}
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="6f6f0-110">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6f6f0-110">Request headers</span></span>

| <span data-ttu-id="6f6f0-111">名前</span><span class="sxs-lookup"><span data-stu-id="6f6f0-111">Name</span></span>          | <span data-ttu-id="6f6f0-112">型</span><span class="sxs-lookup"><span data-stu-id="6f6f0-112">Type</span></span>   | <span data-ttu-id="6f6f0-113">説明</span><span class="sxs-lookup"><span data-stu-id="6f6f0-113">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6f6f0-114">if-match</span><span class="sxs-lookup"><span data-stu-id="6f6f0-114">if-match</span></span>      | <span data-ttu-id="6f6f0-115">String</span><span class="sxs-lookup"><span data-stu-id="6f6f0-115">String</span></span> | <span data-ttu-id="6f6f0-116">この要求ヘッダーが含まれていて、指定された eTag (または cTag) がフォルダーの現在の eTag に一致しない場合には、`412 Precondition Failed` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="6f6f0-116">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f6f0-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="6f6f0-117">Request body</span></span>
<span data-ttu-id="6f6f0-p101">要求本文で、更新すべきプロパティの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最高のパフォーマンスのためには、変更されていないプロパティをアプリケーションに含めないでください。</span><span class="sxs-lookup"><span data-stu-id="6f6f0-p101">In the request body, supply the values for properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance your app should not include properties that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="6f6f0-121">応答</span><span class="sxs-lookup"><span data-stu-id="6f6f0-121">Response</span></span>

<span data-ttu-id="6f6f0-122">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [DriveItem](../resources/driveitem.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="6f6f0-122">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f6f0-123">例</span><span class="sxs-lookup"><span data-stu-id="6f6f0-123">Example</span></span>
<span data-ttu-id="6f6f0-124">この例では、driveItem の名前を変更します。</span><span class="sxs-lookup"><span data-stu-id="6f6f0-124">This example renames the driveItem.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_item"
}-->
```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
    "name": "new-file-name.docx"
}
```

##### <a name="response"></a><span data-ttu-id="6f6f0-125">応答</span><span class="sxs-lookup"><span data-stu-id="6f6f0-125">Response</span></span>

<span data-ttu-id="6f6f0-p102">次の例は応答を示しています。この応答は、読みやすさのために切り詰められています。</span><span class="sxs-lookup"><span data-stu-id="6f6f0-p102">The following example shows the response. This response is truncated for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
    "name": "new-file-name.docx",
    "file": { }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update item",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update item"
}-->
