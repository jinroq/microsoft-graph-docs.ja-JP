---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ファイルまたはフォルダーのサムネイルを取得する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e220caed7a745caf7f75935ed9b47eb415173135
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33590035"
---
# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="41805-102">DriveItem のサムネイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="41805-102">List thumbnails for a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41805-103">[DriveItem](../resources/driveitem.md) リソースの [ThumbnailSet](../resources/thumbnailset.md) リソースのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="41805-103">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="41805-p101">DriveItem はゼロ以上の [ThumbnailSet](../resources/thumbnailset.md) リソースで表すことができます。各 **thumbnailSet** は 1 つ以上の[**サムネイル**](../resources/thumbnail.md) オブジェクトを持つことができ、そのオブジェクトはアイテムを表すイメージです。たとえば、**thumbnailSet** には `small`、`medium`、`large` など、一般的な**サムネイル** オブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="41805-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="41805-p102">OneDrive 上でサムネイルを操作する方法はたくさんあります。次に、最も一般的なものを示します。</span><span class="sxs-lookup"><span data-stu-id="41805-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="41805-109">アイテムの利用可能なサムネイルを列挙する</span><span class="sxs-lookup"><span data-stu-id="41805-109">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="41805-110">アイテムの 1 つのサムネイルを取得する</span><span class="sxs-lookup"><span data-stu-id="41805-110">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="41805-111">サムネイルのコンテンツを取得する</span><span class="sxs-lookup"><span data-stu-id="41805-111">Retrieve thumbnail content</span></span>
* <span data-ttu-id="41805-112">1 つの要求で複数のアイテムのサムネイルを取得する</span><span class="sxs-lookup"><span data-stu-id="41805-112">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="41805-113">カスタムのサムネイル サイズを取得する</span><span class="sxs-lookup"><span data-stu-id="41805-113">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="41805-114">アイテムのカスタム サムネイルをアップロードする</span><span class="sxs-lookup"><span data-stu-id="41805-114">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="41805-115">カスタムのアップロード済みサムネイルが存在するかどうかを確認する</span><span class="sxs-lookup"><span data-stu-id="41805-115">Determine if a custom uploaded thumbnail exists</span></span>


## <a name="permissions"></a><span data-ttu-id="41805-116">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="41805-116">Permissions</span></span>

<span data-ttu-id="41805-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41805-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41805-119">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="41805-119">Permission type</span></span>      | <span data-ttu-id="41805-120">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="41805-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41805-121">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="41805-121">Delegated (work or school account)</span></span> | <span data-ttu-id="41805-122">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41805-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="41805-123">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="41805-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41805-124">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41805-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="41805-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="41805-125">Application</span></span> | <span data-ttu-id="41805-126">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41805-126">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="41805-127">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="41805-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="41805-128">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="41805-128">Optional query parameters</span></span>

<span data-ttu-id="41805-129">このメソッドは、応答をカスタマイズするための `$select` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="41805-129">This method supports the `$select` [OData puery parameter](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="41805-130">応答</span><span class="sxs-lookup"><span data-stu-id="41805-130">Response</span></span>

<span data-ttu-id="41805-131">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [ThumbnailSet](../resources/thumbnailset.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="41805-131">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41805-132">例</span><span class="sxs-lookup"><span data-stu-id="41805-132">Example</span></span>

<span data-ttu-id="41805-133">次は、現在のユーザーの OneDrive 内のアイテムで使用可能なサムネイルを取得する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="41805-133">Here is an example of the request which retrieves available thumbnails for an item in the current user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails
```

<span data-ttu-id="41805-134">このアイテムの使用可能な **thumbnailSets** の配列が返されます。</span><span class="sxs-lookup"><span data-stu-id="41805-134">This returns an array of available **thumbnailSets** for the item.</span></span> <span data-ttu-id="41805-135">ドライブにあるすべてのアイテムは、0 個以上のサムネイルを保持できます。</span><span class="sxs-lookup"><span data-stu-id="41805-135">Any item in a drive can have zero or more thumbnails.</span></span>

<span data-ttu-id="41805-p105">**注:**_select_ クエリ文字列パラメーターを使用すると、**ThumbnailSet** で返されるサムネイルのサイズを制御できます。 たとえば、`/thumbnails?select=medium` では、中サイズのサムネイルのみを取得します。</span><span class="sxs-lookup"><span data-stu-id="41805-p105">**Note:** You can use the _select_ query string parameter to control which thumbnail sizes are returned in the **ThumbnailSet**. For example, `/thumbnails?select=medium` retrieves only the medium sized thumbnails.</span></span>


### <a name="response"></a><span data-ttu-id="41805-138">応答</span><span class="sxs-lookup"><span data-stu-id="41805-138">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="41805-139">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="41805-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="41805-140">Visual</span><span class="sxs-lookup"><span data-stu-id="41805-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/enum-item-thumbnails-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41805-141">Java</span><span class="sxs-lookup"><span data-stu-id="41805-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/enum-item-thumbnails-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="get-a-single-thumbnail"></a><span data-ttu-id="41805-142">1 つのサムネイルを取得する</span><span class="sxs-lookup"><span data-stu-id="41805-142">Get a single thumbnail</span></span>

<span data-ttu-id="41805-143">1 つのサムネイルとサイズのメタデータを、要求で直接アドレス指定して取得します。</span><span class="sxs-lookup"><span data-stu-id="41805-143">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

### <a name="http-request"></a><span data-ttu-id="41805-144">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="41805-144">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```

### <a name="path-parameters"></a><span data-ttu-id="41805-145">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="41805-145">Path parameters</span></span>

| <span data-ttu-id="41805-146">名前</span><span class="sxs-lookup"><span data-stu-id="41805-146">Name</span></span>         | <span data-ttu-id="41805-147">型</span><span class="sxs-lookup"><span data-stu-id="41805-147">Type</span></span>   | <span data-ttu-id="41805-148">説明</span><span class="sxs-lookup"><span data-stu-id="41805-148">Description</span></span>                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="41805-149">**item-id**</span><span class="sxs-lookup"><span data-stu-id="41805-149">**item-id**</span></span>  | <span data-ttu-id="41805-150">string</span><span class="sxs-lookup"><span data-stu-id="41805-150">string</span></span> | <span data-ttu-id="41805-151">参照されるアイテムの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="41805-151">The unique identifier for the item referenced.</span></span>                                           |
| <span data-ttu-id="41805-152">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="41805-152">**thumb-id**</span></span> | <span data-ttu-id="41805-153">number</span><span class="sxs-lookup"><span data-stu-id="41805-153">number</span></span> | <span data-ttu-id="41805-p106">サムネイルのインデックス (通常 0-4)。 カスタム サムネイルがある場合は、そのインデックスは 0 になります。</span><span class="sxs-lookup"><span data-stu-id="41805-p106">The index of the thumbnail, usually 0-4. If there is a custom thumbnail, its index is 0.</span></span> |
| <span data-ttu-id="41805-156">**size**</span><span class="sxs-lookup"><span data-stu-id="41805-156">**size**</span></span>     | <span data-ttu-id="41805-157">string</span><span class="sxs-lookup"><span data-stu-id="41805-157">string</span></span> | <span data-ttu-id="41805-158">要求されたサムネイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="41805-158">The size of the thumbnail requested.</span></span> <span data-ttu-id="41805-159">これは、後述する標準サイズか、カスタム サイズのいずれかになります。</span><span class="sxs-lookup"><span data-stu-id="41805-159">This can be one of the standard sizes listed below or a custom size.</span></span> |

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="41805-160">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="41805-160">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="41805-161">Visual</span><span class="sxs-lookup"><span data-stu-id="41805-161">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-one-thumbnail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41805-162">Java</span><span class="sxs-lookup"><span data-stu-id="41805-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-one-thumbnail-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="retrieve-thumbnail-binary-content"></a><span data-ttu-id="41805-163">サムネイルのバイナリ コンテンツを取得する</span><span class="sxs-lookup"><span data-stu-id="41805-163">Retrieve thumbnail binary content</span></span>

<span data-ttu-id="41805-164">サムネイルの **content** プロパティを要求することにより、サムネイルのコンテンツを直接取得できます。</span><span class="sxs-lookup"><span data-stu-id="41805-164">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

### <a name="http-request"></a><span data-ttu-id="41805-165">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="41805-165">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```

### <a name="response"></a><span data-ttu-id="41805-166">応答</span><span class="sxs-lookup"><span data-stu-id="41805-166">Response</span></span>

<span data-ttu-id="41805-167">サービスは、サムネイルの URL へのリダイレクトで応答します。</span><span class="sxs-lookup"><span data-stu-id="41805-167">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="41805-168">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="41805-168">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="41805-169">Visual</span><span class="sxs-lookup"><span data-stu-id="41805-169">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-thumbnail-content-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41805-170">Java</span><span class="sxs-lookup"><span data-stu-id="41805-170">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-thumbnail-content-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="41805-171">サムネイル URL はキャッシュ対応です。</span><span class="sxs-lookup"><span data-stu-id="41805-171">Thumbnail URLs are cache-safe.</span></span> <span data-ttu-id="41805-172">この URL は、新しいサムネイルの生成を必要とする方法でアイテムを変更する場合に変更されます。</span><span class="sxs-lookup"><span data-stu-id="41805-172">The URL will change, if the item changes in a way that requires a new thumbnail to be generated.</span></span>


## <a name="getting-thumbnails-while-listing-driveitems"></a><span data-ttu-id="41805-173">DriveItems を一覧表示する際にサムネイルを取得する</span><span class="sxs-lookup"><span data-stu-id="41805-173">Getting thumbnails while listing DriveItems</span></span>

<span data-ttu-id="41805-174">表示する DriveItem リソースのリストを取得する場合、_$expand_ クエリ文字列パラメーターを使用して、それらのリソースのサムネイルも含めることができます。</span><span class="sxs-lookup"><span data-stu-id="41805-174">If you are retrieving a list of DriveItem resources to display, you can use the _$expand_ query string parameter to also include the thumbnails for those resources.</span></span>
<span data-ttu-id="41805-175">これによりアプリは、複数の要求を実行することなく、サムネイルとアイテムを 1 つの要求で取得することができます。</span><span class="sxs-lookup"><span data-stu-id="41805-175">This enables your app to retrieve thumbnails and items in a single request, instead of issuing many requests.</span></span>

### <a name="http-request"></a><span data-ttu-id="41805-176">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="41805-176">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```

### <a name="response"></a><span data-ttu-id="41805-177">応答</span><span class="sxs-lookup"><span data-stu-id="41805-177">Response</span></span>

<span data-ttu-id="41805-178">サービスは、DriveItems とそのサムネイルのリストで応答します。</span><span class="sxs-lookup"><span data-stu-id="41805-178">The service responses with the list of DriveItems and their thumbnails.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="41805-179">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="41805-179">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="41805-180">Visual</span><span class="sxs-lookup"><span data-stu-id="41805-180">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-thumbnail-while-listing-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41805-181">Java</span><span class="sxs-lookup"><span data-stu-id="41805-181">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-thumbnail-while-listing-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="size-values"></a><span data-ttu-id="41805-182">サイズの値</span><span class="sxs-lookup"><span data-stu-id="41805-182">Size values</span></span>

<span data-ttu-id="41805-p110">次の表で、使用可能なサムネイルのサイズを定義します。サムネイルの任意のサイズを要求できますが、定義済みの値が存在する可能性が高く、値は即時に返されます。</span><span class="sxs-lookup"><span data-stu-id="41805-p110">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="41805-185">名前</span><span class="sxs-lookup"><span data-stu-id="41805-185">Name</span></span>           | <span data-ttu-id="41805-186">解決策</span><span class="sxs-lookup"><span data-stu-id="41805-186">Resolution</span></span>  | <span data-ttu-id="41805-187">縦横比</span><span class="sxs-lookup"><span data-stu-id="41805-187">Aspect Ratio</span></span> | <span data-ttu-id="41805-188">説明</span><span class="sxs-lookup"><span data-stu-id="41805-188">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="41805-189">96 longest</span><span class="sxs-lookup"><span data-stu-id="41805-189">96 longest</span></span>  | <span data-ttu-id="41805-190">Original</span><span class="sxs-lookup"><span data-stu-id="41805-190">Original</span></span>     | <span data-ttu-id="41805-191">圧縮率の高い小さなサムネイルは、正方形にトリミングされます。</span><span class="sxs-lookup"><span data-stu-id="41805-191">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="41805-192">176 longest</span><span class="sxs-lookup"><span data-stu-id="41805-192">176 longest</span></span> | <span data-ttu-id="41805-193">Original</span><span class="sxs-lookup"><span data-stu-id="41805-193">Original</span></span>     | <span data-ttu-id="41805-194">OneDrive の Web ビューの標準的なアイテムのサイズにトリミングされます。</span><span class="sxs-lookup"><span data-stu-id="41805-194">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="41805-195">800 longest</span><span class="sxs-lookup"><span data-stu-id="41805-195">800 longest</span></span> | <span data-ttu-id="41805-196">元の比率</span><span class="sxs-lookup"><span data-stu-id="41805-196">Original</span></span>     | <span data-ttu-id="41805-197">サムネイルの長辺が 800 ピクセルになるよう、サイズ変更されます。</span><span class="sxs-lookup"><span data-stu-id="41805-197">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |
| `smallSquare`  | <span data-ttu-id="41805-198">96x96</span><span class="sxs-lookup"><span data-stu-id="41805-198">96x96</span></span>       | <span data-ttu-id="41805-199">正方形にトリミング</span><span class="sxs-lookup"><span data-stu-id="41805-199">Square Crop</span></span>  | <span data-ttu-id="41805-200">小さな正方形のサムネイル</span><span class="sxs-lookup"><span data-stu-id="41805-200">Small square thumbnail</span></span>                                               |
| `mediumSquare` | <span data-ttu-id="41805-201">176x176</span><span class="sxs-lookup"><span data-stu-id="41805-201">176x176</span></span>     | <span data-ttu-id="41805-202">正方形にトリミング</span><span class="sxs-lookup"><span data-stu-id="41805-202">Square Crop</span></span>  | <span data-ttu-id="41805-203">小さな正方形のサムネイル</span><span class="sxs-lookup"><span data-stu-id="41805-203">Small square thumbnail</span></span>                                               |
| `largeSquare`  | <span data-ttu-id="41805-204">800x800</span><span class="sxs-lookup"><span data-stu-id="41805-204">800x800</span></span>     | <span data-ttu-id="41805-205">正方形にトリミング</span><span class="sxs-lookup"><span data-stu-id="41805-205">Square Crop</span></span>  | <span data-ttu-id="41805-206">大きな正方形のサムネイル</span><span class="sxs-lookup"><span data-stu-id="41805-206">Large square thumbnail</span></span>                                               |

## <a name="requesting-custom-thumbnail-sizes"></a><span data-ttu-id="41805-207">カスタムのサムネイル サイズを要求する</span><span class="sxs-lookup"><span data-stu-id="41805-207">Requesting custom thumbnail sizes</span></span>

<span data-ttu-id="41805-208">定義済みのサイズに加えて、アプリでは、先頭に `c` を付けたサムネイルのディメンションを指定することで、カスタムのサムネイル サイズを要求できます。</span><span class="sxs-lookup"><span data-stu-id="41805-208">In addition to the defined sizes, your app can request a custom thumbnail size by specifying the dimensions of the thumbnail prefixed with `c`.</span></span>
<span data-ttu-id="41805-209">たとえば、アプリで 300x400 のサムネイルが必要な場合は、そのサイズを次に示すように要求できます。</span><span class="sxs-lookup"><span data-stu-id="41805-209">For example if your app needs thumbnails that are 300x400, it can request that size like this:</span></span>

<!-- { "name": "get-thumbnail-custom-size", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_Crop
```

<span data-ttu-id="41805-210">これにより、選択したカスタムのサムネイル サイズのみの応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="41805-210">Which responds with just the custom thumbnail size selected:</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="41805-211">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="41805-211">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="41805-212">Visual</span><span class="sxs-lookup"><span data-stu-id="41805-212">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-thumbnail-custom-size-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41805-213">Java</span><span class="sxs-lookup"><span data-stu-id="41805-213">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-thumbnail-custom-size-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="41805-214">要求するサムネイルのサイズの後ろに、次に示すオプションを指定できます。</span><span class="sxs-lookup"><span data-stu-id="41805-214">You can specify the following options after the size of the thumbnail requested:</span></span>

### <a name="examples-of-custom-identifiers"></a><span data-ttu-id="41805-215">カスタム識別子の例</span><span class="sxs-lookup"><span data-stu-id="41805-215">Examples of custom identifiers</span></span>

| <span data-ttu-id="41805-216">サムネイル識別子</span><span class="sxs-lookup"><span data-stu-id="41805-216">Thumbnail identifier</span></span> | <span data-ttu-id="41805-217">解像度</span><span class="sxs-lookup"><span data-stu-id="41805-217">Resolution</span></span>             | <span data-ttu-id="41805-218">縦横比</span><span class="sxs-lookup"><span data-stu-id="41805-218">Aspect ratio</span></span> | <span data-ttu-id="41805-219">説明</span><span class="sxs-lookup"><span data-stu-id="41805-219">Description</span></span>                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="41805-220">c300x400</span><span class="sxs-lookup"><span data-stu-id="41805-220">c300x400</span></span>             | <span data-ttu-id="41805-221">300x400 のボックスに制限されます</span><span class="sxs-lookup"><span data-stu-id="41805-221">Bounded by 300x400 box</span></span> | <span data-ttu-id="41805-222">Original</span><span class="sxs-lookup"><span data-stu-id="41805-222">Original</span></span>     | <span data-ttu-id="41805-223">300x400 ピクセルのボックスに収まるサムネイルを生成します。縦横比は維持されます。</span><span class="sxs-lookup"><span data-stu-id="41805-223">Generate a thumbnail that fits inside a 300x400 pixel box, maintaining aspect ratio</span></span>                                                                 |
| <span data-ttu-id="41805-224">c300x400_Crop</span><span class="sxs-lookup"><span data-stu-id="41805-224">c300x400_Crop</span></span>        | <span data-ttu-id="41805-225">300x400</span><span class="sxs-lookup"><span data-stu-id="41805-225">300x400</span></span>                | <span data-ttu-id="41805-226">トリミング</span><span class="sxs-lookup"><span data-stu-id="41805-226">Cropped</span></span>      | <span data-ttu-id="41805-p112">300x400 ピクセルのサムネイルを生成します。 これは、300x400 のボックスに収まるように画像のサイズを変更し、このボックスに収まらない部分をトリミングするように動作します。</span><span class="sxs-lookup"><span data-stu-id="41805-p112">Generate a thumbnail that is 300x400 pixels. This works by resizing the image to fill the 300x400 box and cropping whatever spills outside the box.</span></span> |

<span data-ttu-id="41805-229">**注:** 返されるサムネイルのピクセル ディメンションは要求されたものと正確に一致しないことがありますが、縦横比は一致します。</span><span class="sxs-lookup"><span data-stu-id="41805-229">**Note:** The thumbnail returned may not exactly match the pixel dimensions that was requested, but will match the aspect ratio.</span></span>
<span data-ttu-id="41805-230">サムネイルがすでに存在しており、要求された解像度に簡単に拡大縮小できる場合、要求されたものよりも大きいサムネイルが返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="41805-230">In some cases, a larger thumbnail may be returned than was requested, if the thumbnail already exists and can easily be scaled to match the requested resolution.</span></span>

## <a name="remarks"></a><span data-ttu-id="41805-231">備考</span><span class="sxs-lookup"><span data-stu-id="41805-231">Remarks</span></span>

<span data-ttu-id="41805-232">**注:** OneDrive for Business および SharePoint の場合:</span><span class="sxs-lookup"><span data-stu-id="41805-232">**Note** In OneDrive for Business and SharePoint:</span></span>

<span data-ttu-id="41805-233">次の呼び出しを使用したサムネイル コレクションの展開は機能しません: </span><span class="sxs-lookup"><span data-stu-id="41805-233">Using these calls to expand the thumbnails collection will not work:</span></span>

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

<span data-ttu-id="41805-234">サムネイルは、SharePoint Server 2016 ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41805-234">Thumbnails are not supported on SharePoint Server 2016.</span></span>

### <a name="error-responses"></a><span data-ttu-id="41805-235">エラー応答</span><span class="sxs-lookup"><span data-stu-id="41805-235">Error responses</span></span>

<span data-ttu-id="41805-236">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41805-236">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "Items/Thumbnails",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
