---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ファイルまたはフォルダーのサムネイルを取得する
localization_priority: Normal
ms.prod: sharepoint
description: DriveItem リソースの ThumbnailSet リソースのコレクションを取得します。
doc_type: apiPageType
ms.openlocfilehash: 64a863464bb457e6fd3e9909ff8df6ddd99ec73a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349377"
---
# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="e2812-103">DriveItem のサムネイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e2812-103">List thumbnails for a DriveItem</span></span>

<span data-ttu-id="e2812-104">[DriveItem](../resources/driveitem.md) リソースの [ThumbnailSet](../resources/thumbnailset.md) リソースのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="e2812-104">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="e2812-p101">DriveItem はゼロ以上の [ThumbnailSet](../resources/thumbnailset.md) リソースで表すことができます。各 **thumbnailSet** は 1 つ以上の[**サムネイル**](../resources/thumbnail.md) オブジェクトを持つことができ、そのオブジェクトはアイテムを表すイメージです。たとえば、**thumbnailSet** には `small`、`medium`、`large` など、一般的な**サムネイル** オブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="e2812-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="e2812-p102">OneDrive 上でサムネイルを操作する方法はたくさんあります。次に、最も一般的なものを示します。</span><span class="sxs-lookup"><span data-stu-id="e2812-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="e2812-110">アイテムの利用可能なサムネイルを列挙する</span><span class="sxs-lookup"><span data-stu-id="e2812-110">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="e2812-111">アイテムの 1 つのサムネイルを取得する</span><span class="sxs-lookup"><span data-stu-id="e2812-111">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="e2812-112">サムネイルのコンテンツを取得する</span><span class="sxs-lookup"><span data-stu-id="e2812-112">Retrieve thumbnail content</span></span>
* <span data-ttu-id="e2812-113">1 つの要求で複数のアイテムのサムネイルを取得する</span><span class="sxs-lookup"><span data-stu-id="e2812-113">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="e2812-114">カスタムのサムネイル サイズを取得する</span><span class="sxs-lookup"><span data-stu-id="e2812-114">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="e2812-115">アイテムのカスタム サムネイルをアップロードする</span><span class="sxs-lookup"><span data-stu-id="e2812-115">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="e2812-116">カスタムのアップロード済みサムネイルが存在するかどうかを確認する</span><span class="sxs-lookup"><span data-stu-id="e2812-116">Determine if a custom uploaded thumbnail exists</span></span>

## <a name="permissions"></a><span data-ttu-id="e2812-117">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e2812-117">Permissions</span></span>

<span data-ttu-id="e2812-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2812-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2812-120">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e2812-120">Permission type</span></span>      | <span data-ttu-id="e2812-121">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e2812-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2812-122">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e2812-122">Delegated (work or school account)</span></span> | <span data-ttu-id="e2812-123">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2812-123">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e2812-124">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e2812-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2812-125">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2812-125">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e2812-126">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e2812-126">Application</span></span> | <span data-ttu-id="e2812-127">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2812-127">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2812-128">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e2812-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e2812-129">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e2812-129">Optional query parameters</span></span>

<span data-ttu-id="e2812-130">このメソッドは、応答をカスタマイズするための `$select` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e2812-130">This method supports the `$select` [OData puery parameter](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="e2812-131">応答</span><span class="sxs-lookup"><span data-stu-id="e2812-131">Response</span></span>

<span data-ttu-id="e2812-132">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [ThumbnailSet](../resources/thumbnailset.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e2812-132">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2812-133">例</span><span class="sxs-lookup"><span data-stu-id="e2812-133">Example</span></span>

<span data-ttu-id="e2812-134">次は、現在のユーザーの OneDrive 内のアイテムで使用可能なサムネイルを取得する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e2812-134">Here is an example of the request which retrieves available thumbnails for an item in the current user's OneDrive.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e2812-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e2812-135">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/thumbnails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e2812-136">C#</span><span class="sxs-lookup"><span data-stu-id="e2812-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-item-thumbnails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e2812-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2812-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-item-thumbnails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e2812-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="e2812-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-item-thumbnails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e2812-139">Java</span><span class="sxs-lookup"><span data-stu-id="e2812-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-item-thumbnails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="e2812-140">このアイテムの使用可能な **thumbnailSets** の配列が返されます。</span><span class="sxs-lookup"><span data-stu-id="e2812-140">This returns an array of available **thumbnailSets** for the item.</span></span> <span data-ttu-id="e2812-141">ドライブにあるすべてのアイテムは、0 個以上のサムネイルを保持できます。</span><span class="sxs-lookup"><span data-stu-id="e2812-141">Any item in a drive can have zero or more thumbnails.</span></span>

<span data-ttu-id="e2812-p105">**注:**_select_ クエリ文字列パラメーターを使用すると、**ThumbnailSet** で返されるサムネイルのサイズを制御できます。 たとえば、`/thumbnails?select=medium` では、中サイズのサムネイルのみを取得します。</span><span class="sxs-lookup"><span data-stu-id="e2812-p105">**Note:** You can use the _select_ query string parameter to control which thumbnail sizes are returned in the **ThumbnailSet**. For example, `/thumbnails?select=medium` retrieves only the medium sized thumbnails.</span></span>


### <a name="response"></a><span data-ttu-id="e2812-144">応答</span><span class="sxs-lookup"><span data-stu-id="e2812-144">Response</span></span>

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

## <a name="get-a-single-thumbnail"></a><span data-ttu-id="e2812-145">1 つのサムネイルを取得する</span><span class="sxs-lookup"><span data-stu-id="e2812-145">Get a single thumbnail</span></span>

<span data-ttu-id="e2812-146">1 つのサムネイルとサイズのメタデータを、要求で直接アドレス指定して取得します。</span><span class="sxs-lookup"><span data-stu-id="e2812-146">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

### <a name="http-request"></a><span data-ttu-id="e2812-147">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e2812-147">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e2812-148">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e2812-148">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e2812-149">C#</span><span class="sxs-lookup"><span data-stu-id="e2812-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-one-thumbnail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e2812-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2812-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-one-thumbnail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e2812-151">目的-C</span><span class="sxs-lookup"><span data-stu-id="e2812-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-one-thumbnail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e2812-152">Java</span><span class="sxs-lookup"><span data-stu-id="e2812-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-one-thumbnail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="e2812-153">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="e2812-153">Path parameters</span></span>

| <span data-ttu-id="e2812-154">名前</span><span class="sxs-lookup"><span data-stu-id="e2812-154">Name</span></span>         | <span data-ttu-id="e2812-155">型</span><span class="sxs-lookup"><span data-stu-id="e2812-155">Type</span></span>   | <span data-ttu-id="e2812-156">説明</span><span class="sxs-lookup"><span data-stu-id="e2812-156">Description</span></span>                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="e2812-157">**item-id**</span><span class="sxs-lookup"><span data-stu-id="e2812-157">**item-id**</span></span>  | <span data-ttu-id="e2812-158">string</span><span class="sxs-lookup"><span data-stu-id="e2812-158">string</span></span> | <span data-ttu-id="e2812-159">参照されるアイテムの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="e2812-159">The unique identifier for the item referenced.</span></span>                                           |
| <span data-ttu-id="e2812-160">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="e2812-160">**thumb-id**</span></span> | <span data-ttu-id="e2812-161">number</span><span class="sxs-lookup"><span data-stu-id="e2812-161">number</span></span> | <span data-ttu-id="e2812-p106">サムネイルのインデックス (通常 0-4)。 カスタム サムネイルがある場合は、そのインデックスは 0 になります。</span><span class="sxs-lookup"><span data-stu-id="e2812-p106">The index of the thumbnail, usually 0-4. If there is a custom thumbnail, its index is 0.</span></span> |
| <span data-ttu-id="e2812-164">**size**</span><span class="sxs-lookup"><span data-stu-id="e2812-164">**size**</span></span>     | <span data-ttu-id="e2812-165">string</span><span class="sxs-lookup"><span data-stu-id="e2812-165">string</span></span> | <span data-ttu-id="e2812-166">要求されたサムネイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="e2812-166">The size of the thumbnail requested.</span></span> <span data-ttu-id="e2812-167">これは、後述する標準サイズか、カスタム サイズのいずれかになります。</span><span class="sxs-lookup"><span data-stu-id="e2812-167">This can be one of the standard sizes listed below or a custom size.</span></span> |

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

## <a name="retrieve-thumbnail-binary-content"></a><span data-ttu-id="e2812-168">サムネイルのバイナリ コンテンツを取得する</span><span class="sxs-lookup"><span data-stu-id="e2812-168">Retrieve thumbnail binary content</span></span>

<span data-ttu-id="e2812-169">サムネイルの **content** プロパティを要求することにより、サムネイルのコンテンツを直接取得できます。</span><span class="sxs-lookup"><span data-stu-id="e2812-169">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

### <a name="http-request"></a><span data-ttu-id="e2812-170">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e2812-170">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e2812-171">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e2812-171">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e2812-172">C#</span><span class="sxs-lookup"><span data-stu-id="e2812-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e2812-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2812-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e2812-174">目的-C</span><span class="sxs-lookup"><span data-stu-id="e2812-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e2812-175">Java</span><span class="sxs-lookup"><span data-stu-id="e2812-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e2812-176">応答</span><span class="sxs-lookup"><span data-stu-id="e2812-176">Response</span></span>

<span data-ttu-id="e2812-177">サービスは、サムネイルの URL へのリダイレクトで応答します。</span><span class="sxs-lookup"><span data-stu-id="e2812-177">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="e2812-178">サムネイル URL はキャッシュ対応です。</span><span class="sxs-lookup"><span data-stu-id="e2812-178">Thumbnail URLs are cache-safe.</span></span> <span data-ttu-id="e2812-179">この URL は、新しいサムネイルの生成を必要とする方法でアイテムを変更する場合に変更されます。</span><span class="sxs-lookup"><span data-stu-id="e2812-179">The URL will change, if the item changes in a way that requires a new thumbnail to be generated.</span></span>


## <a name="getting-thumbnails-while-listing-driveitems"></a><span data-ttu-id="e2812-180">DriveItems を一覧表示する際にサムネイルを取得する</span><span class="sxs-lookup"><span data-stu-id="e2812-180">Getting thumbnails while listing DriveItems</span></span>

<span data-ttu-id="e2812-181">表示する DriveItem リソースのリストを取得する場合、_$expand_ クエリ文字列パラメーターを使用して、それらのリソースのサムネイルも含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e2812-181">If you are retrieving a list of DriveItem resources to display, you can use the _$expand_ query string parameter to also include the thumbnails for those resources.</span></span>
<span data-ttu-id="e2812-182">これによりアプリは、複数の要求を実行することなく、サムネイルとアイテムを 1 つの要求で取得することができます。</span><span class="sxs-lookup"><span data-stu-id="e2812-182">This enables your app to retrieve thumbnails and items in a single request, instead of issuing many requests.</span></span>

### <a name="http-request"></a><span data-ttu-id="e2812-183">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e2812-183">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e2812-184">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e2812-184">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e2812-185">C#</span><span class="sxs-lookup"><span data-stu-id="e2812-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-while-listing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e2812-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2812-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-while-listing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e2812-187">目的-C</span><span class="sxs-lookup"><span data-stu-id="e2812-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-while-listing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e2812-188">Java</span><span class="sxs-lookup"><span data-stu-id="e2812-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-while-listing-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e2812-189">応答</span><span class="sxs-lookup"><span data-stu-id="e2812-189">Response</span></span>

<span data-ttu-id="e2812-190">サービスは、DriveItems とそのサムネイルのリストで応答します。</span><span class="sxs-lookup"><span data-stu-id="e2812-190">The service responses with the list of DriveItems and their thumbnails.</span></span>

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

## <a name="size-options"></a><span data-ttu-id="e2812-191">サイズオプション</span><span class="sxs-lookup"><span data-stu-id="e2812-191">Size options</span></span>

<span data-ttu-id="e2812-p110">次の表で、使用可能なサムネイルのサイズを定義します。サムネイルの任意のサイズを要求できますが、定義済みの値が存在する可能性が高く、値は即時に返されます。</span><span class="sxs-lookup"><span data-stu-id="e2812-p110">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="e2812-194">名前</span><span class="sxs-lookup"><span data-stu-id="e2812-194">Name</span></span>           | <span data-ttu-id="e2812-195">解像度</span><span class="sxs-lookup"><span data-stu-id="e2812-195">Resolution</span></span>  | <span data-ttu-id="e2812-196">縦横比</span><span class="sxs-lookup"><span data-stu-id="e2812-196">Aspect Ratio</span></span> | <span data-ttu-id="e2812-197">説明</span><span class="sxs-lookup"><span data-stu-id="e2812-197">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="e2812-198">96 longest</span><span class="sxs-lookup"><span data-stu-id="e2812-198">96 longest</span></span>  | <span data-ttu-id="e2812-199">Original</span><span class="sxs-lookup"><span data-stu-id="e2812-199">Original</span></span>     | <span data-ttu-id="e2812-200">圧縮率の高い小さなサムネイルは、正方形にトリミングされます。</span><span class="sxs-lookup"><span data-stu-id="e2812-200">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="e2812-201">176 longest</span><span class="sxs-lookup"><span data-stu-id="e2812-201">176 longest</span></span> | <span data-ttu-id="e2812-202">Original</span><span class="sxs-lookup"><span data-stu-id="e2812-202">Original</span></span>     | <span data-ttu-id="e2812-203">OneDrive の Web ビューの標準的なアイテムのサイズにトリミングされます。</span><span class="sxs-lookup"><span data-stu-id="e2812-203">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="e2812-204">800 longest</span><span class="sxs-lookup"><span data-stu-id="e2812-204">800 longest</span></span> | <span data-ttu-id="e2812-205">Original</span><span class="sxs-lookup"><span data-stu-id="e2812-205">Original</span></span>     | <span data-ttu-id="e2812-206">サムネイルの長辺が 800 ピクセルになるよう、サイズ変更されます。</span><span class="sxs-lookup"><span data-stu-id="e2812-206">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |
| `smallSquare`  | <span data-ttu-id="e2812-207">96x96</span><span class="sxs-lookup"><span data-stu-id="e2812-207">96x96</span></span>       | <span data-ttu-id="e2812-208">正方形にトリミング</span><span class="sxs-lookup"><span data-stu-id="e2812-208">Square Crop</span></span>  | <span data-ttu-id="e2812-209">小さな正方形のサムネイル</span><span class="sxs-lookup"><span data-stu-id="e2812-209">Small square thumbnail</span></span>                                               |
| `mediumSquare` | <span data-ttu-id="e2812-210">176x176</span><span class="sxs-lookup"><span data-stu-id="e2812-210">176x176</span></span>     | <span data-ttu-id="e2812-211">正方形にトリミング</span><span class="sxs-lookup"><span data-stu-id="e2812-211">Square Crop</span></span>  | <span data-ttu-id="e2812-212">小さな正方形のサムネイル</span><span class="sxs-lookup"><span data-stu-id="e2812-212">Small square thumbnail</span></span>                                               |
| `largeSquare`  | <span data-ttu-id="e2812-213">800x800</span><span class="sxs-lookup"><span data-stu-id="e2812-213">800x800</span></span>     | <span data-ttu-id="e2812-214">正方形にトリミング</span><span class="sxs-lookup"><span data-stu-id="e2812-214">Square Crop</span></span>  | <span data-ttu-id="e2812-215">大きな正方形のサムネイル</span><span class="sxs-lookup"><span data-stu-id="e2812-215">Large square thumbnail</span></span>                                               |

## <a name="requesting-custom-thumbnail-sizes"></a><span data-ttu-id="e2812-216">カスタムのサムネイル サイズを要求する</span><span class="sxs-lookup"><span data-stu-id="e2812-216">Requesting custom thumbnail sizes</span></span>

<span data-ttu-id="e2812-217">定義済みのサイズに加えて、アプリでは、先頭に `c` を付けたサムネイルのディメンションを指定することで、カスタムのサムネイル サイズを要求できます。</span><span class="sxs-lookup"><span data-stu-id="e2812-217">In addition to the defined sizes, your app can request a custom thumbnail size by specifying the dimensions of the thumbnail prefixed with `c`.</span></span>
<span data-ttu-id="e2812-218">たとえば、アプリで 300x400 のサムネイルが必要な場合は、そのサイズを次に示すように要求できます。</span><span class="sxs-lookup"><span data-stu-id="e2812-218">For example if your app needs thumbnails that are 300x400, it can request that size like this:</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e2812-219">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e2812-219">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-thumbnail-custom-size", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_Crop
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e2812-220">C#</span><span class="sxs-lookup"><span data-stu-id="e2812-220">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-custom-size-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e2812-221">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2812-221">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-custom-size-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e2812-222">目的-C</span><span class="sxs-lookup"><span data-stu-id="e2812-222">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-custom-size-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e2812-223">Java</span><span class="sxs-lookup"><span data-stu-id="e2812-223">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-custom-size-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="e2812-224">これにより、選択したカスタムのサムネイル サイズのみの応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="e2812-224">Which responds with just the custom thumbnail size selected:</span></span>

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

<span data-ttu-id="e2812-225">要求するサムネイルのサイズの後ろに、次に示すオプションを指定できます。</span><span class="sxs-lookup"><span data-stu-id="e2812-225">You can specify the following options after the size of the thumbnail requested:</span></span>

### <a name="examples-of-custom-identifiers"></a><span data-ttu-id="e2812-226">カスタム識別子の例</span><span class="sxs-lookup"><span data-stu-id="e2812-226">Examples of custom identifiers</span></span>

| <span data-ttu-id="e2812-227">サムネイル識別子</span><span class="sxs-lookup"><span data-stu-id="e2812-227">Thumbnail identifier</span></span> | <span data-ttu-id="e2812-228">解像度</span><span class="sxs-lookup"><span data-stu-id="e2812-228">Resolution</span></span>             | <span data-ttu-id="e2812-229">縦横比</span><span class="sxs-lookup"><span data-stu-id="e2812-229">Aspect ratio</span></span> | <span data-ttu-id="e2812-230">説明</span><span class="sxs-lookup"><span data-stu-id="e2812-230">Description</span></span>                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e2812-231">c300x400</span><span class="sxs-lookup"><span data-stu-id="e2812-231">c300x400</span></span>             | <span data-ttu-id="e2812-232">300x400 のボックスに制限されます</span><span class="sxs-lookup"><span data-stu-id="e2812-232">Bounded by 300x400 box</span></span> | <span data-ttu-id="e2812-233">Original</span><span class="sxs-lookup"><span data-stu-id="e2812-233">Original</span></span>     | <span data-ttu-id="e2812-234">300x400 ピクセルのボックスに収まるサムネイルを生成します。縦横比は維持されます。</span><span class="sxs-lookup"><span data-stu-id="e2812-234">Generate a thumbnail that fits inside a 300x400 pixel box, maintaining aspect ratio</span></span>                                                                 |
| <span data-ttu-id="e2812-235">c300x400_Crop</span><span class="sxs-lookup"><span data-stu-id="e2812-235">c300x400_Crop</span></span>        | <span data-ttu-id="e2812-236">300x400</span><span class="sxs-lookup"><span data-stu-id="e2812-236">300x400</span></span>                | <span data-ttu-id="e2812-237">トリミング</span><span class="sxs-lookup"><span data-stu-id="e2812-237">Cropped</span></span>      | <span data-ttu-id="e2812-p112">300x400 ピクセルのサムネイルを生成します。 これは、300x400 のボックスに収まるように画像のサイズを変更し、このボックスに収まらない部分をトリミングするように動作します。</span><span class="sxs-lookup"><span data-stu-id="e2812-p112">Generate a thumbnail that is 300x400 pixels. This works by resizing the image to fill the 300x400 box and cropping whatever spills outside the box.</span></span> |

<span data-ttu-id="e2812-240">**注:** 返されるサムネイルのピクセル ディメンションは要求されたものと正確に一致しないことがありますが、縦横比は一致します。</span><span class="sxs-lookup"><span data-stu-id="e2812-240">**Note:** The thumbnail returned may not exactly match the pixel dimensions that was requested, but will match the aspect ratio.</span></span>
<span data-ttu-id="e2812-241">サムネイルがすでに存在しており、要求された解像度に簡単に拡大縮小できる場合、要求されたものよりも大きいサムネイルが返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e2812-241">In some cases, a larger thumbnail may be returned than was requested, if the thumbnail already exists and can easily be scaled to match the requested resolution.</span></span>

## <a name="remarks"></a><span data-ttu-id="e2812-242">備考</span><span class="sxs-lookup"><span data-stu-id="e2812-242">Remarks</span></span>

<span data-ttu-id="e2812-243">**注:** OneDrive for Business および SharePoint の場合:</span><span class="sxs-lookup"><span data-stu-id="e2812-243">**Note** In OneDrive for Business and SharePoint:</span></span>

<span data-ttu-id="e2812-244">次の呼び出しを使用したサムネイル コレクションの展開は機能しません: </span><span class="sxs-lookup"><span data-stu-id="e2812-244">Using these calls to expand the thumbnails collection will not work:</span></span>

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

<span data-ttu-id="e2812-245">サムネイルは、SharePoint Server 2016 ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2812-245">Thumbnails are not supported on SharePoint Server 2016.</span></span>

### <a name="error-responses"></a><span data-ttu-id="e2812-246">エラー応答</span><span class="sxs-lookup"><span data-stu-id="e2812-246">Error responses</span></span>

<span data-ttu-id="e2812-247">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2812-247">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

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
