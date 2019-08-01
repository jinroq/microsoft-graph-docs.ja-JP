---
title: 'Table: clearFilters'
description: 現在テーブルに適用されているすべてのフィルターをクリアします。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c79466877a32fb4fe37e005ea29c311734be8147
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36024579"
---
# <a name="table-clearfilters"></a><span data-ttu-id="b0bed-103">Table: clearFilters</span><span class="sxs-lookup"><span data-stu-id="b0bed-103">Table: clearFilters</span></span>

<span data-ttu-id="b0bed-104">現在テーブルに適用されているすべてのフィルターをクリアします。</span><span class="sxs-lookup"><span data-stu-id="b0bed-104">Clears all the filters currently applied on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="b0bed-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b0bed-105">Permissions</span></span>
<span data-ttu-id="b0bed-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0bed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0bed-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b0bed-108">Permission type</span></span>      | <span data-ttu-id="b0bed-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b0bed-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0bed-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b0bed-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b0bed-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0bed-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b0bed-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b0bed-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0bed-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0bed-113">Not supported.</span></span>    |
|<span data-ttu-id="b0bed-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b0bed-114">Application</span></span> | <span data-ttu-id="b0bed-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0bed-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0bed-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b0bed-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/clearFilters
POST /workbook/worksheets/{id|name}/tables/{id|name}/clearFilters

```
## <a name="request-headers"></a><span data-ttu-id="b0bed-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b0bed-117">Request headers</span></span>
| <span data-ttu-id="b0bed-118">名前</span><span class="sxs-lookup"><span data-stu-id="b0bed-118">Name</span></span>       | <span data-ttu-id="b0bed-119">説明</span><span class="sxs-lookup"><span data-stu-id="b0bed-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b0bed-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0bed-120">Authorization</span></span>  | <span data-ttu-id="b0bed-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b0bed-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b0bed-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b0bed-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="b0bed-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="b0bed-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0bed-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b0bed-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="b0bed-127">応答</span><span class="sxs-lookup"><span data-stu-id="b0bed-127">Response</span></span>

<span data-ttu-id="b0bed-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b0bed-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0bed-130">例</span><span class="sxs-lookup"><span data-stu-id="b0bed-130">Example</span></span>
<span data-ttu-id="b0bed-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="b0bed-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b0bed-132">要求</span><span class="sxs-lookup"><span data-stu-id="b0bed-132">Request</span></span>
<span data-ttu-id="b0bed-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b0bed-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b0bed-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b0bed-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_clearfilters"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/clearFilters
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b0bed-135">C#</span><span class="sxs-lookup"><span data-stu-id="b0bed-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-clearfilters-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b0bed-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="b0bed-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-clearfilters-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b0bed-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="b0bed-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-clearfilters-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b0bed-138">Java</span><span class="sxs-lookup"><span data-stu-id="b0bed-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-clearfilters-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b0bed-139">応答</span><span class="sxs-lookup"><span data-stu-id="b0bed-139">Response</span></span>
<span data-ttu-id="b0bed-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b0bed-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Table: clearFilters",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
