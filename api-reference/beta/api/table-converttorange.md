---
title: 'Table: convertToRange'
description: テーブルを通常の範囲のセルに変換します。すべてのデータが保持されます。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: bb9b97e1a3e413369ed1fec77bc54cd589613de0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271177"
---
# <a name="table-converttorange"></a><span data-ttu-id="c7fc3-104">Table: convertToRange</span><span class="sxs-lookup"><span data-stu-id="c7fc3-104">Table: convertToRange</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7fc3-p102">テーブルを通常の範囲のセルに変換します。すべてのデータが保持されます。</span><span class="sxs-lookup"><span data-stu-id="c7fc3-p102">Converts the table into a normal range of cells. All data is preserved.</span></span>
## <a name="permissions"></a><span data-ttu-id="c7fc3-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c7fc3-107">Permissions</span></span>
<span data-ttu-id="c7fc3-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c7fc3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7fc3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c7fc3-110">Permission type</span></span>      | <span data-ttu-id="c7fc3-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c7fc3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7fc3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c7fc3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c7fc3-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7fc3-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c7fc3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c7fc3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7fc3-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7fc3-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c7fc3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c7fc3-116">Application</span></span> | <span data-ttu-id="c7fc3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7fc3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7fc3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c7fc3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/convertToRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/convertToRange

```
## <a name="request-headers"></a><span data-ttu-id="c7fc3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c7fc3-119">Request headers</span></span>
| <span data-ttu-id="c7fc3-120">名前</span><span class="sxs-lookup"><span data-stu-id="c7fc3-120">Name</span></span>       | <span data-ttu-id="c7fc3-121">説明</span><span class="sxs-lookup"><span data-stu-id="c7fc3-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c7fc3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7fc3-122">Authorization</span></span>  | <span data-ttu-id="c7fc3-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c7fc3-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c7fc3-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c7fc3-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="c7fc3-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="c7fc3-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7fc3-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="c7fc3-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c7fc3-129">応答</span><span class="sxs-lookup"><span data-stu-id="c7fc3-129">Response</span></span>

<span data-ttu-id="c7fc3-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/workbookrange.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c7fc3-130">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7fc3-131">例</span><span class="sxs-lookup"><span data-stu-id="c7fc3-131">Example</span></span>
<span data-ttu-id="c7fc3-132">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="c7fc3-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c7fc3-133">要求</span><span class="sxs-lookup"><span data-stu-id="c7fc3-133">Request</span></span>
<span data-ttu-id="c7fc3-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c7fc3-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_converttorange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/convertToRange
```

##### <a name="response"></a><span data-ttu-id="c7fc3-135">応答</span><span class="sxs-lookup"><span data-stu-id="c7fc3-135">Response</span></span>
<span data-ttu-id="c7fc3-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c7fc3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c7fc3-139">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="c7fc3-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c7fc3-140">C#</span><span class="sxs-lookup"><span data-stu-id="c7fc3-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/table_converttorange-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c7fc3-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="c7fc3-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/table_converttorange-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c7fc3-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="c7fc3-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/table_converttorange-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Table: convertToRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/table-converttorange.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/table-converttorange.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/table-converttorange.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
