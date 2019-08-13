---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ファイルを検索する
localization_priority: Priority
ms.prod: sharepoint
description: クエリと一致するアイテムを対象にアイテムの階層を検索します。
doc_type: apiPageType
ms.openlocfilehash: 46f24b88ba22d71789b8d5d9afe38626e050076e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367249"
---
# <a name="search-for-a-driveitems-within-a-drive"></a><span data-ttu-id="eefd9-103">ドライブ内の DriveItems を検索する</span><span class="sxs-lookup"><span data-stu-id="eefd9-103">Search for a DriveItems within a drive</span></span>

<span data-ttu-id="eefd9-104">クエリと一致するアイテムを対象にアイテムの階層を検索します。</span><span class="sxs-lookup"><span data-stu-id="eefd9-104">Search the hierarchy of items for items matching a query.</span></span>
<span data-ttu-id="eefd9-105">フォルダー階層内、ドライブ全体、現在のユーザーと共有されるファイル内で検索できます。</span><span class="sxs-lookup"><span data-stu-id="eefd9-105">You can search within a folder hierarchy, a whole drive, or files shared with the current user.</span></span>

## <a name="permissions"></a><span data-ttu-id="eefd9-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="eefd9-106">Permissions</span></span>

<span data-ttu-id="eefd9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eefd9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eefd9-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eefd9-109">Permission type</span></span>      | <span data-ttu-id="eefd9-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="eefd9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eefd9-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eefd9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="eefd9-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eefd9-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="eefd9-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eefd9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eefd9-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eefd9-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="eefd9-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eefd9-115">Application</span></span> | <span data-ttu-id="eefd9-116">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eefd9-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eefd9-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eefd9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/search(q='{search-text}')
GET /groups/{group-id}/drive/root/search(q='{search-text}')
GET /me/drive/root/search(q='{search-text}')
GET /sites/{site-id}/drive/root/search(q='{search-text}')
GET /users/{user-id}/drive/root/search(q='{search-text}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eefd9-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="eefd9-118">Optional query parameters</span></span>

<span data-ttu-id="eefd9-119">このメソッドは、応答をカスタマイズするための `$expand`、`$select`、`$skipToken`、`$top`、`$orderby` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="eefd9-119">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="eefd9-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="eefd9-120">Function parameters</span></span>

| <span data-ttu-id="eefd9-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="eefd9-121">Parameter</span></span> | <span data-ttu-id="eefd9-122">型</span><span class="sxs-lookup"><span data-stu-id="eefd9-122">Type</span></span>  | <span data-ttu-id="eefd9-123">説明</span><span class="sxs-lookup"><span data-stu-id="eefd9-123">Description</span></span>                                                                                                                          |
|:-----|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="eefd9-124">q</span><span class="sxs-lookup"><span data-stu-id="eefd9-124">q</span></span>  | <span data-ttu-id="eefd9-125">string</span><span class="sxs-lookup"><span data-stu-id="eefd9-125">string</span></span> | <span data-ttu-id="eefd9-p103">アイテムの検索に使用するクエリ テキスト。値は、ファイル名、メタデータ、およびファイルのコンテンツを含む複数のフィールドに渡って照合できます。</span><span class="sxs-lookup"><span data-stu-id="eefd9-p103">The query text used to search for items. Values may be matched across several fields including filename, metadata, and file content.</span></span> |

## <a name="example"></a><span data-ttu-id="eefd9-128">例</span><span class="sxs-lookup"><span data-stu-id="eefd9-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="eefd9-129">要求</span><span class="sxs-lookup"><span data-stu-id="eefd9-129">Request</span></span>

<span data-ttu-id="eefd9-130">ここでは、現在のユーザーの OneDrive を検索する要求の例を示します。</span><span class="sxs-lookup"><span data-stu-id="eefd9-130">Here is an example of the request searching the current user's OneDrive</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="eefd9-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="eefd9-131">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "item_search", "tags": "service.graph" }-->

```http
GET /me/drive/root/search(q='{search-query}')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="eefd9-132">C#</span><span class="sxs-lookup"><span data-stu-id="eefd9-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/item-search-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eefd9-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eefd9-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/item-search-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="eefd9-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eefd9-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/item-search-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="eefd9-135">Java</span><span class="sxs-lookup"><span data-stu-id="eefd9-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/item-search-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eefd9-136">応答</span><span class="sxs-lookup"><span data-stu-id="eefd9-136">Response</span></span>

<span data-ttu-id="eefd9-p104">このメソッドは、検索条件に一致する [DriveItems](../resources/driveitem.md) のコレクション含んでいるオブジェクトを返します。アイテムが見つからない場合は、空のコレクションが返されます。</span><span class="sxs-lookup"><span data-stu-id="eefd9-p104">This method returns an object containing an collection of [DriveItems](../resources/driveitem.md) that match the search criteria. If no items were found, an empty collection is returned.</span></span>

<span data-ttu-id="eefd9-p105">一致が多すぎる場合は、応答はページ化され、**@odata.nextLink** プロパティには、後続の結果ページへの URL が含まれます。`$top` クエリ パラメーターを使用すると、ページ内のアイテム数を指定できます。</span><span class="sxs-lookup"><span data-stu-id="eefd9-p105">If there are too many matches the response will be paged and an **@odata.nextLink** property will contain a URL to the next page of results. You can use the `$top` query parameter to specify the number of items in the page.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```

## <a name="searching-for-items-a-user-can-access"></a><span data-ttu-id="eefd9-141">ユーザーがアクセスできるアイテムの検索</span><span class="sxs-lookup"><span data-stu-id="eefd9-141">Searching for items a user can access</span></span>

<span data-ttu-id="eefd9-p106">ドライブ内のアイテムの検索に加えて、アプリでは現在のユーザーと共有されるアイテムを含めるように、検索範囲を広げることができます。検索範囲を広げるには、[Drive](../resources/drive.md) リソースの **search** メソッドを使用します。</span><span class="sxs-lookup"><span data-stu-id="eefd9-p106">In addition to searching for items within a drive, your app can search more broadly to include items shared with the current user. To broaden the search scope, use the **search** method on the [Drive](../resources/drive.md) resource.</span></span>

### <a name="example"></a><span data-ttu-id="eefd9-144">例</span><span class="sxs-lookup"><span data-stu-id="eefd9-144">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="eefd9-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="eefd9-145">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "item_search_all", "tags": "service.graph" }-->

```http
GET /me/drive/search(q='{search-query}')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="eefd9-146">C#</span><span class="sxs-lookup"><span data-stu-id="eefd9-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/item-search-all-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eefd9-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eefd9-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/item-search-all-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="eefd9-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eefd9-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/item-search-all-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="eefd9-149">Java</span><span class="sxs-lookup"><span data-stu-id="eefd9-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/item-search-all-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eefd9-150">応答</span><span class="sxs-lookup"><span data-stu-id="eefd9-150">Response</span></span>

<span data-ttu-id="eefd9-p107">**ドライブ** リソースからの検索時の応答には、ドライブの外部のアイテム (現在のユーザーと共有されているアイテム) が含まれていることがあります。こうしたアイテムには、それらが対象のドライブの外部に保存されていることを示す、[**remoteItem**](../resources/remoteitem.md) ファセットが含まれます。</span><span class="sxs-lookup"><span data-stu-id="eefd9-p107">Responses when searching from the **drive** resource may include items outside of the drive (items shared with the current user). These items will include the [**remoteItem**](../resources/remoteitem.md) facet to indicate they are stored outside of the target drive.</span></span> 

<!-- { "blockType": "response", "truncated": true, "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" },
        "remoteItem": { "id": "!23141901", "parentReference": { "driveId": "s!1020101jlkjl12lx" } }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```

## <a name="error-responses"></a><span data-ttu-id="eefd9-153">エラー応答</span><span class="sxs-lookup"><span data-stu-id="eefd9-153">Error responses</span></span>

<span data-ttu-id="eefd9-154">エラーがどのように返されるかの詳細については、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eefd9-154">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Search for a file across a OneDrive.",
  "keywords": "search,query,bing,filename,content",
  "section": "documentation",
  "tocPath": "Items/Search",
  "suppressions": [
  ]
} -->
