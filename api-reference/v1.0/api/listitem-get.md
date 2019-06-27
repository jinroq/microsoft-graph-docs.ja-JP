---
author: JeremyKelley
ms.author: JeremyKelley
title: listItem を取得
description: SharePoint リスト内の item のメタデータを返します。
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 57d95b67ff27ff58e26310db69f97c027d5e3639
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271996"
---
# <a name="get-listitem"></a><span data-ttu-id="7d8a0-103">listItem を取得</span><span class="sxs-lookup"><span data-stu-id="7d8a0-103">Get listItem</span></span>

<span data-ttu-id="7d8a0-104">[list][] 内の [item][] のメタデータを返します。</span><span class="sxs-lookup"><span data-stu-id="7d8a0-104">Returns the metadata for an [item][] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="7d8a0-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7d8a0-107">Permissions</span></span>

<span data-ttu-id="7d8a0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7d8a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d8a0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7d8a0-110">Permission type</span></span>      | <span data-ttu-id="7d8a0-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7d8a0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d8a0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7d8a0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7d8a0-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d8a0-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7d8a0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7d8a0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d8a0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d8a0-115">Not supported.</span></span>    |
|<span data-ttu-id="7d8a0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7d8a0-116">Application</span></span> | <span data-ttu-id="7d8a0-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d8a0-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d8a0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7d8a0-118">HTTP request</span></span>

<span data-ttu-id="7d8a0-119">listItemを取得</span><span class="sxs-lookup"><span data-stu-id="7d8a0-119">Get a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
<span data-ttu-id="7d8a0-120">リスト アイテムの列の値を取得します。</span><span class="sxs-lookup"><span data-stu-id="7d8a0-120">Get the column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
<span data-ttu-id="7d8a0-121">リスト アイテムの特定の列の値を取得します。</span><span class="sxs-lookup"><span data-stu-id="7d8a0-121">Get specific column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7d8a0-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7d8a0-122">Optional query parameters</span></span>
<span data-ttu-id="7d8a0-123">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7d8a0-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d8a0-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d8a0-124">Request headers</span></span>

| <span data-ttu-id="7d8a0-125">名前</span><span class="sxs-lookup"><span data-stu-id="7d8a0-125">Name</span></span>      |<span data-ttu-id="7d8a0-126">説明</span><span class="sxs-lookup"><span data-stu-id="7d8a0-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7d8a0-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d8a0-127">Authorization</span></span>  | <span data-ttu-id="7d8a0-128">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="7d8a0-128">Bearer {code}.</span></span> <span data-ttu-id="7d8a0-129">必須です。</span><span class="sxs-lookup"><span data-stu-id="7d8a0-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d8a0-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="7d8a0-130">Request body</span></span>

<span data-ttu-id="7d8a0-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7d8a0-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d8a0-132">応答</span><span class="sxs-lookup"><span data-stu-id="7d8a0-132">Response</span></span> 

<span data-ttu-id="7d8a0-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [item][] を返します。</span><span class="sxs-lookup"><span data-stu-id="7d8a0-133">If successful, this method returns a `200 OK` response code and an [item][] in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d8a0-134">例</span><span class="sxs-lookup"><span data-stu-id="7d8a0-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d8a0-135">要求</span><span class="sxs-lookup"><span data-stu-id="7d8a0-135">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="7d8a0-136">応答</span><span class="sxs-lookup"><span data-stu-id="7d8a0-136">Response</span></span>

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

#### <a name="sdk-sample-code"></a><span data-ttu-id="7d8a0-137">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="7d8a0-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7d8a0-138">C#</span><span class="sxs-lookup"><span data-stu-id="7d8a0-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-list-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7d8a0-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="7d8a0-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-list-item-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7d8a0-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d8a0-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-list-item-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
