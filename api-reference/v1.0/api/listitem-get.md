---
author: JeremyKelley
ms.author: JeremyKelley
title: listItem を取得
description: SharePoint リスト内の item のメタデータを返します。
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: a498947002247541bebf4fc7cd24147a0ca0df7a
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33968787"
---
# <a name="get-listitem"></a><span data-ttu-id="37ca1-103">listItem を取得</span><span class="sxs-lookup"><span data-stu-id="37ca1-103">Get listItem</span></span>

<span data-ttu-id="37ca1-104">[list][] 内の [item][] のメタデータを返します。</span><span class="sxs-lookup"><span data-stu-id="37ca1-104">Returns the metadata for an [item][] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="37ca1-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="37ca1-107">Permissions</span></span>

<span data-ttu-id="37ca1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="37ca1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37ca1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="37ca1-110">Permission type</span></span>      | <span data-ttu-id="37ca1-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="37ca1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37ca1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="37ca1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="37ca1-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37ca1-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="37ca1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="37ca1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37ca1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37ca1-115">Not supported.</span></span>    |
|<span data-ttu-id="37ca1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="37ca1-116">Application</span></span> | <span data-ttu-id="37ca1-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37ca1-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37ca1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="37ca1-118">HTTP request</span></span>

<span data-ttu-id="37ca1-119">listItemを取得</span><span class="sxs-lookup"><span data-stu-id="37ca1-119">Get a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
<span data-ttu-id="37ca1-120">リスト アイテムの列の値を取得します。</span><span class="sxs-lookup"><span data-stu-id="37ca1-120">Get the column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
<span data-ttu-id="37ca1-121">リスト アイテムの特定の列の値を取得します。</span><span class="sxs-lookup"><span data-stu-id="37ca1-121">Get specific column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```
## <a name="optional-query-parameters"></a><span data-ttu-id="37ca1-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="37ca1-122">Optional query parameters</span></span>
<span data-ttu-id="37ca1-123">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="37ca1-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37ca1-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="37ca1-124">Request headers</span></span>

| <span data-ttu-id="37ca1-125">名前</span><span class="sxs-lookup"><span data-stu-id="37ca1-125">Name</span></span>      |<span data-ttu-id="37ca1-126">説明</span><span class="sxs-lookup"><span data-stu-id="37ca1-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="37ca1-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="37ca1-127">Authorization</span></span>  | <span data-ttu-id="37ca1-128">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="37ca1-128">Bearer {code}.</span></span> <span data-ttu-id="37ca1-129">必須です。</span><span class="sxs-lookup"><span data-stu-id="37ca1-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="37ca1-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="37ca1-130">Request body</span></span>

<span data-ttu-id="37ca1-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="37ca1-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37ca1-132">応答</span><span class="sxs-lookup"><span data-stu-id="37ca1-132">Response</span></span> 

<span data-ttu-id="37ca1-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [item][] を返します。</span><span class="sxs-lookup"><span data-stu-id="37ca1-133">If successful, this method returns a `200 OK` response code and an updated [notificationMessageTemplate][] object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37ca1-134">例</span><span class="sxs-lookup"><span data-stu-id="37ca1-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="37ca1-135">要求</span><span class="sxs-lookup"><span data-stu-id="37ca1-135">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="37ca1-136">応答</span><span class="sxs-lookup"><span data-stu-id="37ca1-136">Response</span></span>

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

#### <a name="sdk-sample-code"></a><span data-ttu-id="37ca1-137">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="37ca1-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="37ca1-138">C#</span><span class="sxs-lookup"><span data-stu-id="37ca1-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-list-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="37ca1-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="37ca1-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-list-item-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
