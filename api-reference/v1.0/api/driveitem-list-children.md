---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: フォルダーの内容を一覧表示する
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 1e5fea5d1ac036ffc8498e9c4eee1315074f00b4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891209"
---
# <a name="list-children-of-a-driveitem"></a><span data-ttu-id="c4a85-102">driveItem の子を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c4a85-102">List children of a driveItem</span></span>

<span data-ttu-id="c4a85-103">DriveItem の**子**リレーションシップで [DriveItems](../resources/driveitem.md) のコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="c4a85-103">Return a collection of [DriveItems](../resources/driveitem.md) in the **children** relationship of a DriveItem.</span></span>

<span data-ttu-id="c4a85-104">NULL でない **folder** または **package** ファセットがある DriveItems は、1 つ以上の子 DriveItems を持つことができます。</span><span class="sxs-lookup"><span data-stu-id="c4a85-104">DriveItems with a non-null **folder** or **package** facet can have one or more child DriveItems.</span></span>


## <a name="permissions"></a><span data-ttu-id="c4a85-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c4a85-105">Permissions</span></span>

<span data-ttu-id="c4a85-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c4a85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4a85-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c4a85-108">Permission type</span></span>      | <span data-ttu-id="c4a85-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c4a85-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4a85-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c4a85-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c4a85-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4a85-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c4a85-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c4a85-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4a85-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4a85-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c4a85-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c4a85-114">Application</span></span> | <span data-ttu-id="c4a85-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4a85-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4a85-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c4a85-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/items/{item-id}/children
GET /me/drive/items/{item-id}/children
GET /sites/{site-id}/drive/items/{item-id}/children
GET /users/{user-id}/drive/items/{item-id}/children
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4a85-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c4a85-117">Optional query parameters</span></span>

<span data-ttu-id="c4a85-118">このメソッドは、応答をカスタマイズするための `$expand`、`$select`、`$skipToken`、`$top`、`$orderby` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c4a85-118">This method supports the `$expand`, `$select`, `$skipToken`, `$top` and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

### <a name="optional-request-headers"></a><span data-ttu-id="c4a85-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c4a85-119">Optional request headers</span></span>

| <span data-ttu-id="c4a85-120">名前</span><span class="sxs-lookup"><span data-stu-id="c4a85-120">Name</span></span>     | <span data-ttu-id="c4a85-121">値</span><span class="sxs-lookup"><span data-stu-id="c4a85-121">Value</span></span> | <span data-ttu-id="c4a85-122">説明</span><span class="sxs-lookup"><span data-stu-id="c4a85-122">Description</span></span>                                                                                                                                              |
|:----------------|:------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c4a85-123">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="c4a85-123">_if-none-match_</span></span> | <span data-ttu-id="c4a85-124">etag</span><span class="sxs-lookup"><span data-stu-id="c4a85-124">etag</span></span>  | <span data-ttu-id="c4a85-125">この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="c4a85-125">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="examples"></a><span data-ttu-id="c4a85-126">例</span><span class="sxs-lookup"><span data-stu-id="c4a85-126">Examples</span></span>

### <a name="list-children-in-the-root-of-the-current-users-drive"></a><span data-ttu-id="c4a85-127">現在のユーザーのドライブのルートの子を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c4a85-127">List children in the root of the current user's drive</span></span>

<span data-ttu-id="c4a85-128">ドライブのルートのファイルを取得するには、ドライブ上の `root` リレーションシップを使用して、子のリレーションシップにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="c4a85-128">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c4a85-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4a85-129">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-children-root", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/root/children
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c4a85-130">C#</span><span class="sxs-lookup"><span data-stu-id="c4a85-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-children-root-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c4a85-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="c4a85-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-children-root-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c4a85-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4a85-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-children-root-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c4a85-133">Java</span><span class="sxs-lookup"><span data-stu-id="c4a85-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-children-root-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="list-children-of-a-driveitem-with-a-known-id"></a><span data-ttu-id="c4a85-134">既知の ID を持つ DriveItem の子を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c4a85-134">List children of a DriveItem with a known ID</span></span>

<span data-ttu-id="c4a85-135">ドライブのルートのファイルを取得するには、ドライブ上の `root` リレーションシップを使用して、子のリレーションシップにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="c4a85-135">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c4a85-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4a85-136">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-children-files", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c4a85-137">C#</span><span class="sxs-lookup"><span data-stu-id="c4a85-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-children-files-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c4a85-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="c4a85-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-children-files-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c4a85-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4a85-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-children-files-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c4a85-140">Java</span><span class="sxs-lookup"><span data-stu-id="c4a85-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-children-files-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="list-children-of-a-driveitem-with-a-known-path"></a><span data-ttu-id="c4a85-141">既知のパスを持つ DriveItem の子を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c4a85-141">List children of a DriveItem with a known path</span></span>

<!-- { "blockType": "request", "name": "list-children-from-path", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/root:/{path-relative-to-root}:/children
```

## <a name="response"></a><span data-ttu-id="c4a85-142">応答</span><span class="sxs-lookup"><span data-stu-id="c4a85-142">Response</span></span>

<span data-ttu-id="c4a85-143">成功すると、このメソッドはターゲット アイテムの子コレクション内にあるアイテムの一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="c4a85-143">If successful, this method returns the list of items in the children collection of the target item.</span></span>
<span data-ttu-id="c4a85-144">子コレクションは、[driveItem][item-resource] リソースで構成されます。</span><span class="sxs-lookup"><span data-stu-id="c4a85-144">The children collection will be composed of [driveItem][item-resource] resources.</span></span>

<!-- { "blockType": "response", 
       "@odata.type": "Collection(microsoft.graph.driveItem)", 
       "truncated": true,
       "name": [ "list-children-root", "list-children-files", "list-children-from-path" ] } -->

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

<span data-ttu-id="c4a85-145">**注:** コレクションが既定のページ サイズ (200 アイテム) を超えた場合は、応答で **@odata.nextLink** プロパティが返され、より多くのアイテムが使用できることが示されます。また、アイテムの次のページの要求 URL も提供されます。</span><span class="sxs-lookup"><span data-stu-id="c4a85-145">**Note:** If a collection exceeds the default page size (200 items), the **@odata.nextLink** property is returned in the response to indicate more items are available and provide the request URL for the next page of items.</span></span>

<span data-ttu-id="c4a85-146">ページ サイズは[オプションのクエリ文字列パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)で制御できます。</span><span class="sxs-lookup"><span data-stu-id="c4a85-146">You can control the page size through [optional query string parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters)</span></span>

### <a name="error-responses"></a><span data-ttu-id="c4a85-147">エラー応答</span><span class="sxs-lookup"><span data-stu-id="c4a85-147">Error responses</span></span>

<span data-ttu-id="c4a85-148">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c4a85-148">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "Items/List children",
  "suppressions": [
  ]
} -->
