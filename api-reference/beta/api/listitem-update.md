---
author: JeremyKelley
description: リストアイテム のプロパティを更新します。
ms.date: 09/11/2017
title: SharePoint リスト内のレコードを更新する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 9090d2bb3285e5b511b46855b937506b5c868be1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993033"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="1527b-103">リスト内のアイテムを更新する</span><span class="sxs-lookup"><span data-stu-id="1527b-103">Update an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1527b-104">**[listItem][]** のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1527b-104">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="1527b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1527b-105">Permissions</span></span>

<span data-ttu-id="1527b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1527b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1527b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1527b-108">Permission type</span></span>      | <span data-ttu-id="1527b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1527b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1527b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1527b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1527b-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1527b-111">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1527b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1527b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1527b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1527b-113">Not supported.</span></span>    |
|<span data-ttu-id="1527b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1527b-114">Application</span></span> | <span data-ttu-id="1527b-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1527b-115">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1527b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1527b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="1527b-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1527b-117">Optional request headers</span></span>

| <span data-ttu-id="1527b-118">名前</span><span class="sxs-lookup"><span data-stu-id="1527b-118">Name</span></span>       | <span data-ttu-id="1527b-119">値</span><span class="sxs-lookup"><span data-stu-id="1527b-119">Value</span></span> | <span data-ttu-id="1527b-120">説明</span><span class="sxs-lookup"><span data-stu-id="1527b-120">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="1527b-121">_if-match_</span><span class="sxs-lookup"><span data-stu-id="1527b-121">_if-match_</span></span> | <span data-ttu-id="1527b-122">etag</span><span class="sxs-lookup"><span data-stu-id="1527b-122">etag</span></span>  | <span data-ttu-id="1527b-123">この要求ヘッダーが含まれていて、指定された eTag がアイテムの現在の eTag に一致しない場合には、`412 Precondition Failed` 応答が返され、アイテムは更新されません。</span><span class="sxs-lookup"><span data-stu-id="1527b-123">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="1527b-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="1527b-124">Request body</span></span>

<span data-ttu-id="1527b-125">要求本文に、更新するフィールドを指定する [fieldValueSet][] の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1527b-125">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="1527b-126">例</span><span class="sxs-lookup"><span data-stu-id="1527b-126">Example</span></span>

<span data-ttu-id="1527b-127">ここでは、リスト アイテムの Color フィールドと Quantity フィールドを新しい値で更新する例を示します。</span><span class="sxs-lookup"><span data-stu-id="1527b-127">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="1527b-128">listItem の他の値はすべてそのままです。</span><span class="sxs-lookup"><span data-stu-id="1527b-128">All other values on the listItem are left alone.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="1527b-129">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1527b-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1527b-130">C#</span><span class="sxs-lookup"><span data-stu-id="1527b-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1527b-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="1527b-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1527b-132">目的-C</span><span class="sxs-lookup"><span data-stu-id="1527b-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1527b-133">Java</span><span class="sxs-lookup"><span data-stu-id="1527b-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="1527b-134">応答</span><span class="sxs-lookup"><span data-stu-id="1527b-134">Response</span></span>

<span data-ttu-id="1527b-135">成功した場合、このメソッドは更新されたリスト アイテムの応答本文で [fieldValueSet][] を返します。</span><span class="sxs-lookup"><span data-stu-id="1527b-135">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

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
