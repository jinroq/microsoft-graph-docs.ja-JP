---
title: 'Table: convertToRange'
description: テーブルを通常の範囲のセルに変換します。すべてのデータが保持されます。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 19d9f7e84d18886826455ba961e86ab93b4af1dc
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33603111"
---
# <a name="table-converttorange"></a><span data-ttu-id="af8a3-104">Table: convertToRange</span><span class="sxs-lookup"><span data-stu-id="af8a3-104">Table: convertToRange</span></span>

<span data-ttu-id="af8a3-p102">テーブルを通常の範囲のセルに変換します。すべてのデータが保持されます。</span><span class="sxs-lookup"><span data-stu-id="af8a3-p102">Converts the table into a normal range of cells. All data is preserved.</span></span>
## <a name="permissions"></a><span data-ttu-id="af8a3-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="af8a3-107">Permissions</span></span>
<span data-ttu-id="af8a3-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="af8a3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af8a3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="af8a3-110">Permission type</span></span>      | <span data-ttu-id="af8a3-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="af8a3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af8a3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="af8a3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="af8a3-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="af8a3-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="af8a3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="af8a3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af8a3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af8a3-115">Not supported.</span></span>    |
|<span data-ttu-id="af8a3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="af8a3-116">Application</span></span> | <span data-ttu-id="af8a3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af8a3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="af8a3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="af8a3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/convertToRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/convertToRange

```
## <a name="request-headers"></a><span data-ttu-id="af8a3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="af8a3-119">Request headers</span></span>
| <span data-ttu-id="af8a3-120">名前</span><span class="sxs-lookup"><span data-stu-id="af8a3-120">Name</span></span>       | <span data-ttu-id="af8a3-121">説明</span><span class="sxs-lookup"><span data-stu-id="af8a3-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="af8a3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="af8a3-122">Authorization</span></span>  | <span data-ttu-id="af8a3-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="af8a3-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="af8a3-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="af8a3-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="af8a3-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="af8a3-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="af8a3-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="af8a3-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="af8a3-129">応答</span><span class="sxs-lookup"><span data-stu-id="af8a3-129">Response</span></span>

<span data-ttu-id="af8a3-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="af8a3-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af8a3-131">例</span><span class="sxs-lookup"><span data-stu-id="af8a3-131">Example</span></span>
<span data-ttu-id="af8a3-132">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="af8a3-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="af8a3-133">要求</span><span class="sxs-lookup"><span data-stu-id="af8a3-133">Request</span></span>
<span data-ttu-id="af8a3-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="af8a3-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_converttorange"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/convertToRange
```

##### <a name="response"></a><span data-ttu-id="af8a3-135">応答</span><span class="sxs-lookup"><span data-stu-id="af8a3-135">Response</span></span>
<span data-ttu-id="af8a3-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="af8a3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="af8a3-139">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="af8a3-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="af8a3-140">Visual</span><span class="sxs-lookup"><span data-stu-id="af8a3-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/table_converttorange-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="af8a3-141">Java</span><span class="sxs-lookup"><span data-stu-id="af8a3-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/table_converttorange-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Table: convertToRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/table-converttorange.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/table-converttorange.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
