# <a name="move-a-driveitem"></a><span data-ttu-id="31cf6-101">DriveItem を移動する</span><span class="sxs-lookup"><span data-stu-id="31cf6-101">Move a DriveItem</span></span>

<span data-ttu-id="31cf6-p101">DriveItem を新しい親アイテムに移動する場合は、移動する DriveItem の **parentReference** をアプリで更新します。これは、[更新](item_update.md)メソッドの特殊なケースです。アプリでは、新しいコンテナーへのアイテムの移動と、アイテムの別のプロパティの更新を単一の要求に組み合わせることができます。</span><span class="sxs-lookup"><span data-stu-id="31cf6-p101">To move a DriveItem to a new parent item, your app requests to update the **parentReference** of the DriveItem to move. This is a special case of the [Update](item_update.md) method. Your app can combine moving an item to a new container and updating other properties of the item into a single request.</span></span>

<span data-ttu-id="31cf6-105">この要求を使用して、アイテムを[ドライブ](../resources/drive.md)間で移動することはできません。</span><span class="sxs-lookup"><span data-stu-id="31cf6-105">Items cannot be moved between [Drives](../resources/drive.md) using this request.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31cf6-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="31cf6-106">Prerequisites</span></span>
<span data-ttu-id="31cf6-107">この API を実行するには、以下のいずれかの**スコープ**が必要です。</span><span class="sxs-lookup"><span data-stu-id="31cf6-107">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="31cf6-108">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="31cf6-108">Files.ReadWrite</span></span>
* <span data-ttu-id="31cf6-109">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31cf6-109">Files.ReadWrite.All</span></span>
* <span data-ttu-id="31cf6-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31cf6-110">Sites.ReadWrite.All</span></span>


## <a name="http-request"></a><span data-ttu-id="31cf6-111">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="31cf6-111">HTTP request</span></span>

```http
PATCH /me/drive/items/{item-id}
PATCH /me/drive/root:/{item-path}
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="31cf6-112">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31cf6-112">Request headers</span></span>

| <span data-ttu-id="31cf6-113">名前</span><span class="sxs-lookup"><span data-stu-id="31cf6-113">Name</span></span>          | <span data-ttu-id="31cf6-114">型</span><span class="sxs-lookup"><span data-stu-id="31cf6-114">Type</span></span>   | <span data-ttu-id="31cf6-115">説明</span><span class="sxs-lookup"><span data-stu-id="31cf6-115">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="31cf6-116">if-match</span><span class="sxs-lookup"><span data-stu-id="31cf6-116">if-match</span></span>      | <span data-ttu-id="31cf6-117">String</span><span class="sxs-lookup"><span data-stu-id="31cf6-117">String</span></span> | <span data-ttu-id="31cf6-118">この要求ヘッダーが含まれていて、指定された eTag (または cTag) がフォルダーの現在の eTag に一致しない場合には、`412 Precondition Failed` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="31cf6-118">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |


## <a name="request-body"></a><span data-ttu-id="31cf6-119">要求本文</span><span class="sxs-lookup"><span data-stu-id="31cf6-119">Request body</span></span>
<span data-ttu-id="31cf6-p102">要求の本文内に、**parentReference** プロパティの新しい値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="31cf6-p102">In the request body, supply the new value for the **parentReference** property. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

<span data-ttu-id="31cf6-p103">**注:**OneDrive のルートにアイテムを移動するときには、`"id:" "root"` 構文は使用できません。ルート フォルダーの実際の ID を使用するか、親参照の `{"path": "/drive/root"}` を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="31cf6-p103">**Note:** When moving items to the root of a OneDrive you cannot use the `"id:" "root"` syntax. You either need to use the real ID of the root folder, or use `{"path": "/drive/root"}` for the parent reference.</span></span>

## <a name="response"></a><span data-ttu-id="31cf6-125">応答</span><span class="sxs-lookup"><span data-stu-id="31cf6-125">Response</span></span>

<span data-ttu-id="31cf6-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [DriveItem](../resources/driveitem.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="31cf6-126">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31cf6-127">例</span><span class="sxs-lookup"><span data-stu-id="31cf6-127">Example</span></span>
<span data-ttu-id="31cf6-128">この例では、{item-id} で指定したアイテムを、ユーザーの OneDrive の **Documents** フォルダーに移動します</span><span class="sxs-lookup"><span data-stu-id="31cf6-128">This example moves an item specified by {item-id} into the **Documents** folder in the user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_item"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{item-id}
Content-type: application/json

{
    "name": "new-item-name",
    "parentReference" : {"path": "/drive/root:/Documents"}
}
```

##### <a name="response"></a><span data-ttu-id="31cf6-129">応答</span><span class="sxs-lookup"><span data-stu-id="31cf6-129">Response</span></span>

<span data-ttu-id="31cf6-130">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="31cf6-130">The following example shows the response from the server with the search results.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "0123456789abc",
    "name": "new-item-name",
    "folder": { "childCount": 3 },
  "parentReference": {
    "id": "507DE6D5-0201-496A-AA87-5E2563247982",
    "path": "/drive/root:/Documents"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Move item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
