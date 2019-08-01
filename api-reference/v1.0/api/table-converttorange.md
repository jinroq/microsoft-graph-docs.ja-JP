---
title: 'Table: convertToRange'
description: テーブルを通常の範囲のセルに変換します。すべてのデータが保持されます。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 29666544e46e9879313fa0593b15ef83f1fb7f25
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36024580"
---
# <a name="table-converttorange"></a><span data-ttu-id="7dcda-104">Table: convertToRange</span><span class="sxs-lookup"><span data-stu-id="7dcda-104">Table: convertToRange</span></span>

<span data-ttu-id="7dcda-p102">テーブルを通常の範囲のセルに変換します。すべてのデータが保持されます。</span><span class="sxs-lookup"><span data-stu-id="7dcda-p102">Converts the table into a normal range of cells. All data is preserved.</span></span>
## <a name="permissions"></a><span data-ttu-id="7dcda-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7dcda-107">Permissions</span></span>
<span data-ttu-id="7dcda-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7dcda-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dcda-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7dcda-110">Permission type</span></span>      | <span data-ttu-id="7dcda-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7dcda-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7dcda-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7dcda-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7dcda-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7dcda-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7dcda-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7dcda-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7dcda-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7dcda-115">Not supported.</span></span>    |
|<span data-ttu-id="7dcda-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7dcda-116">Application</span></span> | <span data-ttu-id="7dcda-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7dcda-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7dcda-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7dcda-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/convertToRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/convertToRange

```
## <a name="request-headers"></a><span data-ttu-id="7dcda-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7dcda-119">Request headers</span></span>
| <span data-ttu-id="7dcda-120">名前</span><span class="sxs-lookup"><span data-stu-id="7dcda-120">Name</span></span>       | <span data-ttu-id="7dcda-121">説明</span><span class="sxs-lookup"><span data-stu-id="7dcda-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7dcda-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7dcda-122">Authorization</span></span>  | <span data-ttu-id="7dcda-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7dcda-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7dcda-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7dcda-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="7dcda-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="7dcda-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7dcda-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="7dcda-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7dcda-129">応答</span><span class="sxs-lookup"><span data-stu-id="7dcda-129">Response</span></span>

<span data-ttu-id="7dcda-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7dcda-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7dcda-131">例</span><span class="sxs-lookup"><span data-stu-id="7dcda-131">Example</span></span>
<span data-ttu-id="7dcda-132">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="7dcda-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7dcda-133">要求</span><span class="sxs-lookup"><span data-stu-id="7dcda-133">Request</span></span>
<span data-ttu-id="7dcda-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7dcda-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7dcda-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7dcda-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_converttorange"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/convertToRange
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7dcda-136">C#</span><span class="sxs-lookup"><span data-stu-id="7dcda-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-converttorange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7dcda-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="7dcda-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-converttorange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7dcda-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="7dcda-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-converttorange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7dcda-139">Java</span><span class="sxs-lookup"><span data-stu-id="7dcda-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-converttorange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7dcda-140">応答</span><span class="sxs-lookup"><span data-stu-id="7dcda-140">Response</span></span>
<span data-ttu-id="7dcda-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7dcda-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Table: convertToRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
