---
title: 'フィルター: 適用'
description: 指定した列に指定されたフィルター条件を適用します。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 7ed815297c4bc0e9512208ca3cc257bba3148b05
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954374"
---
# <a name="filter-apply"></a><span data-ttu-id="631b7-103">フィルター: 適用</span><span class="sxs-lookup"><span data-stu-id="631b7-103">Filter: apply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="631b7-104">指定した列に指定されたフィルター条件を適用します。</span><span class="sxs-lookup"><span data-stu-id="631b7-104">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="631b7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="631b7-105">Permissions</span></span>
<span data-ttu-id="631b7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="631b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="631b7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="631b7-108">Permission type</span></span>      | <span data-ttu-id="631b7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="631b7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="631b7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="631b7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="631b7-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="631b7-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="631b7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="631b7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="631b7-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="631b7-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="631b7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="631b7-114">Application</span></span> | <span data-ttu-id="631b7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="631b7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="631b7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="631b7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="631b7-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="631b7-117">Request headers</span></span>
| <span data-ttu-id="631b7-118">名前</span><span class="sxs-lookup"><span data-stu-id="631b7-118">Name</span></span>       | <span data-ttu-id="631b7-119">説明</span><span class="sxs-lookup"><span data-stu-id="631b7-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="631b7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="631b7-120">Authorization</span></span>  | <span data-ttu-id="631b7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="631b7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="631b7-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="631b7-123">Request body</span></span>
<span data-ttu-id="631b7-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="631b7-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="631b7-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="631b7-125">Parameter</span></span>    | <span data-ttu-id="631b7-126">型</span><span class="sxs-lookup"><span data-stu-id="631b7-126">Type</span></span>   |<span data-ttu-id="631b7-127">説明</span><span class="sxs-lookup"><span data-stu-id="631b7-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="631b7-128">criteria</span><span class="sxs-lookup"><span data-stu-id="631b7-128">criteria</span></span>|<span data-ttu-id="631b7-129">workbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="631b7-129">workbookFilterCriteria</span></span>|<span data-ttu-id="631b7-130">適用する基準。</span><span class="sxs-lookup"><span data-stu-id="631b7-130">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="631b7-131">応答</span><span class="sxs-lookup"><span data-stu-id="631b7-131">Response</span></span>

<span data-ttu-id="631b7-p103">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="631b7-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="631b7-134">例</span><span class="sxs-lookup"><span data-stu-id="631b7-134">Example</span></span>
<span data-ttu-id="631b7-135">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="631b7-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="631b7-136">要求</span><span class="sxs-lookup"><span data-stu-id="631b7-136">Request</span></span>
<span data-ttu-id="631b7-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="631b7-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="631b7-138">プロトコル</span><span class="sxs-lookup"><span data-stu-id="631b7-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "filter_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
Content-type: application/json
Content-length: 321

{
  "criteria": {
    "criterion1": "criterion1-value",
    "criterion2": "criterion2-value",
    "color": "color-value",
    "operator": {
    },
    "icon": {
      "set": "set-value",
      "index": 99
    },
    "dynamicCriteria": "dynamicCriteria-value",
    "values": {
    },
    "filterOn": "filterOn-value"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="631b7-139">C#</span><span class="sxs-lookup"><span data-stu-id="631b7-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/filter-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="631b7-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="631b7-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/filter-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="631b7-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="631b7-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/filter-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="631b7-142">Java</span><span class="sxs-lookup"><span data-stu-id="631b7-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/filter-apply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="631b7-143">応答</span><span class="sxs-lookup"><span data-stu-id="631b7-143">Response</span></span>
<span data-ttu-id="631b7-144">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="631b7-144">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Filter: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
