---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ファイルまたはフォルダーのサムネイルを取得する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 20fd52d3436251e8047b56aec9ddf594d864783e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443988"
---
# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="934ed-102">DriveItem のサムネイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="934ed-102">List thumbnails for a DriveItem</span></span>

<span data-ttu-id="934ed-103">[DriveItem](../resources/driveitem.md) リソースの [ThumbnailSet](../resources/thumbnailset.md) リソースのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="934ed-103">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="934ed-p101">DriveItem はゼロ以上の [ThumbnailSet](../resources/thumbnailset.md) リソースで表すことができます。各 **thumbnailSet** は 1 つ以上の[**サムネイル**](../resources/thumbnail.md) オブジェクトを持つことができ、そのオブジェクトはアイテムを表すイメージです。たとえば、**thumbnailSet** には `small`、`medium`、`large` など、一般的な**サムネイル** オブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="934ed-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="934ed-p102">OneDrive 上でサムネイルを操作する方法はたくさんあります。次に、最も一般的なものを示します。</span><span class="sxs-lookup"><span data-stu-id="934ed-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="934ed-109">アイテムの利用可能なサムネイルを列挙する</span><span class="sxs-lookup"><span data-stu-id="934ed-109">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="934ed-110">アイテムの 1 つのサムネイルを取得する</span><span class="sxs-lookup"><span data-stu-id="934ed-110">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="934ed-111">サムネイルのコンテンツを取得する</span><span class="sxs-lookup"><span data-stu-id="934ed-111">Retrieve thumbnail content</span></span>
* <span data-ttu-id="934ed-112">1 つの要求で複数のアイテムのサムネイルを取得する</span><span class="sxs-lookup"><span data-stu-id="934ed-112">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="934ed-113">カスタムのサムネイル サイズを取得する</span><span class="sxs-lookup"><span data-stu-id="934ed-113">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="934ed-114">アイテムのカスタム サムネイルをアップロードする</span><span class="sxs-lookup"><span data-stu-id="934ed-114">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="934ed-115">カスタムのアップロード済みサムネイルが存在するかどうかを確認する</span><span class="sxs-lookup"><span data-stu-id="934ed-115">Determine if a custom uploaded thumbnail exists</span></span>

## <a name="permissions"></a><span data-ttu-id="934ed-116">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="934ed-116">Permissions</span></span>

<span data-ttu-id="934ed-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="934ed-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="934ed-119">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="934ed-119">Permission type</span></span>      | <span data-ttu-id="934ed-120">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="934ed-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="934ed-121">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="934ed-121">Delegated (work or school account)</span></span> | <span data-ttu-id="934ed-122">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="934ed-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="934ed-123">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="934ed-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="934ed-124">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="934ed-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="934ed-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="934ed-125">Application</span></span> | <span data-ttu-id="934ed-126">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="934ed-126">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="934ed-127">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="934ed-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="934ed-128">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="934ed-128">Optional query parameters</span></span>

<span data-ttu-id="934ed-129">このメソッドは、応答をカスタマイズするための `$select` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="934ed-129">This method supports the `$select` [OData puery parameter](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="934ed-130">応答</span><span class="sxs-lookup"><span data-stu-id="934ed-130">Response</span></span>

<span data-ttu-id="934ed-131">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [ThumbnailSet](../resources/thumbnailset.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="934ed-131">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="934ed-132">例</span><span class="sxs-lookup"><span data-stu-id="934ed-132">Example</span></span>

<span data-ttu-id="934ed-133">次は、現在のユーザーの OneDrive 内のアイテムで使用可能なサムネイルを取得する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="934ed-133">Here is an example of the request which retrieves available thumbnails for an item in the current user's OneDrive.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="934ed-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="934ed-134">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/thumbnails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="934ed-135">C#</span><span class="sxs-lookup"><span data-stu-id="934ed-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-item-thumbnails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="934ed-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="934ed-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-item-thumbnails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="934ed-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="934ed-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-item-thumbnails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="934ed-138">このアイテムの使用可能な **thumbnailSets** の配列が返されます。</span><span class="sxs-lookup"><span data-stu-id="934ed-138">This returns an array of available **thumbnailSets** for the item.</span></span> <span data-ttu-id="934ed-139">ドライブにあるすべてのアイテムは、0 個以上のサムネイルを保持できます。</span><span class="sxs-lookup"><span data-stu-id="934ed-139">Any item in a drive can have zero or more thumbnails.</span></span>

<span data-ttu-id="934ed-p105">**注:**_select_ クエリ文字列パラメーターを使用すると、**ThumbnailSet** で返されるサムネイルのサイズを制御できます。 たとえば、`/thumbnails?select=medium` では、中サイズのサムネイルのみを取得します。</span><span class="sxs-lookup"><span data-stu-id="934ed-p105">**Note:** You can use the _select_ query string parameter to control which thumbnail sizes are returned in the **ThumbnailSet**. For example, `/thumbnails?select=medium` retrieves only the medium sized thumbnails.</span></span>


### <a name="response"></a><span data-ttu-id="934ed-142">応答</span><span class="sxs-lookup"><span data-stu-id="934ed-142">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.thumbnailSet)" } -->

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

## <a name="get-a-single-thumbnail"></a><span data-ttu-id="934ed-143">1 つのサムネイルを取得する</span><span class="sxs-lookup"><span data-stu-id="934ed-143">Get a single thumbnail</span></span>

<span data-ttu-id="934ed-144">1 つのサムネイルとサイズのメタデータを、要求で直接アドレス指定して取得します。</span><span class="sxs-lookup"><span data-stu-id="934ed-144">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

### <a name="http-request"></a><span data-ttu-id="934ed-145">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="934ed-145">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="934ed-146">プロトコル</span><span class="sxs-lookup"><span data-stu-id="934ed-146">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="934ed-147">C#</span><span class="sxs-lookup"><span data-stu-id="934ed-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-one-thumbnail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="934ed-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="934ed-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-one-thumbnail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="934ed-149">目的-C</span><span class="sxs-lookup"><span data-stu-id="934ed-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-one-thumbnail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="934ed-150">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="934ed-150">Path parameters</span></span>

| <span data-ttu-id="934ed-151">名前</span><span class="sxs-lookup"><span data-stu-id="934ed-151">Name</span></span>         | <span data-ttu-id="934ed-152">型</span><span class="sxs-lookup"><span data-stu-id="934ed-152">Type</span></span>   | <span data-ttu-id="934ed-153">説明</span><span class="sxs-lookup"><span data-stu-id="934ed-153">Description</span></span>                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="934ed-154">**item-id**</span><span class="sxs-lookup"><span data-stu-id="934ed-154">**item-id**</span></span>  | <span data-ttu-id="934ed-155">string</span><span class="sxs-lookup"><span data-stu-id="934ed-155">string</span></span> | <span data-ttu-id="934ed-156">参照されるアイテムの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="934ed-156">The unique identifier for the item referenced.</span></span>                                           |
| <span data-ttu-id="934ed-157">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="934ed-157">**thumb-id**</span></span> | <span data-ttu-id="934ed-158">number</span><span class="sxs-lookup"><span data-stu-id="934ed-158">number</span></span> | <span data-ttu-id="934ed-p106">サムネイルのインデックス (通常 0-4)。 カスタム サムネイルがある場合は、そのインデックスは 0 になります。</span><span class="sxs-lookup"><span data-stu-id="934ed-p106">The index of the thumbnail, usually 0-4. If there is a custom thumbnail, its index is 0.</span></span> |
| <span data-ttu-id="934ed-161">**size**</span><span class="sxs-lookup"><span data-stu-id="934ed-161">**size**</span></span>     | <span data-ttu-id="934ed-162">string</span><span class="sxs-lookup"><span data-stu-id="934ed-162">string</span></span> | <span data-ttu-id="934ed-163">要求されたサムネイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="934ed-163">The size of the thumbnail requested.</span></span> <span data-ttu-id="934ed-164">これは、後述する標準サイズか、カスタム サイズのいずれかになります。</span><span class="sxs-lookup"><span data-stu-id="934ed-164">This can be one of the standard sizes listed below or a custom size.</span></span> |

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.thumbnail" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "width": 100,
  "height": 100,
  "url": "https://onedrive.com/asd123a/asdjlkasjdkasdjlk.jpg"
}
```

## <a name="retrieve-thumbnail-binary-content"></a><span data-ttu-id="934ed-165">サムネイルのバイナリ コンテンツを取得する</span><span class="sxs-lookup"><span data-stu-id="934ed-165">Retrieve thumbnail binary content</span></span>

<span data-ttu-id="934ed-166">サムネイルの **content** プロパティを要求することにより、サムネイルのコンテンツを直接取得できます。</span><span class="sxs-lookup"><span data-stu-id="934ed-166">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

### <a name="http-request"></a><span data-ttu-id="934ed-167">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="934ed-167">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="934ed-168">プロトコル</span><span class="sxs-lookup"><span data-stu-id="934ed-168">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="934ed-169">C#</span><span class="sxs-lookup"><span data-stu-id="934ed-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="934ed-170">Javascript</span><span class="sxs-lookup"><span data-stu-id="934ed-170">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="934ed-171">目的-C</span><span class="sxs-lookup"><span data-stu-id="934ed-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="934ed-172">応答</span><span class="sxs-lookup"><span data-stu-id="934ed-172">Response</span></span>

<span data-ttu-id="934ed-173">サービスは、サムネイルの URL へのリダイレクトで応答します。</span><span class="sxs-lookup"><span data-stu-id="934ed-173">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="934ed-174">サムネイル URL はキャッシュ対応です。</span><span class="sxs-lookup"><span data-stu-id="934ed-174">Thumbnail URLs are cache-safe.</span></span> <span data-ttu-id="934ed-175">この URL は、新しいサムネイルの生成を必要とする方法でアイテムを変更する場合に変更されます。</span><span class="sxs-lookup"><span data-stu-id="934ed-175">The URL will change, if the item changes in a way that requires a new thumbnail to be generated.</span></span>


## <a name="getting-thumbnails-while-listing-driveitems"></a><span data-ttu-id="934ed-176">DriveItems を一覧表示する際にサムネイルを取得する</span><span class="sxs-lookup"><span data-stu-id="934ed-176">Getting thumbnails while listing DriveItems</span></span>

<span data-ttu-id="934ed-177">表示する DriveItem リソースのリストを取得する場合、_$expand_ クエリ文字列パラメーターを使用して、それらのリソースのサムネイルも含めることができます。</span><span class="sxs-lookup"><span data-stu-id="934ed-177">If you are retrieving a list of DriveItem resources to display, you can use the _$expand_ query string parameter to also include the thumbnails for those resources.</span></span>
<span data-ttu-id="934ed-178">これによりアプリは、複数の要求を実行することなく、サムネイルとアイテムを 1 つの要求で取得することができます。</span><span class="sxs-lookup"><span data-stu-id="934ed-178">This enables your app to retrieve thumbnails and items in a single request, instead of issuing many requests.</span></span>

### <a name="http-request"></a><span data-ttu-id="934ed-179">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="934ed-179">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="934ed-180">プロトコル</span><span class="sxs-lookup"><span data-stu-id="934ed-180">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="934ed-181">C#</span><span class="sxs-lookup"><span data-stu-id="934ed-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-while-listing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="934ed-182">Javascript</span><span class="sxs-lookup"><span data-stu-id="934ed-182">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-while-listing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="934ed-183">目的-C</span><span class="sxs-lookup"><span data-stu-id="934ed-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-while-listing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="934ed-184">応答</span><span class="sxs-lookup"><span data-stu-id="934ed-184">Response</span></span>

<span data-ttu-id="934ed-185">サービスは、DriveItems とそのサムネイルのリストで応答します。</span><span class="sxs-lookup"><span data-stu-id="934ed-185">The service responses with the list of DriveItems and their thumbnails.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "182331E8-2788-4932-B52A-A6550577043F",
      "name": "my photo.jpg",
      "thumbnails": [
        {
          "small": { "width": 96,
                     "height": 96,
                     "url": "https://sn3302files..."
                   }
        }
      ]
    },
    {
      "id": "2D223953-A56B-4D9B-ADF3-13E7820673A2",
      "name": "presentation.pptx",
      "thumbnails": [
        {
          "small": { "width": 96,
                     "height": 96,
                     "url": "https://sn3302files..."
                   }
        }
      ]
    }
  ]
}
```

## <a name="size-options"></a><span data-ttu-id="934ed-186">サイズオプション</span><span class="sxs-lookup"><span data-stu-id="934ed-186">Size options</span></span>

<span data-ttu-id="934ed-p110">次の表で、使用可能なサムネイルのサイズを定義します。サムネイルの任意のサイズを要求できますが、定義済みの値が存在する可能性が高く、値は即時に返されます。</span><span class="sxs-lookup"><span data-stu-id="934ed-p110">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="934ed-189">名前</span><span class="sxs-lookup"><span data-stu-id="934ed-189">Name</span></span>           | <span data-ttu-id="934ed-190">解決策</span><span class="sxs-lookup"><span data-stu-id="934ed-190">Resolution</span></span>  | <span data-ttu-id="934ed-191">縦横比</span><span class="sxs-lookup"><span data-stu-id="934ed-191">Aspect Ratio</span></span> | <span data-ttu-id="934ed-192">説明</span><span class="sxs-lookup"><span data-stu-id="934ed-192">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="934ed-193">96 longest</span><span class="sxs-lookup"><span data-stu-id="934ed-193">96 longest</span></span>  | <span data-ttu-id="934ed-194">Original</span><span class="sxs-lookup"><span data-stu-id="934ed-194">Original</span></span>     | <span data-ttu-id="934ed-195">圧縮率の高い小さなサムネイルは、正方形にトリミングされます。</span><span class="sxs-lookup"><span data-stu-id="934ed-195">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="934ed-196">176 longest</span><span class="sxs-lookup"><span data-stu-id="934ed-196">176 longest</span></span> | <span data-ttu-id="934ed-197">Original</span><span class="sxs-lookup"><span data-stu-id="934ed-197">Original</span></span>     | <span data-ttu-id="934ed-198">OneDrive の Web ビューの標準的なアイテムのサイズにトリミングされます。</span><span class="sxs-lookup"><span data-stu-id="934ed-198">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="934ed-199">800 longest</span><span class="sxs-lookup"><span data-stu-id="934ed-199">800 longest</span></span> | <span data-ttu-id="934ed-200">元の比率</span><span class="sxs-lookup"><span data-stu-id="934ed-200">Original</span></span>     | <span data-ttu-id="934ed-201">サムネイルの長辺が 800 ピクセルになるよう、サイズ変更されます。</span><span class="sxs-lookup"><span data-stu-id="934ed-201">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |
| `smallSquare`  | <span data-ttu-id="934ed-202">96x96</span><span class="sxs-lookup"><span data-stu-id="934ed-202">96x96</span></span>       | <span data-ttu-id="934ed-203">正方形にトリミング</span><span class="sxs-lookup"><span data-stu-id="934ed-203">Square Crop</span></span>  | <span data-ttu-id="934ed-204">小さな正方形のサムネイル</span><span class="sxs-lookup"><span data-stu-id="934ed-204">Small square thumbnail</span></span>                                               |
| `mediumSquare` | <span data-ttu-id="934ed-205">176x176</span><span class="sxs-lookup"><span data-stu-id="934ed-205">176x176</span></span>     | <span data-ttu-id="934ed-206">正方形にトリミング</span><span class="sxs-lookup"><span data-stu-id="934ed-206">Square Crop</span></span>  | <span data-ttu-id="934ed-207">小さな正方形のサムネイル</span><span class="sxs-lookup"><span data-stu-id="934ed-207">Small square thumbnail</span></span>                                               |
| `largeSquare`  | <span data-ttu-id="934ed-208">800x800</span><span class="sxs-lookup"><span data-stu-id="934ed-208">800x800</span></span>     | <span data-ttu-id="934ed-209">正方形にトリミング</span><span class="sxs-lookup"><span data-stu-id="934ed-209">Square Crop</span></span>  | <span data-ttu-id="934ed-210">大きな正方形のサムネイル</span><span class="sxs-lookup"><span data-stu-id="934ed-210">Large square thumbnail</span></span>                                               |

## <a name="requesting-custom-thumbnail-sizes"></a><span data-ttu-id="934ed-211">カスタムのサムネイル サイズを要求する</span><span class="sxs-lookup"><span data-stu-id="934ed-211">Requesting custom thumbnail sizes</span></span>

<span data-ttu-id="934ed-212">定義済みのサイズに加えて、アプリでは、先頭に `c` を付けたサムネイルのディメンションを指定することで、カスタムのサムネイル サイズを要求できます。</span><span class="sxs-lookup"><span data-stu-id="934ed-212">In addition to the defined sizes, your app can request a custom thumbnail size by specifying the dimensions of the thumbnail prefixed with `c`.</span></span>
<span data-ttu-id="934ed-213">たとえば、アプリで 300x400 のサムネイルが必要な場合は、そのサイズを次に示すように要求できます。</span><span class="sxs-lookup"><span data-stu-id="934ed-213">For example if your app needs thumbnails that are 300x400, it can request that size like this:</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="934ed-214">プロトコル</span><span class="sxs-lookup"><span data-stu-id="934ed-214">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-thumbnail-custom-size", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_Crop
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="934ed-215">C#</span><span class="sxs-lookup"><span data-stu-id="934ed-215">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-custom-size-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="934ed-216">Javascript</span><span class="sxs-lookup"><span data-stu-id="934ed-216">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-custom-size-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="934ed-217">目的-C</span><span class="sxs-lookup"><span data-stu-id="934ed-217">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-custom-size-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="934ed-218">これにより、選択したカスタムのサムネイル サイズのみの応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="934ed-218">Which responds with just the custom thumbnail size selected:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.thumbnailSet)" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "0",
      "c300x400_Crop": { "height": 300, "width": 400, "url": "https://sn3302files.onedrive.com/123"},
    }
  ]
}
```

<span data-ttu-id="934ed-219">要求するサムネイルのサイズの後ろに、次に示すオプションを指定できます。</span><span class="sxs-lookup"><span data-stu-id="934ed-219">You can specify the following options after the size of the thumbnail requested:</span></span>

### <a name="examples-of-custom-identifiers"></a><span data-ttu-id="934ed-220">カスタム識別子の例</span><span class="sxs-lookup"><span data-stu-id="934ed-220">Examples of custom identifiers</span></span>

| <span data-ttu-id="934ed-221">サムネイル識別子</span><span class="sxs-lookup"><span data-stu-id="934ed-221">Thumbnail identifier</span></span> | <span data-ttu-id="934ed-222">解像度</span><span class="sxs-lookup"><span data-stu-id="934ed-222">Resolution</span></span>             | <span data-ttu-id="934ed-223">縦横比</span><span class="sxs-lookup"><span data-stu-id="934ed-223">Aspect ratio</span></span> | <span data-ttu-id="934ed-224">説明</span><span class="sxs-lookup"><span data-stu-id="934ed-224">Description</span></span>                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="934ed-225">c300x400</span><span class="sxs-lookup"><span data-stu-id="934ed-225">c300x400</span></span>             | <span data-ttu-id="934ed-226">300x400 のボックスに制限されます</span><span class="sxs-lookup"><span data-stu-id="934ed-226">Bounded by 300x400 box</span></span> | <span data-ttu-id="934ed-227">Original</span><span class="sxs-lookup"><span data-stu-id="934ed-227">Original</span></span>     | <span data-ttu-id="934ed-228">300x400 ピクセルのボックスに収まるサムネイルを生成します。縦横比は維持されます。</span><span class="sxs-lookup"><span data-stu-id="934ed-228">Generate a thumbnail that fits inside a 300x400 pixel box, maintaining aspect ratio</span></span>                                                                 |
| <span data-ttu-id="934ed-229">c300x400_Crop</span><span class="sxs-lookup"><span data-stu-id="934ed-229">c300x400_Crop</span></span>        | <span data-ttu-id="934ed-230">300x400</span><span class="sxs-lookup"><span data-stu-id="934ed-230">300x400</span></span>                | <span data-ttu-id="934ed-231">トリミング</span><span class="sxs-lookup"><span data-stu-id="934ed-231">Cropped</span></span>      | <span data-ttu-id="934ed-p112">300x400 ピクセルのサムネイルを生成します。 これは、300x400 のボックスに収まるように画像のサイズを変更し、このボックスに収まらない部分をトリミングするように動作します。</span><span class="sxs-lookup"><span data-stu-id="934ed-p112">Generate a thumbnail that is 300x400 pixels. This works by resizing the image to fill the 300x400 box and cropping whatever spills outside the box.</span></span> |

<span data-ttu-id="934ed-234">**注:** 返されるサムネイルのピクセル ディメンションは要求されたものと正確に一致しないことがありますが、縦横比は一致します。</span><span class="sxs-lookup"><span data-stu-id="934ed-234">**Note:** The thumbnail returned may not exactly match the pixel dimensions that was requested, but will match the aspect ratio.</span></span>
<span data-ttu-id="934ed-235">サムネイルがすでに存在しており、要求された解像度に簡単に拡大縮小できる場合、要求されたものよりも大きいサムネイルが返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="934ed-235">In some cases, a larger thumbnail may be returned than was requested, if the thumbnail already exists and can easily be scaled to match the requested resolution.</span></span>

## <a name="remarks"></a><span data-ttu-id="934ed-236">備考</span><span class="sxs-lookup"><span data-stu-id="934ed-236">Remarks</span></span>

<span data-ttu-id="934ed-237">**注:** OneDrive for Business および SharePoint の場合:</span><span class="sxs-lookup"><span data-stu-id="934ed-237">**Note** In OneDrive for Business and SharePoint:</span></span>

<span data-ttu-id="934ed-238">次の呼び出しを使用したサムネイル コレクションの展開は機能しません: </span><span class="sxs-lookup"><span data-stu-id="934ed-238">Using these calls to expand the thumbnails collection will not work:</span></span>

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

<span data-ttu-id="934ed-239">サムネイルは、SharePoint Server 2016 ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="934ed-239">Thumbnails are not supported on SharePoint Server 2016.</span></span>

### <a name="error-responses"></a><span data-ttu-id="934ed-240">エラー応答</span><span class="sxs-lookup"><span data-stu-id="934ed-240">Error responses</span></span>

<span data-ttu-id="934ed-241">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="934ed-241">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/api/driveitem-list-thumbnails.md:
      Unable to map some markdown elements into schema.
         Unmapped methods:
      enum-item-thumbnails, get-one-thumbnail, get-thumbnail-content, get-thumbnail-while-listing, get-thumbnail-custom-size
         Unmapped tables:
      Permissions - AuthScopes, Path parameters - PathParameters, Size options - Unknown, Examples of custom identifiers - Unknown",
    "Warning: Couldn't serialize request for path /me/drive/items/{var}/thumbnails/{var}/{var}/content into EDMX: System.InvalidOperationException: Uri path requires navigating into unknown object hierarchy: missing property '{var}' on 'thumbnailSet'. Possible issues:
         1) Doc bug where '{var}' isn't defined on the resource.         2) Doc bug where '{var}' is an example key and should instead be replaced with a placeholder like {item-id} or declared in the sampleKeys annotation.       3) Doc bug where 'thumbnailSet' is supposed to be an entity type, but is being treated as a complex because it (and its ancestors) are missing the keyProperty annotation
     at ApiDocs.Publishing.CSDL.CsdlWriter.ParseRequestTargetType(String requestPath, MethodCollection requestMethodCollection, EntityFramework edmx, IssueLogger issues) in D:/src/mds2/ApiDocs.Publishing/CSDL/CsdlWriter.cs:line 1145
     at ApiDocs.Publishing.CSDL.CsdlWriter.ProcessRestRequestPaths(EntityFramework edmx, String[] baseUrlsToRemove, IssueLogger issues) in D:/src/mds2/ApiDocs.Publishing/CSDL/CsdlWriter.cs:line 821"
  ],
  "tocPath": "Items/Thumbnails"
} -->
