# <a name="update-driveitem-properties"></a><span data-ttu-id="c88d2-101">DriveItem プロパティを更新する</span><span class="sxs-lookup"><span data-stu-id="c88d2-101">Update DriveItem properties</span></span>

<span data-ttu-id="c88d2-102">[DriveItem](../resources/driveitem.md) のメタデータを、ID またはパスで更新します。</span><span class="sxs-lookup"><span data-stu-id="c88d2-102">Update the metadata for a [DriveItem](../resources/driveitem.md) by ID or path.</span></span>

<span data-ttu-id="c88d2-103">別の親に[アイテムを移動](item_move.md)するために更新を使用することもできます。その場合は、アイテムの **parentReference** プロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c88d2-103">You can also use update to [move an item](item_move.md) to another parent by updating the item's **parentReference** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="c88d2-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c88d2-104">Permissions</span></span>
<span data-ttu-id="c88d2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c88d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c88d2-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c88d2-107">Permission type</span></span>      | <span data-ttu-id="c88d2-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c88d2-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c88d2-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c88d2-109">Delegated (work or school account)</span></span> | <span data-ttu-id="c88d2-110">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c88d2-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c88d2-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c88d2-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c88d2-112">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c88d2-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c88d2-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c88d2-113">Application</span></span> | <span data-ttu-id="c88d2-114">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c88d2-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c88d2-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c88d2-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{item-id}
PATCH /me/drive/root:/{item-path}
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="c88d2-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c88d2-116">Request headers</span></span>

| <span data-ttu-id="c88d2-117">名前</span><span class="sxs-lookup"><span data-stu-id="c88d2-117">Name</span></span>          | <span data-ttu-id="c88d2-118">型</span><span class="sxs-lookup"><span data-stu-id="c88d2-118">Type</span></span>   | <span data-ttu-id="c88d2-119">説明</span><span class="sxs-lookup"><span data-stu-id="c88d2-119">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c88d2-120">if-match</span><span class="sxs-lookup"><span data-stu-id="c88d2-120">if-match</span></span>      | <span data-ttu-id="c88d2-121">String</span><span class="sxs-lookup"><span data-stu-id="c88d2-121">String</span></span> | <span data-ttu-id="c88d2-122">この要求ヘッダーが含まれていて、指定された eTag (または cTag) がフォルダーの現在の eTag に一致しない場合には、`412 Precondition Failed` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="c88d2-122">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c88d2-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="c88d2-123">Request body</span></span>
<span data-ttu-id="c88d2-p102">要求本文で、更新すべきプロパティの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最高のパフォーマンスのためには、変更されていないプロパティをアプリケーションに含めないでください。</span><span class="sxs-lookup"><span data-stu-id="c88d2-p102">In the request body, supply the values for properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance your app should not include properties that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="c88d2-127">応答</span><span class="sxs-lookup"><span data-stu-id="c88d2-127">Response</span></span>

<span data-ttu-id="c88d2-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [DriveItem](../resources/driveitem.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="c88d2-128">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c88d2-129">例</span><span class="sxs-lookup"><span data-stu-id="c88d2-129">Example</span></span>
<span data-ttu-id="c88d2-130">この例では、driveItem の名前を変更します。</span><span class="sxs-lookup"><span data-stu-id="c88d2-130">This example renames the driveItem.</span></span>

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

##### <a name="response"></a><span data-ttu-id="c88d2-131">応答</span><span class="sxs-lookup"><span data-stu-id="c88d2-131">Response</span></span>

<span data-ttu-id="c88d2-p103">次の例は応答を示しています。この応答は、読みやすさのために切り詰められています。</span><span class="sxs-lookup"><span data-stu-id="c88d2-p103">The following example shows the response. This response is truncated for readability.</span></span>

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
