---
title: 範囲:EntireColumn
description: 範囲に含まれるすべての列を表すオブジェクトを取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2c79cb546aa959c9bbea99b684cee7d52e20c27f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412286"
---
# <a name="range-entirecolumn"></a><span data-ttu-id="0aaa8-103">範囲:EntireColumn</span><span class="sxs-lookup"><span data-stu-id="0aaa8-103">Range: EntireColumn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0aaa8-104">範囲に含まれるすべての列を表すオブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="0aaa8-104">Gets an object that represents the entire column of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="0aaa8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0aaa8-105">Permissions</span></span>
<span data-ttu-id="0aaa8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0aaa8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0aaa8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0aaa8-108">Permission type</span></span>      | <span data-ttu-id="0aaa8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0aaa8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0aaa8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0aaa8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0aaa8-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0aaa8-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0aaa8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0aaa8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0aaa8-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0aaa8-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0aaa8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0aaa8-114">Application</span></span> | <span data-ttu-id="0aaa8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0aaa8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0aaa8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0aaa8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/EntireColumn
GET /workbook/worksheets/{id|name}/range(address='<address>')/EntireColumn
GET /workbook/tables/{id|name}/columns/{id|name}/range/EntireColumn

```
## <a name="request-headers"></a><span data-ttu-id="0aaa8-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0aaa8-117">Request headers</span></span>
| <span data-ttu-id="0aaa8-118">名前</span><span class="sxs-lookup"><span data-stu-id="0aaa8-118">Name</span></span>       | <span data-ttu-id="0aaa8-119">説明</span><span class="sxs-lookup"><span data-stu-id="0aaa8-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0aaa8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0aaa8-120">Authorization</span></span>  | <span data-ttu-id="0aaa8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0aaa8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0aaa8-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0aaa8-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="0aaa8-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="0aaa8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0aaa8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0aaa8-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="0aaa8-127">応答</span><span class="sxs-lookup"><span data-stu-id="0aaa8-127">Response</span></span>

<span data-ttu-id="0aaa8-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/workbookrange.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0aaa8-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0aaa8-129">例</span><span class="sxs-lookup"><span data-stu-id="0aaa8-129">Example</span></span>
<span data-ttu-id="0aaa8-130">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="0aaa8-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0aaa8-131">要求</span><span class="sxs-lookup"><span data-stu-id="0aaa8-131">Request</span></span>
<span data-ttu-id="0aaa8-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0aaa8-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0aaa8-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0aaa8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_entirecolumn"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/EntireColumn
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0aaa8-134">C#</span><span class="sxs-lookup"><span data-stu-id="0aaa8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-entirecolumn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0aaa8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0aaa8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-entirecolumn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0aaa8-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="0aaa8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-entirecolumn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0aaa8-137">応答</span><span class="sxs-lookup"><span data-stu-id="0aaa8-137">Response</span></span>
<span data-ttu-id="0aaa8-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0aaa8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Range: EntireColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
