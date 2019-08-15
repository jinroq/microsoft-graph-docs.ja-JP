---
title: RangeBorder を作成する
description: この API を使用して、新しい RangeBorder を作成します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 9c6bf7dfeb59bba338ce0e5739cdd84a731b688c
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36411971"
---
# <a name="create-rangeborder"></a><span data-ttu-id="8f205-103">RangeBorder を作成する</span><span class="sxs-lookup"><span data-stu-id="8f205-103">Create RangeBorder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f205-104">この API を使用して、新しい RangeBorder を作成します。</span><span class="sxs-lookup"><span data-stu-id="8f205-104">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="8f205-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8f205-105">Permissions</span></span>
<span data-ttu-id="8f205-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8f205-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f205-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8f205-108">Permission type</span></span>      | <span data-ttu-id="8f205-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8f205-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f205-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8f205-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8f205-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f205-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8f205-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8f205-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f205-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f205-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8f205-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8f205-114">Application</span></span> | <span data-ttu-id="8f205-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8f205-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f205-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8f205-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/borders
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="8f205-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8f205-117">Request headers</span></span>
| <span data-ttu-id="8f205-118">名前</span><span class="sxs-lookup"><span data-stu-id="8f205-118">Name</span></span>       | <span data-ttu-id="8f205-119">説明</span><span class="sxs-lookup"><span data-stu-id="8f205-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8f205-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f205-120">Authorization</span></span>  | <span data-ttu-id="8f205-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8f205-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f205-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8f205-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8f205-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="8f205-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f205-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8f205-126">Request body</span></span>
<span data-ttu-id="8f205-127">要求本文で、 [workbookRangeBorder](../resources/workbookrangeborder.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8f205-127">In the request body, supply a JSON representation of [workbookRangeBorder](../resources/workbookrangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8f205-128">応答</span><span class="sxs-lookup"><span data-stu-id="8f205-128">Response</span></span>

<span data-ttu-id="8f205-129">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[workbookRangeBorder](../resources/workbookrangeborder.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8f205-129">If successful, this method returns `201 Created` response code and [workbookRangeBorder](../resources/workbookrangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f205-130">例</span><span class="sxs-lookup"><span data-stu-id="8f205-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8f205-131">要求</span><span class="sxs-lookup"><span data-stu-id="8f205-131">Request</span></span>
<span data-ttu-id="8f205-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8f205-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8f205-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8f205-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/borders
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8f205-134">C#</span><span class="sxs-lookup"><span data-stu-id="8f205-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-rangeborder-from-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f205-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f205-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-rangeborder-from-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8f205-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="8f205-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-rangeborder-from-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="8f205-137">要求本文で、 [workbookRangeBorder](../resources/workbookrangeborder.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8f205-137">In the request body, supply a JSON representation of [workbookRangeBorder](../resources/workbookrangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8f205-138">応答</span><span class="sxs-lookup"><span data-stu-id="8f205-138">Response</span></span>
<span data-ttu-id="8f205-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8f205-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
