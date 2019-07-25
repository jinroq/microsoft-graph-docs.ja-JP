---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: フォルダーの内容を一覧表示する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: db11d1bb36e608a477669ec174ef8bdb09dbdf55
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861119"
---
# <a name="list-children-of-a-driveitem"></a><span data-ttu-id="7ffee-102">driveItem の子を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7ffee-102">List children of a driveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ffee-103">DriveItem の**子**リレーションシップで [DriveItems](../resources/driveitem.md) のコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7ffee-103">Return a collection of [DriveItems](../resources/driveitem.md) in the **children** relationship of a DriveItem.</span></span>

<span data-ttu-id="7ffee-104">NULL でない **folder** または **package** ファセットがある DriveItems は、1 つ以上の子 DriveItems を持つことができます。</span><span class="sxs-lookup"><span data-stu-id="7ffee-104">DriveItems with a non-null **folder** or **package** facet can have one or more child DriveItems.</span></span>


## <a name="permissions"></a><span data-ttu-id="7ffee-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7ffee-105">Permissions</span></span>

<span data-ttu-id="7ffee-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7ffee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ffee-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7ffee-108">Permission type</span></span>      | <span data-ttu-id="7ffee-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7ffee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ffee-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7ffee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7ffee-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ffee-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7ffee-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7ffee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ffee-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ffee-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="7ffee-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7ffee-114">Application</span></span> | <span data-ttu-id="7ffee-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ffee-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ffee-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7ffee-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/items/{item-id}/children
GET /me/drive/items/{item-id}/children
GET /sites/{site-id}/drive/items/{item-id}/children
GET /users/{user-id}/drive/items/{item-id}/children
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7ffee-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7ffee-117">Optional query parameters</span></span>

<span data-ttu-id="7ffee-118">このメソッドは、応答をカスタマイズするための `$expand`、`$select`、`$skipToken`、`$top`、`$orderby` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7ffee-118">This method supports the `$expand`, `$select`, `$skipToken`, `$top` and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

### <a name="optional-request-headers"></a><span data-ttu-id="7ffee-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7ffee-119">Optional request headers</span></span>

| <span data-ttu-id="7ffee-120">ヘッダー名</span><span class="sxs-lookup"><span data-stu-id="7ffee-120">Header name</span></span>     | <span data-ttu-id="7ffee-121">値</span><span class="sxs-lookup"><span data-stu-id="7ffee-121">Value</span></span> | <span data-ttu-id="7ffee-122">説明</span><span class="sxs-lookup"><span data-stu-id="7ffee-122">Description</span></span>                                                                                                                                              |
|:----------------|:------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="7ffee-123">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="7ffee-123">_if-none-match_</span></span> | <span data-ttu-id="7ffee-124">etag</span><span class="sxs-lookup"><span data-stu-id="7ffee-124">etag</span></span>  | <span data-ttu-id="7ffee-125">この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="7ffee-125">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="examples"></a><span data-ttu-id="7ffee-126">例</span><span class="sxs-lookup"><span data-stu-id="7ffee-126">Examples</span></span>

### <a name="list-children-in-the-root-of-the-current-users-drive"></a><span data-ttu-id="7ffee-127">現在のユーザーのドライブのルートの子を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7ffee-127">List children in the root of the current user's drive</span></span>

<span data-ttu-id="7ffee-128">ドライブのルートのファイルを取得するには、ドライブ上の `root` リレーションシップを使用して、子のリレーションシップにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="7ffee-128">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7ffee-129">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7ffee-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-children-root", "scopes": "files.read" } -->

```http
GET /me/drive/root/children
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7ffee-130">C#</span><span class="sxs-lookup"><span data-stu-id="7ffee-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-children-root-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7ffee-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="7ffee-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-children-root-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7ffee-132">目的-C</span><span class="sxs-lookup"><span data-stu-id="7ffee-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-children-root-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7ffee-133">Java</span><span class="sxs-lookup"><span data-stu-id="7ffee-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-children-root-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="list-children-of-a-driveitem-with-a-known-id"></a><span data-ttu-id="7ffee-134">既知の ID を持つ DriveItem の子を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7ffee-134">List children of a DriveItem with a known ID</span></span>

<span data-ttu-id="7ffee-135">ドライブのルートのファイルを取得するには、ドライブ上の `root` リレーションシップを使用して、子のリレーションシップにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="7ffee-135">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7ffee-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7ffee-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-children", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7ffee-137">C#</span><span class="sxs-lookup"><span data-stu-id="7ffee-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7ffee-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="7ffee-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7ffee-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="7ffee-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7ffee-140">Java</span><span class="sxs-lookup"><span data-stu-id="7ffee-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-children-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="list-children-of-a-driveitem-with-a-known-path"></a><span data-ttu-id="7ffee-141">既知のパスを持つ DriveItem の子を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7ffee-141">List children of a DriveItem with a known path</span></span>

<!-- { "blockType": "request", "name": "list-children-from-path", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/root:/{path-relative-to-root}:/children
```

## <a name="response"></a><span data-ttu-id="7ffee-142">応答</span><span class="sxs-lookup"><span data-stu-id="7ffee-142">Response</span></span>

<span data-ttu-id="7ffee-143">成功すると、このメソッドはターゲット アイテムの子コレクション内にあるアイテムの一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="7ffee-143">If successful, this method returns the list of items in the children collection of the target item.</span></span>
<span data-ttu-id="7ffee-144">子のコレクションは、[driveItem][item-resource] リソースで構成されます。</span><span class="sxs-lookup"><span data-stu-id="7ffee-144">The children collection will be composed of [driveItem][item-resource] resources.</span></span>

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

<span data-ttu-id="7ffee-145">**注:** コレクションが既定のページ サイズ (200 アイテム) を超えた場合は、応答で **@odata.nextLink** プロパティが返され、より多くのアイテムが使用できることが示されます。また、アイテムの次のページの要求 URL も提供されます。</span><span class="sxs-lookup"><span data-stu-id="7ffee-145">**Note:** If a collection exceeds the default page size (200 items), the **@odata.nextLink** property is returned in the response to indicate more items are available and provide the request URL for the next page of items.</span></span>

<span data-ttu-id="7ffee-146">ページ サイズは[オプションのクエリ文字列パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)で制御できます。</span><span class="sxs-lookup"><span data-stu-id="7ffee-146">You can control the page size through [optional query string parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters)</span></span>

### <a name="error-responses"></a><span data-ttu-id="7ffee-147">エラー応答</span><span class="sxs-lookup"><span data-stu-id="7ffee-147">Error responses</span></span>

<span data-ttu-id="7ffee-148">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7ffee-148">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

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
