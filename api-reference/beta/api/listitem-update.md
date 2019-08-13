---
author: JeremyKelley
description: リストアイテム のプロパティを更新します。
ms.date: 09/11/2017
title: SharePoint リスト内のレコードを更新する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 4c2335b868184ee4e751a4d1e4adf19df501cf9c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342972"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="c1fa8-103">リスト内のアイテムを更新する</span><span class="sxs-lookup"><span data-stu-id="c1fa8-103">Update an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1fa8-104">**[listItem][]** のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c1fa8-104">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1fa8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c1fa8-105">Permissions</span></span>

<span data-ttu-id="c1fa8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c1fa8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1fa8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c1fa8-108">Permission type</span></span>      | <span data-ttu-id="c1fa8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c1fa8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1fa8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c1fa8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c1fa8-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1fa8-111">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c1fa8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c1fa8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1fa8-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1fa8-113">Not supported.</span></span>    |
|<span data-ttu-id="c1fa8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c1fa8-114">Application</span></span> | <span data-ttu-id="c1fa8-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1fa8-115">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1fa8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c1fa8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="c1fa8-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c1fa8-117">Optional request headers</span></span>

| <span data-ttu-id="c1fa8-118">名前</span><span class="sxs-lookup"><span data-stu-id="c1fa8-118">Name</span></span>       | <span data-ttu-id="c1fa8-119">値</span><span class="sxs-lookup"><span data-stu-id="c1fa8-119">Value</span></span> | <span data-ttu-id="c1fa8-120">説明</span><span class="sxs-lookup"><span data-stu-id="c1fa8-120">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="c1fa8-121">_if-match_</span><span class="sxs-lookup"><span data-stu-id="c1fa8-121">_if-match_</span></span> | <span data-ttu-id="c1fa8-122">etag</span><span class="sxs-lookup"><span data-stu-id="c1fa8-122">etag</span></span>  | <span data-ttu-id="c1fa8-123">この要求ヘッダーが含まれていて、指定された eTag がアイテムの現在の eTag に一致しない場合には、`412 Precondition Failed` 応答が返され、アイテムは更新されません。</span><span class="sxs-lookup"><span data-stu-id="c1fa8-123">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="c1fa8-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="c1fa8-124">Request body</span></span>

<span data-ttu-id="c1fa8-125">要求本文に、更新するフィールドを指定する [fieldValueSet][] の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c1fa8-125">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="c1fa8-126">例</span><span class="sxs-lookup"><span data-stu-id="c1fa8-126">Example</span></span>

<span data-ttu-id="c1fa8-127">ここでは、リスト アイテムの Color フィールドと Quantity フィールドを新しい値で更新する例を示します。</span><span class="sxs-lookup"><span data-stu-id="c1fa8-127">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="c1fa8-128">listItem の他の値はすべてそのままです。</span><span class="sxs-lookup"><span data-stu-id="c1fa8-128">All other values on the listItem are left alone.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="c1fa8-129">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c1fa8-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c1fa8-130">C#</span><span class="sxs-lookup"><span data-stu-id="c1fa8-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1fa8-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1fa8-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c1fa8-132">目的-C</span><span class="sxs-lookup"><span data-stu-id="c1fa8-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c1fa8-133">Java</span><span class="sxs-lookup"><span data-stu-id="c1fa8-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="c1fa8-134">応答</span><span class="sxs-lookup"><span data-stu-id="c1fa8-134">Response</span></span>

<span data-ttu-id="c1fa8-135">成功した場合、このメソッドは更新されたリスト アイテムの応答本文で [fieldValueSet][] を返します。</span><span class="sxs-lookup"><span data-stu-id="c1fa8-135">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "Name": "Widget",
  "Color": "Fuchsia",
  "Quantity": 934
}
```

[fieldValueSet]: ../resources/fieldvalueset.md
[listItem]: ../resources/listitem.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update",
  "suppressions": [
  ]
}
-->
