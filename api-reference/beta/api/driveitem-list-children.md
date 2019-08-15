---
author: JeremyKelley
description: DriveItem の子リレーションシップで DriveItems のコレクションを返します。
ms.date: 09/10/2017
title: フォルダーの内容を一覧表示する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 0f2fd43c752a3c072d7c031d9f9662bc75a2059f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416738"
---
# <a name="list-children-of-a-driveitem"></a><span data-ttu-id="4f3a6-103">driveItem の子を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="4f3a6-103">List children of a driveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f3a6-104">DriveItem の**子**リレーションシップで [DriveItems](../resources/driveitem.md) のコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="4f3a6-104">Return a collection of [DriveItems](../resources/driveitem.md) in the **children** relationship of a DriveItem.</span></span>

<span data-ttu-id="4f3a6-105">NULL でない **folder** または **package** ファセットがある DriveItems は、1 つ以上の子 DriveItems を持つことができます。</span><span class="sxs-lookup"><span data-stu-id="4f3a6-105">DriveItems with a non-null **folder** or **package** facet can have one or more child DriveItems.</span></span>


## <a name="permissions"></a><span data-ttu-id="4f3a6-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4f3a6-106">Permissions</span></span>

<span data-ttu-id="4f3a6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f3a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f3a6-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4f3a6-109">Permission type</span></span>      | <span data-ttu-id="4f3a6-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4f3a6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f3a6-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4f3a6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4f3a6-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f3a6-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4f3a6-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4f3a6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f3a6-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f3a6-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="4f3a6-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4f3a6-115">Application</span></span> | <span data-ttu-id="4f3a6-116">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f3a6-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f3a6-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4f3a6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/items/{item-id}/children
GET /me/drive/items/{item-id}/children
GET /sites/{site-id}/drive/items/{item-id}/children
GET /users/{user-id}/drive/items/{item-id}/children
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f3a6-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4f3a6-118">Optional query parameters</span></span>

<span data-ttu-id="4f3a6-119">このメソッドは、応答をカスタマイズするための `$expand`、`$select`、`$skipToken`、`$top`、`$orderby` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4f3a6-119">This method supports the `$expand`, `$select`, `$skipToken`, `$top` and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

### <a name="optional-request-headers"></a><span data-ttu-id="4f3a6-120">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4f3a6-120">Optional request headers</span></span>

| <span data-ttu-id="4f3a6-121">ヘッダー名</span><span class="sxs-lookup"><span data-stu-id="4f3a6-121">Header name</span></span>     | <span data-ttu-id="4f3a6-122">値</span><span class="sxs-lookup"><span data-stu-id="4f3a6-122">Value</span></span> | <span data-ttu-id="4f3a6-123">説明</span><span class="sxs-lookup"><span data-stu-id="4f3a6-123">Description</span></span>                                                                                                                                              |
|:----------------|:------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4f3a6-124">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="4f3a6-124">_if-none-match_</span></span> | <span data-ttu-id="4f3a6-125">etag</span><span class="sxs-lookup"><span data-stu-id="4f3a6-125">etag</span></span>  | <span data-ttu-id="4f3a6-126">この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="4f3a6-126">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="examples"></a><span data-ttu-id="4f3a6-127">例</span><span class="sxs-lookup"><span data-stu-id="4f3a6-127">Examples</span></span>

### <a name="list-children-in-the-root-of-the-current-users-drive"></a><span data-ttu-id="4f3a6-128">現在のユーザーのドライブのルートの子を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="4f3a6-128">List children in the root of the current user's drive</span></span>

<span data-ttu-id="4f3a6-129">ドライブのルートのファイルを取得するには、ドライブ上の `root` リレーションシップを使用し、子のリレーションシップにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="4f3a6-129">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4f3a6-130">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4f3a6-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-children-root", "scopes": "files.read" } -->

```http
GET /me/drive/root/children
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4f3a6-131">C#</span><span class="sxs-lookup"><span data-stu-id="4f3a6-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-children-root-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4f3a6-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f3a6-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-children-root-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4f3a6-133">目的-C</span><span class="sxs-lookup"><span data-stu-id="4f3a6-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-children-root-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="list-children-of-a-driveitem-with-a-known-id"></a><span data-ttu-id="4f3a6-134">既知の ID を持つ DriveItem の子を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="4f3a6-134">List children of a DriveItem with a known ID</span></span>

<span data-ttu-id="4f3a6-135">ドライブのルートのファイルを取得するには、ドライブ上の `root` リレーションシップを使用して、子のリレーションシップにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="4f3a6-135">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4f3a6-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4f3a6-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-children", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4f3a6-137">C#</span><span class="sxs-lookup"><span data-stu-id="4f3a6-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4f3a6-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f3a6-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4f3a6-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="4f3a6-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="list-children-of-a-driveitem-with-a-known-path"></a><span data-ttu-id="4f3a6-140">既知のパスを持つ DriveItem の子を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="4f3a6-140">List children of a DriveItem with a known path</span></span>

<!-- { "blockType": "request", "name": "list-children-from-path", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/root:/{path-relative-to-root}:/children
```

## <a name="response"></a><span data-ttu-id="4f3a6-141">応答</span><span class="sxs-lookup"><span data-stu-id="4f3a6-141">Response</span></span>

<span data-ttu-id="4f3a6-142">成功すると、このメソッドはターゲット アイテムの子コレクション内にあるアイテムの一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="4f3a6-142">If successful, this method returns the list of items in the children collection of the target item.</span></span>
<span data-ttu-id="4f3a6-143">子のコレクションは、[driveItem][item-resource] リソースで構成されます。</span><span class="sxs-lookup"><span data-stu-id="4f3a6-143">The children collection will be composed of [driveItem][item-resource] resources.</span></span>

<!-- { "blockType": "response", 
       "@odata.type": "Collection(microsoft.graph.driveItem)", 
       "truncated": true,
       "name": [ "list-children-root", "list-children", "list-children-from-path" ] } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {"name": "myfile.jpg", "size": 2048, "file": {} },
    {"name": "Documents", "folder": { "childCount": 4} },
    {"name": "Photos", "folder": { "childCount": 203} },
    {"name": "my sheet(1).xlsx", "size": 197 }
  ],
  "@odata.nextLink": "https://..."
}
```

<span data-ttu-id="4f3a6-144">**注:** コレクションが既定のページ サイズ (200 アイテム) を超えた場合は、応答で **@odata.nextLink** プロパティが返され、より多くのアイテムが使用できることが示されます。また、アイテムの次のページの要求 URL も提供されます。</span><span class="sxs-lookup"><span data-stu-id="4f3a6-144">**Note:** If a collection exceeds the default page size (200 items), the **@odata.nextLink** property is returned in the response to indicate more items are available and provide the request URL for the next page of items.</span></span>

<span data-ttu-id="4f3a6-145">ページ サイズは[オプションのクエリ文字列パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)で制御できます。</span><span class="sxs-lookup"><span data-stu-id="4f3a6-145">You can control the page size through [optional query string parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters)</span></span>

### <a name="error-responses"></a><span data-ttu-id="4f3a6-146">エラー応答</span><span class="sxs-lookup"><span data-stu-id="4f3a6-146">Error responses</span></span>

<span data-ttu-id="4f3a6-147">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f3a6-147">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "Items/List children",
  "suppressions": [
  ]
}
-->
