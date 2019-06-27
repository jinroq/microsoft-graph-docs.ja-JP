---
title: 'Table: clearFilters'
description: 現在テーブルに適用されているすべてのフィルターをクリアします。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 94b0d2a144e226993a20cb5e89882219f0adebe4
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271184"
---
# <a name="table-clearfilters"></a><span data-ttu-id="7e226-103">Table: clearFilters</span><span class="sxs-lookup"><span data-stu-id="7e226-103">Table: clearFilters</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e226-104">現在テーブルに適用されているすべてのフィルターをクリアします。</span><span class="sxs-lookup"><span data-stu-id="7e226-104">Clears all the filters currently applied on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="7e226-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7e226-105">Permissions</span></span>
<span data-ttu-id="7e226-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7e226-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e226-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7e226-108">Permission type</span></span>      | <span data-ttu-id="7e226-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7e226-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e226-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7e226-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7e226-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7e226-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7e226-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7e226-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e226-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7e226-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7e226-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7e226-114">Application</span></span> | <span data-ttu-id="7e226-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e226-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e226-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7e226-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/clearFilters
POST /workbook/worksheets/{id|name}/tables/{id|name}/clearFilters

```
## <a name="request-headers"></a><span data-ttu-id="7e226-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7e226-117">Request headers</span></span>
| <span data-ttu-id="7e226-118">名前</span><span class="sxs-lookup"><span data-stu-id="7e226-118">Name</span></span>       | <span data-ttu-id="7e226-119">説明</span><span class="sxs-lookup"><span data-stu-id="7e226-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7e226-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e226-120">Authorization</span></span>  | <span data-ttu-id="7e226-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7e226-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7e226-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7e226-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="7e226-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="7e226-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e226-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7e226-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7e226-127">応答</span><span class="sxs-lookup"><span data-stu-id="7e226-127">Response</span></span>

<span data-ttu-id="7e226-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="7e226-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e226-130">例</span><span class="sxs-lookup"><span data-stu-id="7e226-130">Example</span></span>
<span data-ttu-id="7e226-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="7e226-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7e226-132">要求</span><span class="sxs-lookup"><span data-stu-id="7e226-132">Request</span></span>
<span data-ttu-id="7e226-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7e226-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_clearfilters"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/clearFilters
```

##### <a name="response"></a><span data-ttu-id="7e226-134">応答</span><span class="sxs-lookup"><span data-stu-id="7e226-134">Response</span></span>
<span data-ttu-id="7e226-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="7e226-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7e226-136">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="7e226-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7e226-137">C#</span><span class="sxs-lookup"><span data-stu-id="7e226-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/table_clearfilters-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7e226-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="7e226-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/table_clearfilters-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7e226-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="7e226-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/table_clearfilters-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Table: clearFilters",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/table-clearfilters.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/table-clearfilters.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/table-clearfilters.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
