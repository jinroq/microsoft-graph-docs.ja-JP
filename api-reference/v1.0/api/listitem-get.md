---
author: JeremyKelley
ms.author: JeremyKelley
title: listItem を取得
description: SharePoint リスト内の item のメタデータを返します。
localization_priority: Priority
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 458b8e71f8561c6a96177bac38c8ed450110ee24
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370679"
---
# <a name="get-listitem"></a><span data-ttu-id="53b5c-103">listItem を取得</span><span class="sxs-lookup"><span data-stu-id="53b5c-103">Get listItem</span></span>

<span data-ttu-id="53b5c-104">[list][] 内の [item][] のメタデータを返します。</span><span class="sxs-lookup"><span data-stu-id="53b5c-104">Returns the metadata for an [item][] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="53b5c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="53b5c-107">Permissions</span></span>

<span data-ttu-id="53b5c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="53b5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53b5c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="53b5c-110">Permission type</span></span>      | <span data-ttu-id="53b5c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="53b5c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53b5c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="53b5c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="53b5c-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53b5c-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="53b5c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="53b5c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53b5c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53b5c-115">Not supported.</span></span>    |
|<span data-ttu-id="53b5c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="53b5c-116">Application</span></span> | <span data-ttu-id="53b5c-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53b5c-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53b5c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="53b5c-118">HTTP request</span></span>

<span data-ttu-id="53b5c-119">listItemを取得</span><span class="sxs-lookup"><span data-stu-id="53b5c-119">Get a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
<span data-ttu-id="53b5c-120">リスト アイテムの列の値を取得します。</span><span class="sxs-lookup"><span data-stu-id="53b5c-120">Get the column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
<span data-ttu-id="53b5c-121">リスト アイテムの特定の列の値を取得します。</span><span class="sxs-lookup"><span data-stu-id="53b5c-121">Get specific column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```
## <a name="optional-query-parameters"></a><span data-ttu-id="53b5c-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="53b5c-122">Optional query parameters</span></span>
<span data-ttu-id="53b5c-123">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="53b5c-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="53b5c-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53b5c-124">Request headers</span></span>

| <span data-ttu-id="53b5c-125">名前</span><span class="sxs-lookup"><span data-stu-id="53b5c-125">Name</span></span>      |<span data-ttu-id="53b5c-126">説明</span><span class="sxs-lookup"><span data-stu-id="53b5c-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="53b5c-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="53b5c-127">Authorization</span></span>  | <span data-ttu-id="53b5c-128">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="53b5c-128">Bearer {code}.</span></span> <span data-ttu-id="53b5c-129">必須です。</span><span class="sxs-lookup"><span data-stu-id="53b5c-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="53b5c-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="53b5c-130">Request body</span></span>

<span data-ttu-id="53b5c-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="53b5c-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53b5c-132">応答</span><span class="sxs-lookup"><span data-stu-id="53b5c-132">Response</span></span> 

<span data-ttu-id="53b5c-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [item][] を返します。</span><span class="sxs-lookup"><span data-stu-id="53b5c-133">If successful, this method returns a `200 OK` response code and an [item][] in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53b5c-134">例</span><span class="sxs-lookup"><span data-stu-id="53b5c-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="53b5c-135">要求</span><span class="sxs-lookup"><span data-stu-id="53b5c-135">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="53b5c-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="53b5c-136">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="53b5c-137">C#</span><span class="sxs-lookup"><span data-stu-id="53b5c-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="53b5c-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53b5c-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="53b5c-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53b5c-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="53b5c-140">Java</span><span class="sxs-lookup"><span data-stu-id="53b5c-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="53b5c-141">応答</span><span class="sxs-lookup"><span data-stu-id="53b5c-141">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "5",
  "fields": {
    "Name": "Widget",
    "Color": "Blue",
    "Quantity": 2357
    }
}
```


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
  ]
} -->
