---
title: 範囲:LastColumn
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: fa596da82167db358a0e13d9c927d77ff671827b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36022227"
---
# <a name="range-lastcolumn"></a><span data-ttu-id="94dae-103">範囲:LastColumn</span><span class="sxs-lookup"><span data-stu-id="94dae-103">Range: LastColumn</span></span>

<span data-ttu-id="94dae-p101">範囲内の最後の列を取得します。たとえば、"B2:D5" の最後の列は "D2:D5" になります。</span><span class="sxs-lookup"><span data-stu-id="94dae-p101">Gets the last column within the range. For example, the last column of "B2:D5" is "D2:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="94dae-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="94dae-106">Permissions</span></span>
<span data-ttu-id="94dae-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="94dae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94dae-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="94dae-109">Permission type</span></span>      | <span data-ttu-id="94dae-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="94dae-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94dae-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="94dae-111">Delegated (work or school account)</span></span> | <span data-ttu-id="94dae-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94dae-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="94dae-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="94dae-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94dae-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94dae-114">Not supported.</span></span>    |
|<span data-ttu-id="94dae-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="94dae-115">Application</span></span> | <span data-ttu-id="94dae-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94dae-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="94dae-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="94dae-117">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="94dae-118">プロトコル</span><span class="sxs-lookup"><span data-stu-id="94dae-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/lastColumn
GET /workbook/worksheets/{id|name}/range(address='<address>')/lastColumn
GET /workbook/tables/{id|name}/columns/{id|name}/range/lastColumn

```
## <a name="request-headers"></a><span data-ttu-id="94dae-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="94dae-119">Request headers</span></span>
| <span data-ttu-id="94dae-120">名前</span><span class="sxs-lookup"><span data-stu-id="94dae-120">Name</span></span>       | <span data-ttu-id="94dae-121">説明</span><span class="sxs-lookup"><span data-stu-id="94dae-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="94dae-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="94dae-122">Authorization</span></span>  | <span data-ttu-id="94dae-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="94dae-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="94dae-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="94dae-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="94dae-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="94dae-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="94dae-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="94dae-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="94dae-129">応答</span><span class="sxs-lookup"><span data-stu-id="94dae-129">Response</span></span>

<span data-ttu-id="94dae-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="94dae-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94dae-131">例</span><span class="sxs-lookup"><span data-stu-id="94dae-131">Example</span></span>
<span data-ttu-id="94dae-132">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="94dae-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="94dae-133">要求</span><span class="sxs-lookup"><span data-stu-id="94dae-133">Request</span></span>
<span data-ttu-id="94dae-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="94dae-134">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_lastcolumn"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/lastColumn
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="94dae-135">C#</span><span class="sxs-lookup"><span data-stu-id="94dae-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-lastcolumn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="94dae-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="94dae-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-lastcolumn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="94dae-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="94dae-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-lastcolumn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="94dae-138">Java</span><span class="sxs-lookup"><span data-stu-id="94dae-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-lastcolumn-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="94dae-139">応答</span><span class="sxs-lookup"><span data-stu-id="94dae-139">Response</span></span>
<span data-ttu-id="94dae-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="94dae-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: LastColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
