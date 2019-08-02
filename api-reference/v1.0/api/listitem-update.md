---
author: JeremyKelley
ms.author: JeremyKelley
title: リスト アイテムを更新します。
description: '**[listItem][]** のプロパティを更新します。'
localization_priority: Priority
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: d346e9aedf6a9c7061fcfc2e1093ed6257034345
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023126"
---
# <a name="update-listitem"></a><span data-ttu-id="fd997-103">リスト アイテムを更新します。</span><span class="sxs-lookup"><span data-stu-id="fd997-103">Update listItem</span></span>

<span data-ttu-id="fd997-104">**[listItem][]** のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fd997-104">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd997-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fd997-105">Permissions</span></span>

<span data-ttu-id="fd997-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fd997-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd997-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fd997-108">Permission type</span></span>      | <span data-ttu-id="fd997-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fd997-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd997-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fd997-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fd997-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd997-111">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="fd997-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fd997-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd997-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd997-113">Not supported.</span></span>    |
|<span data-ttu-id="fd997-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fd997-114">Application</span></span> | <span data-ttu-id="fd997-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd997-115">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd997-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fd997-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="fd997-117">リストアイテム のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fd997-117">Update the properties on a listItem.</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

<span data-ttu-id="fd997-118">リスト アイテムの列の値を更新します。</span><span class="sxs-lookup"><span data-stu-id="fd997-118">Update column values on a listItem.</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="fd997-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fd997-119">Optional request headers</span></span>

| <span data-ttu-id="fd997-120">名前</span><span class="sxs-lookup"><span data-stu-id="fd997-120">Name</span></span>       | <span data-ttu-id="fd997-121">値</span><span class="sxs-lookup"><span data-stu-id="fd997-121">Value</span></span> | <span data-ttu-id="fd997-122">説明</span><span class="sxs-lookup"><span data-stu-id="fd997-122">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="fd997-123">_if-match_</span><span class="sxs-lookup"><span data-stu-id="fd997-123">_if-match_</span></span> | <span data-ttu-id="fd997-124">etag</span><span class="sxs-lookup"><span data-stu-id="fd997-124">etag</span></span>  | <span data-ttu-id="fd997-125">この要求ヘッダーが含まれていて、指定された eTag がアイテムの現在の eTag に一致しない場合には、`412 Precondition Failed` 応答が返され、アイテムは更新されません。</span><span class="sxs-lookup"><span data-stu-id="fd997-125">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>

## <a name="request-body"></a><span data-ttu-id="fd997-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="fd997-126">Request body</span></span> 
<span data-ttu-id="fd997-127">要求本文に、更新するフィールドを指定する [fieldValueSet][] の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fd997-127">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="response"></a><span data-ttu-id="fd997-128">応答</span><span class="sxs-lookup"><span data-stu-id="fd997-128">Response</span></span> 

<span data-ttu-id="fd997-129">成功した場合、このメソッドは更新されたリスト アイテムの応答本文で`201 Created`応答コードと [fieldValueSet][] を返します。</span><span class="sxs-lookup"><span data-stu-id="fd997-129">If successful, this method returns a `201 Created` response code and a [fieldValueSet][] in the response body for the updated list item.</span></span>

## <a name="example"></a><span data-ttu-id="fd997-130">例</span><span class="sxs-lookup"><span data-stu-id="fd997-130">Example</span></span>

<span data-ttu-id="fd997-131">ここでは、リスト アイテムの **Color** フィールドと **Quantity** フィールドを新しい値で更新する例を示します。</span><span class="sxs-lookup"><span data-stu-id="fd997-131">The following example updates the **Color** and **Quantity** fields of the list item with new values.</span></span> <span data-ttu-id="fd997-132">\*\*listItem \*\*の他の値はすべてそのままです。</span><span class="sxs-lookup"><span data-stu-id="fd997-132">All other values on the **listItem** are left alone.</span></span> 

### <a name="request"></a><span data-ttu-id="fd997-133">要求</span><span class="sxs-lookup"><span data-stu-id="fd997-133">Request</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="fd997-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="fd997-134">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "update-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fd997-135">C#</span><span class="sxs-lookup"><span data-stu-id="fd997-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fd997-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="fd997-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fd997-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fd997-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fd997-138">Java</span><span class="sxs-lookup"><span data-stu-id="fd997-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fd997-139">応答</span><span class="sxs-lookup"><span data-stu-id="fd997-139">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.fieldValueSet", "truncated": true } -->

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update",
  "suppressions": [
  ]
} -->
