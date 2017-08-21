# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="7e2c2-101">DriveItem のサムネイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7e2c2-101">List thumbnails for a DriveItem</span></span>

<span data-ttu-id="7e2c2-102">[DriveItem](../resources/driveitem.md) リソースの [ThumbnailSet](../resources/thumbnailset.md) リソースのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="7e2c2-102">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="7e2c2-p101">DriveItem はゼロ以上の [ThumbnailSet](../resources/thumbnailset.md) リソースで表すことができます。各 **thumbnailSet** は 1 つ以上の[**サムネイル**](../resources/thumbnail.md) オブジェクトを持つことができ、そのオブジェクトはアイテムを表すイメージです。たとえば、**thumbnailSet** には `small`、`medium`、`large` など、一般的な**サムネイル** オブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="7e2c2-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="7e2c2-p102">OneDrive 上でサムネイルを操作する方法はたくさんあります。次に、最も一般的なものを示します。</span><span class="sxs-lookup"><span data-stu-id="7e2c2-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="7e2c2-108">アイテムの利用可能なサムネイルを列挙する</span><span class="sxs-lookup"><span data-stu-id="7e2c2-108">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="7e2c2-109">アイテムの 1 つのサムネイルを取得する</span><span class="sxs-lookup"><span data-stu-id="7e2c2-109">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="7e2c2-110">サムネイルのコンテンツを取得する</span><span class="sxs-lookup"><span data-stu-id="7e2c2-110">Retrieve thumbnail content</span></span>
* <span data-ttu-id="7e2c2-111">1 つの要求で複数のアイテムのサムネイルを取得する</span><span class="sxs-lookup"><span data-stu-id="7e2c2-111">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="7e2c2-112">カスタムのサムネイル サイズを取得する</span><span class="sxs-lookup"><span data-stu-id="7e2c2-112">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="7e2c2-113">アイテムのカスタム サムネイルをアップロードする</span><span class="sxs-lookup"><span data-stu-id="7e2c2-113">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="7e2c2-114">カスタムのアップロード済みサムネイルが存在するかどうかを確認する</span><span class="sxs-lookup"><span data-stu-id="7e2c2-114">Determine if a custom uploaded thumbnail exists</span></span>


## <a name="prerequisites"></a><span data-ttu-id="7e2c2-115">前提条件</span><span class="sxs-lookup"><span data-stu-id="7e2c2-115">Prerequisites</span></span>
<span data-ttu-id="7e2c2-116">この API を実行するには、以下のいずれかの**スコープ**が必要です。</span><span class="sxs-lookup"><span data-stu-id="7e2c2-116">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="7e2c2-117">Files.Read</span><span class="sxs-lookup"><span data-stu-id="7e2c2-117">Files.Read</span></span>
* <span data-ttu-id="7e2c2-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7e2c2-118">Files.ReadWrite</span></span>
* <span data-ttu-id="7e2c2-119">Files.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e2c2-119">Files.Read.All</span></span>
* <span data-ttu-id="7e2c2-120">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e2c2-120">Files.ReadWrite.All</span></span>
* <span data-ttu-id="7e2c2-121">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e2c2-121">Sites.Read.All</span></span>
* <span data-ttu-id="7e2c2-122">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e2c2-122">Sites.ReadWrite.All</span></span>


## <a name="http-request"></a><span data-ttu-id="7e2c2-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7e2c2-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root:/{item-path}:/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7e2c2-124">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7e2c2-124">Optional query parameters</span></span>
<span data-ttu-id="7e2c2-125">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7e2c2-125">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="7e2c2-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7e2c2-126">Request body</span></span>
<span data-ttu-id="7e2c2-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7e2c2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e2c2-128">応答</span><span class="sxs-lookup"><span data-stu-id="7e2c2-128">Response</span></span>

<span data-ttu-id="7e2c2-129">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [ThumbnailSet](../resources/thumbnailset.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7e2c2-129">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e2c2-130">例</span><span class="sxs-lookup"><span data-stu-id="7e2c2-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7e2c2-131">要求</span><span class="sxs-lookup"><span data-stu-id="7e2c2-131">Request</span></span>

<span data-ttu-id="7e2c2-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7e2c2-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_thumbnails"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails
```


##### <a name="response"></a><span data-ttu-id="7e2c2-133">応答</span><span class="sxs-lookup"><span data-stu-id="7e2c2-133">Response</span></span>
<span data-ttu-id="7e2c2-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="7e2c2-134">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.thumbnailSet",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "0",
      "small": { "height": 64, "width": 96, "url": "https://sn3302files..."},
      "medium": { "height": 117, "width": 176, "url": "https://sn3302files..."},
      "large": { "height": 533, "width": 800, "url": "https://sn3302files..."}
    }
  ]
}
```

## <a name="retrieve-a-single-thumbnail"></a><span data-ttu-id="7e2c2-135">1 つのサムネイルを取得する</span><span class="sxs-lookup"><span data-stu-id="7e2c2-135">Retrieve a single thumbnail</span></span>

<span data-ttu-id="7e2c2-136">1 つのサムネイルとサイズのメタデータを、要求で直接識別することにより取得します。</span><span class="sxs-lookup"><span data-stu-id="7e2c2-136">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

## <a name="http-request"></a><span data-ttu-id="7e2c2-137">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7e2c2-137">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-one-thumbnail" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```

## <a name="path-parameters"></a><span data-ttu-id="7e2c2-138">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="7e2c2-138">Path parameters</span></span>

| <span data-ttu-id="7e2c2-139">名前</span><span class="sxs-lookup"><span data-stu-id="7e2c2-139">Name</span></span>         | <span data-ttu-id="7e2c2-140">型</span><span class="sxs-lookup"><span data-stu-id="7e2c2-140">Type</span></span>   | <span data-ttu-id="7e2c2-141">説明</span><span class="sxs-lookup"><span data-stu-id="7e2c2-141">Description</span></span>                                                                         |
|:-------------|:-------|:------------------------------------------------------------------------------------|
| <span data-ttu-id="7e2c2-142">**item-id**</span><span class="sxs-lookup"><span data-stu-id="7e2c2-142">**item-id**</span></span>  | <span data-ttu-id="7e2c2-143">string</span><span class="sxs-lookup"><span data-stu-id="7e2c2-143">string</span></span> | <span data-ttu-id="7e2c2-144">参照されるアイテムの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="7e2c2-144">The unique identifier for the item referenced.</span></span>                                      |
| <span data-ttu-id="7e2c2-145">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="7e2c2-145">**thumb-id**</span></span> | <span data-ttu-id="7e2c2-146">number</span><span class="sxs-lookup"><span data-stu-id="7e2c2-146">number</span></span> | <span data-ttu-id="7e2c2-147">サムネイルのインデックス (通常 0-4)。</span><span class="sxs-lookup"><span data-stu-id="7e2c2-147">The index of the thumbnail, usually 0-4.</span></span>                                            |
| <span data-ttu-id="7e2c2-148">**size**</span><span class="sxs-lookup"><span data-stu-id="7e2c2-148">**size**</span></span>     | <span data-ttu-id="7e2c2-149">string</span><span class="sxs-lookup"><span data-stu-id="7e2c2-149">string</span></span> | <span data-ttu-id="7e2c2-p103">要求されたサムネイルのサイズ。これは、リストされた標準的なサイズのいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="7e2c2-p103">The size of the thumbnail requested. This must be one of the standard sizes listed.</span></span> |


<!-- { "blockType": "response", "@odata.type": "microsoft.graph.thumbnail" } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "width": 100,
  "height": 100,
  "url": "http://onedrive.com/asd123a/asdjlkasjdkasdjlk.jpg"
}
```

## <a name="retrieve-thumbnail-content"></a><span data-ttu-id="7e2c2-152">サムネイルのコンテンツを取得する</span><span class="sxs-lookup"><span data-stu-id="7e2c2-152">Retrieve thumbnail content</span></span>

<span data-ttu-id="7e2c2-153">サムネイルの **content** プロパティを要求することにより、サムネイルのコンテンツを直接、取得できます。</span><span class="sxs-lookup"><span data-stu-id="7e2c2-153">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

## <a name="http-request"></a><span data-ttu-id="7e2c2-154">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7e2c2-154">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-content" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```

## <a name="response"></a><span data-ttu-id="7e2c2-155">応答</span><span class="sxs-lookup"><span data-stu-id="7e2c2-155">Response</span></span>

<span data-ttu-id="7e2c2-156">サービスは、サムネイルの URL へのリダイレクトで応答します。</span><span class="sxs-lookup"><span data-stu-id="7e2c2-156">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="7e2c2-p104">サムネイルのコンテンツ URL は事前認証されており、承認ヘッダーをダウンロードする必要はありません。これらの URL の存続時間は短く、数時間しか有効ではないため、アプリでキャッシュされません。</span><span class="sxs-lookup"><span data-stu-id="7e2c2-p104">Thumbnail content URLs are pre-authenticated and do not require an authorization header to be downloaded. These URLs are short lived and only valid for a few hours and should not be cached by apps.</span></span>


## <a name="size-values"></a><span data-ttu-id="7e2c2-159">サイズの値</span><span class="sxs-lookup"><span data-stu-id="7e2c2-159">Size values</span></span>

<span data-ttu-id="7e2c2-p105">次の表で、使用可能なサムネイルのサイズを定義します。サムネイルの任意のサイズを要求できますが、定義済みの値が存在する可能性が高く、値は即時に返されます。</span><span class="sxs-lookup"><span data-stu-id="7e2c2-p105">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="7e2c2-162">名前</span><span class="sxs-lookup"><span data-stu-id="7e2c2-162">Name</span></span>           | <span data-ttu-id="7e2c2-163">解像度</span><span class="sxs-lookup"><span data-stu-id="7e2c2-163">Resolution</span></span>  | <span data-ttu-id="7e2c2-164">縦横比</span><span class="sxs-lookup"><span data-stu-id="7e2c2-164">Aspect Ratio</span></span> | <span data-ttu-id="7e2c2-165">説明</span><span class="sxs-lookup"><span data-stu-id="7e2c2-165">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="7e2c2-166">96 longest</span><span class="sxs-lookup"><span data-stu-id="7e2c2-166">96 longest</span></span>  | <span data-ttu-id="7e2c2-167">Original</span><span class="sxs-lookup"><span data-stu-id="7e2c2-167">Original</span></span>     | <span data-ttu-id="7e2c2-168">圧縮率の高い小さなサムネイルは、正方形にトリミングされます。</span><span class="sxs-lookup"><span data-stu-id="7e2c2-168">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="7e2c2-169">176 longest</span><span class="sxs-lookup"><span data-stu-id="7e2c2-169">176 longest</span></span> | <span data-ttu-id="7e2c2-170">Original</span><span class="sxs-lookup"><span data-stu-id="7e2c2-170">Original</span></span>     | <span data-ttu-id="7e2c2-171">OneDrive の Web ビューの標準的なアイテムのサイズにトリミングされます。</span><span class="sxs-lookup"><span data-stu-id="7e2c2-171">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="7e2c2-172">800 longest</span><span class="sxs-lookup"><span data-stu-id="7e2c2-172">800 longest</span></span> | <span data-ttu-id="7e2c2-173">Original</span><span class="sxs-lookup"><span data-stu-id="7e2c2-173">Original</span></span>     | <span data-ttu-id="7e2c2-174">サムネイルの長辺が 800 ピクセルになるよう、サイズ変更されます。</span><span class="sxs-lookup"><span data-stu-id="7e2c2-174">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |

## <a name="remarks"></a><span data-ttu-id="7e2c2-175">注釈</span><span class="sxs-lookup"><span data-stu-id="7e2c2-175">Remarks</span></span>

<span data-ttu-id="7e2c2-176">**注:** OneDrive for Business および SharePoint の場合:</span><span class="sxs-lookup"><span data-stu-id="7e2c2-176">**Note** In OneDrive for Business and SharePoint:</span></span>

* <span data-ttu-id="7e2c2-177">次の呼び出しを使用したサムネイル コレクションの展開は機能しません: `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`</span><span class="sxs-lookup"><span data-stu-id="7e2c2-177">Using these calls to expand the thumbnails collection will not work: `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "OneDrive/Item/List thumbnails"
} -->
