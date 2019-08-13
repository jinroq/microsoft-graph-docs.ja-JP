---
author: JeremyKelley
ms.author: jeremyke
title: バンドルを取得する
description: ドライブ項目のバンドルを取得する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 55d24648a8cc69f196be4f5aa820fe619281ff4b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317999"
---
# <a name="get-bundle"></a><span data-ttu-id="974d2-103">バンドルを取得する</span><span class="sxs-lookup"><span data-stu-id="974d2-103">Get bundle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="974d2-104">バンドルの一意の ID に基づいて、[バンドル][]のメタデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="974d2-104">Retrieve the metadata for a [bundle][] based on the bundle's unique ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="974d2-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="974d2-105">Permissions</span></span>

<span data-ttu-id="974d2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="974d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="974d2-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="974d2-108">Permission type</span></span>      | <span data-ttu-id="974d2-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="974d2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="974d2-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="974d2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="974d2-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="974d2-111">Not supported.</span></span>                             |
|<span data-ttu-id="974d2-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="974d2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="974d2-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="974d2-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="974d2-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="974d2-114">Application</span></span>          | <span data-ttu-id="974d2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="974d2-115">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="974d2-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="974d2-116">HTTP request</span></span>

```http
GET /drive/bundles/{bundle-id}
GET /drive/items/{bundle-id}
```

<span data-ttu-id="974d2-117">バンドルはアイテムであるため、 **items**コレクションを使用して、バンドルに関するメタデータを返すことができます。</span><span class="sxs-lookup"><span data-stu-id="974d2-117">Because bundles are items, you can use the **items** collection to return metadata about a bundle.</span></span>
<span data-ttu-id="974d2-118">また、バンドルコレクションを\*\*\*\* 使用して、確実にバンドルを取得していることを確認することもできます。</span><span class="sxs-lookup"><span data-stu-id="974d2-118">You can also use the **bundles** collection as a convenience to ensure you're getting a bundle in response.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="974d2-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="974d2-119">Optional query parameters</span></span>

<span data-ttu-id="974d2-120">[OData クエリ パラメーター][odata-parameters]を使用して、この呼び出しから返されるオブジェクトのシェイプを制限することができます。</span><span class="sxs-lookup"><span data-stu-id="974d2-120">You can use the [OData query parameters][odata-parameters] to restrict the shape of the objects returned from this call.</span></span>

## <a name="request-headers"></a><span data-ttu-id="974d2-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="974d2-121">Request headers</span></span>
| <span data-ttu-id="974d2-122">名前</span><span class="sxs-lookup"><span data-stu-id="974d2-122">Name</span></span>          | <span data-ttu-id="974d2-123">説明</span><span class="sxs-lookup"><span data-stu-id="974d2-123">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="974d2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="974d2-124">Authorization</span></span> | <span data-ttu-id="974d2-125">ベアラー \{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="974d2-125">Bearer \{token\}.</span></span> <span data-ttu-id="974d2-126">必須。</span><span class="sxs-lookup"><span data-stu-id="974d2-126">Required.</span></span> |
| <span data-ttu-id="974d2-127">if-none-match</span><span class="sxs-lookup"><span data-stu-id="974d2-127">if-none-match</span></span> | <span data-ttu-id="974d2-128">eTag.</span><span class="sxs-lookup"><span data-stu-id="974d2-128">eTag.</span></span> <span data-ttu-id="974d2-129">省略可能。</span><span class="sxs-lookup"><span data-stu-id="974d2-129">Optional.</span></span> <span data-ttu-id="974d2-130">この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="974d2-130">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span>

## <a name="request-body"></a><span data-ttu-id="974d2-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="974d2-131">Request body</span></span>

<span data-ttu-id="974d2-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="974d2-132">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="974d2-133">応答</span><span class="sxs-lookup"><span data-stu-id="974d2-133">Response</span></span>

<span data-ttu-id="974d2-134">成功した場合、このメソッドは応答本文で[drive 項目][driveItem] resource with the [bundle][bundle]を返します。</span><span class="sxs-lookup"><span data-stu-id="974d2-134">If successful, this method returns a [driveItem][driveItem] resource with the [bundle][bundle] in the response body.</span></span>

<span data-ttu-id="974d2-135">エラーがどのように返されるかに関する詳細については、「[エラー応答][error-response]」のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="974d2-135">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="974d2-136">例</span><span class="sxs-lookup"><span data-stu-id="974d2-136">Examples</span></span>

### <a name="example-1-get-a-bundle"></a><span data-ttu-id="974d2-137">例 1: バンドルを取得する</span><span class="sxs-lookup"><span data-stu-id="974d2-137">Example 1: Get a bundle</span></span>

#### <a name="request"></a><span data-ttu-id="974d2-138">要求</span><span class="sxs-lookup"><span data-stu-id="974d2-138">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="974d2-139">プロトコル</span><span class="sxs-lookup"><span data-stu-id="974d2-139">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-bundle-metadata" } -->

```http
GET https://graph.microsoft.com/beta/drive/bundles/{bundle-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="974d2-140">C#</span><span class="sxs-lookup"><span data-stu-id="974d2-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bundle-metadata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="974d2-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="974d2-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bundle-metadata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="974d2-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="974d2-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bundle-metadata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="974d2-143">Java</span><span class="sxs-lookup"><span data-stu-id="974d2-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bundle-metadata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="974d2-144">応答</span><span class="sxs-lookup"><span data-stu-id="974d2-144">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0123456789abc",
  "name": "My Photo Album Bundle",
  "eTag": "etag",
  "cTag": "etag",
  "createdBy": { "user": { "id": "1234", "displayName": "Ryan Gregg" } },
  "createdDateTime": "datetime",
  "lastModifiedBy": { "user": { "id": "1234", "displayName": "Ryan Gregg" } },
  "lastModifiedDateTime": "datetime",
  "size": 1234,
  "webUrl": "http://onedrive.com/...",
  "bundle": {
    "childCount": 4,
     "album": { }
  }
}
```

<span data-ttu-id="974d2-145">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="974d2-145">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="974d2-146">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="974d2-146">All the properties will be returned from an actual call.</span></span>

### <a name="example-2-get-a-bundle-and-its-children-in-a-single-call"></a><span data-ttu-id="974d2-147">例 2: 1 回の呼び出しでバンドルとその子を取得する</span><span class="sxs-lookup"><span data-stu-id="974d2-147">Example 2: Get a bundle and its children in a single call</span></span>

<span data-ttu-id="974d2-148">[`expand`](/graph/query-parameters)クエリ文字列パラメーターを使用して、バンドルのメタデータを取得するのと同じ呼び出しで、バンドルの子を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="974d2-148">You can use the [`expand`](/graph/query-parameters) query string parameter to include the children of a bundle in the same call as retrieving the metadata of a bundle.</span></span>

#### <a name="request"></a><span data-ttu-id="974d2-149">要求</span><span class="sxs-lookup"><span data-stu-id="974d2-149">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="974d2-150">プロトコル</span><span class="sxs-lookup"><span data-stu-id="974d2-150">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-bundle-and-children" } -->

```http
GET https://graph.microsoft.com/beta/drive/items/{bundle-id}?expand=children
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="974d2-151">C#</span><span class="sxs-lookup"><span data-stu-id="974d2-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bundle-and-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="974d2-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="974d2-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bundle-and-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="974d2-153">目的-C</span><span class="sxs-lookup"><span data-stu-id="974d2-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bundle-and-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="974d2-154">Java</span><span class="sxs-lookup"><span data-stu-id="974d2-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bundle-and-children-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="974d2-155">応答</span><span class="sxs-lookup"><span data-stu-id="974d2-155">Response</span></span>

<span data-ttu-id="974d2-156">この呼び出しは、バンドルメタデータと、バンドルの子のリストを返します。</span><span class="sxs-lookup"><span data-stu-id="974d2-156">This call will return the bundle metadata and a list of children of the bundle.</span></span>
<span data-ttu-id="974d2-157">バンドルに子がない場合は、空のコレクションが返されます。</span><span class="sxs-lookup"><span data-stu-id="974d2-157">If the bundle has no children, it will return an empty collection.</span></span>

<span data-ttu-id="974d2-158">バンドル内の子の数が既定のページサイズよりも大きい場合は、**子の @ Odata リンク**プロパティが、バンドル内の子の次のページを要求するために使用できる URL を使用して返されます。</span><span class="sxs-lookup"><span data-stu-id="974d2-158">If the number of children in the bundle is greater than the default page size, the **children@odata.nextLink** property will be returned with a URL that can be used to request the next page of children in the bundle.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "101230100alkc",
  "name": "My Cool Day at the Beach",
  "children": [
    { "id": "120100abab", "name": "image1.jpg", "file": {} },
    { "id": "120100abo1", "name": "image2.jpg", "file": {} }
  ],
  "children@odata.nextLink": "https://api.onedrive.com/v1.0/..."
}
```

<span data-ttu-id="974d2-159">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="974d2-159">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="974d2-160">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="974d2-160">All the properties will be returned from an actual call.</span></span>


[バンドル]: ../resources/bundle.md
[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md
[error-response]: /graph/errors
[odata-parameters]: /graph/query-parameters


<!-- {
  "type": "#page.annotation",
  "description": "Retrieve metadata about a bundle and its children in OneDrive",
  "keywords": "retrieve,item,bundle,metadata",
  "section": "documentation",
  "tocPath": "Bundles/Get Bundle Metadata"
} -->
