---
author: JeremyKelley
ms.author: jeremyke
title: リストバンドル
description: ユーザーのドライブのバンドルを一覧表示する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 1bfb1249c19e44f19e4cc39442ecf67d60e8f6aa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944834"
---
# <a name="list-bundles"></a><span data-ttu-id="659af-103">リストバンドル</span><span class="sxs-lookup"><span data-stu-id="659af-103">List bundles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="659af-104">ユーザーのドライブにあるすべての[バンドル][バンドル]のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="659af-104">Get a list of all the [bundles][bundle] in a user's drive.</span></span>

## <a name="permissions"></a><span data-ttu-id="659af-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="659af-105">Permissions</span></span>

<span data-ttu-id="659af-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="659af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="659af-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="659af-108">Permission type</span></span>      | <span data-ttu-id="659af-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="659af-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="659af-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="659af-110">Delegated (work or school account)</span></span> | <span data-ttu-id="659af-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="659af-111">Not supported.</span></span>                             |
|<span data-ttu-id="659af-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="659af-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="659af-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="659af-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="659af-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="659af-114">Application</span></span>          | <span data-ttu-id="659af-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="659af-115">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="659af-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="659af-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/bundles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="659af-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="659af-117">Optional query parameters</span></span>

<span data-ttu-id="659af-118">このメソッドは、応答をフィルター処理してシェイプするための [OData クエリ パラメーター][]をサポートします。</span><span class="sxs-lookup"><span data-stu-id="659af-118">This method supports the [OData Query Parameters][] to filter and shape the response.</span></span>

<span data-ttu-id="659af-119">バンドルの列挙時`expand=children`にクエリパラメーターを使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="659af-119">You can't use the `expand=children` query parameter when enumerating bundles.</span></span>

## <a name="request-headers"></a><span data-ttu-id="659af-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="659af-120">Request headers</span></span>

| <span data-ttu-id="659af-121">名前</span><span class="sxs-lookup"><span data-stu-id="659af-121">Name</span></span>          | <span data-ttu-id="659af-122">説明</span><span class="sxs-lookup"><span data-stu-id="659af-122">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="659af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="659af-123">Authorization</span></span> | <span data-ttu-id="659af-124">ベアラー \{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="659af-124">Bearer \{token\}.</span></span> <span data-ttu-id="659af-125">必須です。</span><span class="sxs-lookup"><span data-stu-id="659af-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="659af-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="659af-126">Request body</span></span>

<span data-ttu-id="659af-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="659af-127">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="659af-128">応答</span><span class="sxs-lookup"><span data-stu-id="659af-128">Response</span></span>

<span data-ttu-id="659af-129">成功した場合、この要求はドライブに対して定義されたバンドルアイテムの一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="659af-129">If successful, this request returns the list of bundle items defined for the drive.</span></span>

<span data-ttu-id="659af-130">エラーがどのように返されるかに関する詳細については、「[エラー応答][error-response]」のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="659af-130">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="659af-131">例</span><span class="sxs-lookup"><span data-stu-id="659af-131">Examples</span></span>

### <a name="example-1-list-all-bundles-in-a-drive"></a><span data-ttu-id="659af-132">例 1: ドライブ内のすべてのバンドルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="659af-132">Example 1: List all bundles in a drive</span></span>

<span data-ttu-id="659af-133">ドライブで定義されているすべてのバンドルの列挙を要求するには、パラメーターを使用せずに、**バンドル**コレクションに対して要求を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="659af-133">To request an enumeration of all bundles defined in the drive, you can make a request to the **bundles** collection without any parameters.</span></span>

#### <a name="request"></a><span data-ttu-id="659af-134">要求</span><span class="sxs-lookup"><span data-stu-id="659af-134">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="659af-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="659af-135">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-all-bundles", "tags": "service.onedrive" } -->

```http
GET https://graph.microsoft.com/beta/drive/bundles
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="659af-136">C#</span><span class="sxs-lookup"><span data-stu-id="659af-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-all-bundles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="659af-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="659af-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-all-bundles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="659af-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="659af-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-all-bundles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="659af-139">Java</span><span class="sxs-lookup"><span data-stu-id="659af-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-all-bundles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="659af-140">応答</span><span class="sxs-lookup"><span data-stu-id="659af-140">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true, "isCollection": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "0123456789abc",
      "name": "Vacation photo album",
      "bundle": {
        "childCount": 1,
        "album": { }
      }
    },
    {
      "id": "0120310201abd",
      "name": "Family shared files",
      "bundle": {
        "childCount": 1
      }
    }
  ],
  "@odata.nextLink": "https://..."
}
```

<span data-ttu-id="659af-141">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="659af-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="659af-142">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="659af-142">All the properties will be returned from an actual call.</span></span>


### <a name="example-2-list-all-photo-albums-in-a-drive"></a><span data-ttu-id="659af-143">例 2: ドライブ内のすべてのフォトアルバムを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="659af-143">Example 2: List all photo albums in a drive</span></span>

<span data-ttu-id="659af-144">要求からバンドルコレクションに返されるバンドルの一覧をフィルター処理するには、 `filter`クエリ文字列パラメーターを使用して、バンドルのファセットが存在するかどうかを確認することで、返すバンドルの種類を指定できます。</span><span class="sxs-lookup"><span data-stu-id="659af-144">To filter the list of bundles returned from a request to the bundles collection, you can use the `filter` query string parameter to specify the type of bundle to return by checking for the existence of a facet on the bundle:</span></span>

#### <a name="request"></a><span data-ttu-id="659af-145">要求</span><span class="sxs-lookup"><span data-stu-id="659af-145">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="659af-146">プロトコル</span><span class="sxs-lookup"><span data-stu-id="659af-146">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "list-album-bundles", "tags": "service.onedrive" } -->

```http
GET https://graph.microsoft.com/beta/drive/bundles?filter=bundle/album%20ne%20null
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="659af-147">C#</span><span class="sxs-lookup"><span data-stu-id="659af-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-album-bundles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="659af-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="659af-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-album-bundles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="659af-149">目的-C</span><span class="sxs-lookup"><span data-stu-id="659af-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-album-bundles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="659af-150">Java</span><span class="sxs-lookup"><span data-stu-id="659af-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-album-bundles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="659af-151">応答</span><span class="sxs-lookup"><span data-stu-id="659af-151">Response</span></span>

<span data-ttu-id="659af-152">バンドルエンドポイントへの GET に対する応答は、[バンドル][]を含む、[ドライブ項目][]リソースの配列です。</span><span class="sxs-lookup"><span data-stu-id="659af-152">The response to a GET to the bundles endpoint is an array of [driveItem][] resources with the [bundle][].</span></span>
<span data-ttu-id="659af-153">すべてのバンドルはアイテムなので、これらのすべての標準アイテム操作を使用できます。</span><span class="sxs-lookup"><span data-stu-id="659af-153">Because all bundles are items, you can use use all the standard item operations on them.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true, "isCollection": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "0123456789abc",
      "name": "Vacation photo album",
      "bundle": {
        "childCount": 1,
        "album": { }
      }
    },
    {
      "id": "120301010abcd",
      "name": "Seattle Center event",
      "bundle": {
        "childCount": 4,
        "album": { }
      },
      "tags": [
        {
          "name": "outside",
          "autoTagged": { }
        }
      ]
    }
  ]
}
```

<span data-ttu-id="659af-154">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="659af-154">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="659af-155">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="659af-155">All the properties will be returned from an actual call.</span></span>


[バンドル]: ../resources/bundle.md
[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md
[error-response]: /graph/errors
[OData クエリパラメーター]: /graph/query-parameters
[OData Query Parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "List the bundles in a drive.",
  "keywords": "list,bundle,collection",
  "section": "documentation",
  "tocPath": "Bundles/List"
} -->
