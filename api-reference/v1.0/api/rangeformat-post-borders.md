---
title: RangeBorder を作成する
description: この API を使用して、新しい RangeBorder を作成します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 74ec5c2c9f620c6444ffd32508b719f7026f38a9
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263610"
---
# <a name="create-rangeborder"></a><span data-ttu-id="32f1c-103">RangeBorder を作成する</span><span class="sxs-lookup"><span data-stu-id="32f1c-103">Create RangeBorder</span></span>

<span data-ttu-id="32f1c-104">この API を使用して、新しい RangeBorder を作成します。</span><span class="sxs-lookup"><span data-stu-id="32f1c-104">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="32f1c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="32f1c-105">Permissions</span></span>
<span data-ttu-id="32f1c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="32f1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32f1c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="32f1c-108">Permission type</span></span>      | <span data-ttu-id="32f1c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="32f1c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32f1c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="32f1c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="32f1c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32f1c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="32f1c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="32f1c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32f1c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32f1c-113">Not supported.</span></span>    |
|<span data-ttu-id="32f1c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="32f1c-114">Application</span></span> | <span data-ttu-id="32f1c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32f1c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="32f1c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="32f1c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/borders
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="32f1c-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="32f1c-117">Request headers</span></span>
| <span data-ttu-id="32f1c-118">名前</span><span class="sxs-lookup"><span data-stu-id="32f1c-118">Name</span></span>       | <span data-ttu-id="32f1c-119">説明</span><span class="sxs-lookup"><span data-stu-id="32f1c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="32f1c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="32f1c-120">Authorization</span></span>  | <span data-ttu-id="32f1c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="32f1c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="32f1c-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="32f1c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="32f1c-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="32f1c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="32f1c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="32f1c-126">Request body</span></span>
<span data-ttu-id="32f1c-127">要求本文で、 [WorkbookRangeBorder](../resources/rangeborder.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="32f1c-127">In the request body, supply a JSON representation of [WorkbookRangeBorder](../resources/rangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="32f1c-128">応答</span><span class="sxs-lookup"><span data-stu-id="32f1c-128">Response</span></span>

<span data-ttu-id="32f1c-129">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[WorkbookRangeBorder](../resources/rangeborder.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="32f1c-129">If successful, this method returns `201 Created` response code and [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32f1c-130">例</span><span class="sxs-lookup"><span data-stu-id="32f1c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="32f1c-131">要求</span><span class="sxs-lookup"><span data-stu-id="32f1c-131">Request</span></span>
<span data-ttu-id="32f1c-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="32f1c-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders
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
<span data-ttu-id="32f1c-133">要求本文で、 [WorkbookRangeBorder](../resources/rangeborder.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="32f1c-133">In the request body, supply a JSON representation of [WorkbookRangeBorder](../resources/rangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="32f1c-134">応答</span><span class="sxs-lookup"><span data-stu-id="32f1c-134">Response</span></span>
<span data-ttu-id="32f1c-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="32f1c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="32f1c-138">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="32f1c-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="32f1c-139">C#</span><span class="sxs-lookup"><span data-stu-id="32f1c-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_rangeborder_from_rangeformat-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="32f1c-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="32f1c-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_rangeborder_from_rangeformat-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="32f1c-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="32f1c-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_rangeborder_from_rangeformat-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/rangeformat-post-borders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-post-borders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-post-borders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
