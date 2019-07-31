---
title: 'フィルター: クリア'
description: 指定した列のフィルターをクリアします。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 266664d3ec58368361febff5714d367555744745
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954387"
---
# <a name="filter-clear"></a><span data-ttu-id="95fcc-103">フィルター: クリア</span><span class="sxs-lookup"><span data-stu-id="95fcc-103">Filter: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95fcc-104">指定した列のフィルターをクリアします。</span><span class="sxs-lookup"><span data-stu-id="95fcc-104">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="95fcc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="95fcc-105">Permissions</span></span>
<span data-ttu-id="95fcc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="95fcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95fcc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="95fcc-108">Permission type</span></span>      | <span data-ttu-id="95fcc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="95fcc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95fcc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="95fcc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="95fcc-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="95fcc-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="95fcc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="95fcc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95fcc-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="95fcc-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="95fcc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="95fcc-114">Application</span></span> | <span data-ttu-id="95fcc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95fcc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="95fcc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="95fcc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="95fcc-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95fcc-117">Request headers</span></span>
| <span data-ttu-id="95fcc-118">名前</span><span class="sxs-lookup"><span data-stu-id="95fcc-118">Name</span></span>       | <span data-ttu-id="95fcc-119">説明</span><span class="sxs-lookup"><span data-stu-id="95fcc-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="95fcc-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="95fcc-120">Authorization</span></span>  | <span data-ttu-id="95fcc-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="95fcc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95fcc-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="95fcc-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="95fcc-124">応答</span><span class="sxs-lookup"><span data-stu-id="95fcc-124">Response</span></span>

<span data-ttu-id="95fcc-p103">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="95fcc-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95fcc-127">例</span><span class="sxs-lookup"><span data-stu-id="95fcc-127">Example</span></span>
<span data-ttu-id="95fcc-128">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="95fcc-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="95fcc-129">要求</span><span class="sxs-lookup"><span data-stu-id="95fcc-129">Request</span></span>
<span data-ttu-id="95fcc-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="95fcc-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="95fcc-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="95fcc-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="95fcc-132">C#</span><span class="sxs-lookup"><span data-stu-id="95fcc-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/filter-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="95fcc-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="95fcc-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/filter-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="95fcc-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="95fcc-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/filter-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="95fcc-135">Java</span><span class="sxs-lookup"><span data-stu-id="95fcc-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/filter-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="95fcc-136">応答</span><span class="sxs-lookup"><span data-stu-id="95fcc-136">Response</span></span>
<span data-ttu-id="95fcc-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="95fcc-137">Here is an example of the response.</span></span> 
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
  "description": "Filter: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
