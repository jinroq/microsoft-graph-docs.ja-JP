---
title: 'workbookChartCollection: ItemAt'
description: コレクション内の位置に基づいて workbookchart を取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 005a0462cb9d8ba0957f398fce10f53684b26a4a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261860"
---
# <a name="chartcollection-itemat"></a><span data-ttu-id="5c81a-103">ChartCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="5c81a-103">ChartCollection: ItemAt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c81a-104">コレクション内での位置を基にグラフを取得します。</span><span class="sxs-lookup"><span data-stu-id="5c81a-104">Gets a chart based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="5c81a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5c81a-105">Permissions</span></span>
<span data-ttu-id="5c81a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5c81a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c81a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5c81a-108">Permission type</span></span>      | <span data-ttu-id="5c81a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5c81a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c81a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5c81a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5c81a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c81a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5c81a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5c81a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c81a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c81a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5c81a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5c81a-114">Application</span></span> | <span data-ttu-id="5c81a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c81a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c81a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5c81a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="5c81a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5c81a-117">Request headers</span></span>
| <span data-ttu-id="5c81a-118">名前</span><span class="sxs-lookup"><span data-stu-id="5c81a-118">Name</span></span>       | <span data-ttu-id="5c81a-119">説明</span><span class="sxs-lookup"><span data-stu-id="5c81a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5c81a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c81a-120">Authorization</span></span>  | <span data-ttu-id="5c81a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5c81a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5c81a-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5c81a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="5c81a-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="5c81a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c81a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="5c81a-126">Request body</span></span>
<span data-ttu-id="5c81a-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="5c81a-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5c81a-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5c81a-128">Parameter</span></span>    | <span data-ttu-id="5c81a-129">型</span><span class="sxs-lookup"><span data-stu-id="5c81a-129">Type</span></span>   |<span data-ttu-id="5c81a-130">説明</span><span class="sxs-lookup"><span data-stu-id="5c81a-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c81a-131">index</span><span class="sxs-lookup"><span data-stu-id="5c81a-131">index</span></span>|<span data-ttu-id="5c81a-132">number</span><span class="sxs-lookup"><span data-stu-id="5c81a-132">number</span></span>|<span data-ttu-id="5c81a-p104">取得するオブジェクトのインデックス値。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="5c81a-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="5c81a-135">応答</span><span class="sxs-lookup"><span data-stu-id="5c81a-135">Response</span></span>

<span data-ttu-id="5c81a-136">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[workbookChart](../resources/workbookchart.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5c81a-136">If successful, this method returns `200 OK` response code and [workbookChart](../resources/workbookchart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c81a-137">例</span><span class="sxs-lookup"><span data-stu-id="5c81a-137">Example</span></span>
<span data-ttu-id="5c81a-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="5c81a-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5c81a-139">要求</span><span class="sxs-lookup"><span data-stu-id="5c81a-139">Request</span></span>
<span data-ttu-id="5c81a-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5c81a-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartcollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": 8
}
```

##### <a name="response"></a><span data-ttu-id="5c81a-141">応答</span><span class="sxs-lookup"><span data-stu-id="5c81a-141">Response</span></span>
<span data-ttu-id="5c81a-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5c81a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5c81a-145">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="5c81a-145">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5c81a-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="5c81a-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/chartcollection_itemat-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5c81a-147">目的-C</span><span class="sxs-lookup"><span data-stu-id="5c81a-147">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/chartcollection_itemat-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartcollection-itemat.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/chartcollection-itemat.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
