# <a name="get-a-driveitem-resource"></a><span data-ttu-id="234b0-101">DriveItem リソースを取得する</span><span class="sxs-lookup"><span data-stu-id="234b0-101">Get a DriveItem resource</span></span>

<span data-ttu-id="234b0-102">[ドライブ](../resources/drive.md) 内の [DriveItem](../resources/driveitem.md) 用のメタデータを、ファイル システム パスまたは ID で取得します。</span><span class="sxs-lookup"><span data-stu-id="234b0-102">Retrieve the metadata for a [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) by file system path or ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="234b0-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="234b0-103">Permissions</span></span>
<span data-ttu-id="234b0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="234b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="234b0-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="234b0-106">Permission type</span></span>      | <span data-ttu-id="234b0-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="234b0-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="234b0-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="234b0-108">Delegated (work or school account)</span></span> | <span data-ttu-id="234b0-109">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="234b0-109">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="234b0-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="234b0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="234b0-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="234b0-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="234b0-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="234b0-112">Application</span></span> | <span data-ttu-id="234b0-113">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="234b0-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="234b0-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="234b0-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{item-id}
GET /me/drive/root:/{item-path}
GET /drives/{drive-id}/items/{item-id}
GET /groups/{group-id}/drive/items/{item-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="234b0-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="234b0-115">Optional query parameters</span></span>
<span data-ttu-id="234b0-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="234b0-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="234b0-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="234b0-117">Request headers</span></span>

| <span data-ttu-id="234b0-118">名前</span><span class="sxs-lookup"><span data-stu-id="234b0-118">Name</span></span>          | <span data-ttu-id="234b0-119">値</span><span class="sxs-lookup"><span data-stu-id="234b0-119">Value</span></span>  | <span data-ttu-id="234b0-120">説明</span><span class="sxs-lookup"><span data-stu-id="234b0-120">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="234b0-121">if-none-match</span><span class="sxs-lookup"><span data-stu-id="234b0-121">if-none-match</span></span> | <span data-ttu-id="234b0-122">String</span><span class="sxs-lookup"><span data-stu-id="234b0-122">String</span></span> | <span data-ttu-id="234b0-123">この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="234b0-123">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |


## <a name="request-body"></a><span data-ttu-id="234b0-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="234b0-124">Request body</span></span>
<span data-ttu-id="234b0-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="234b0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="234b0-126">応答</span><span class="sxs-lookup"><span data-stu-id="234b0-126">Response</span></span>

<span data-ttu-id="234b0-127">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [DriveItem](../resources/driveitem.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="234b0-127">If successful, this method returns a `200 OK` response code and the [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="234b0-128">例</span><span class="sxs-lookup"><span data-stu-id="234b0-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="234b0-129">要求</span><span class="sxs-lookup"><span data-stu-id="234b0-129">Request</span></span>

<span data-ttu-id="234b0-130">以下は、ユーザーの OneDrive のルート フォルダーへの要求の例です。</span><span class="sxs-lookup"><span data-stu-id="234b0-130">Here is an example of the request to the root folder of the user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_item"
}-->
```
GET https://graph.microsoft.com/v1.0//me/drive/root
```

##### <a name="response"></a><span data-ttu-id="234b0-131">応答</span><span class="sxs-lookup"><span data-stu-id="234b0-131">Response</span></span>
<span data-ttu-id="234b0-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="234b0-132">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "createdBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "createdDateTime": "2016-03-21T20:01:37Z",
  "cTag": "\"c:{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},0\"",
  "eTag": "\"{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},1\"",
  "folder": { "childCount": 120 },
  "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
  "lastModifiedBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "lastModifiedDateTime": "2016-03-21T20:01:37Z",
  "name": "OneDrive",
  "root": { },
  "size": 157286400,
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents"
}
```

## <a name="notes"></a><span data-ttu-id="234b0-133">メモ</span><span class="sxs-lookup"><span data-stu-id="234b0-133">Notes</span></span>

<span data-ttu-id="234b0-134">アイテムが**子**関係にある場合、[`$expand` クエリ文字列パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) を使って、アイテムのメタデータを取得するのと同じように、同一呼び出し内のアイテムの子を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="234b0-134">You can use the [`$expand` query string parameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to include the children of an item in the same call as retrieving the metadata of an item if the item has a **children** relationship.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get item",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Get item"
}-->
