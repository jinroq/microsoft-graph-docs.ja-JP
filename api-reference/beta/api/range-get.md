---
title: 範囲を取得する
description: 範囲オブジェクトのプロパティと関係を取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 177f95b5580002a7c8e8b2beae390decb17d507e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266774"
---
# <a name="get-range"></a><span data-ttu-id="8c59f-103">範囲を取得する</span><span class="sxs-lookup"><span data-stu-id="8c59f-103">Get Range</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c59f-104">範囲オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="8c59f-104">Retrieve the properties and relationships of range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8c59f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8c59f-105">Permissions</span></span>
<span data-ttu-id="8c59f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8c59f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c59f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8c59f-108">Permission type</span></span>      | <span data-ttu-id="8c59f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8c59f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c59f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8c59f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8c59f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c59f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8c59f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8c59f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c59f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c59f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8c59f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8c59f-114">Application</span></span> | <span data-ttu-id="8c59f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c59f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c59f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8c59f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/range(address='<address>')
GET /workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8c59f-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8c59f-117">Optional query parameters</span></span>
<span data-ttu-id="8c59f-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8c59f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c59f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8c59f-119">Request headers</span></span>
| <span data-ttu-id="8c59f-120">名前</span><span class="sxs-lookup"><span data-stu-id="8c59f-120">Name</span></span>      |<span data-ttu-id="8c59f-121">説明</span><span class="sxs-lookup"><span data-stu-id="8c59f-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8c59f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c59f-122">Authorization</span></span>  | <span data-ttu-id="8c59f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8c59f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8c59f-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8c59f-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="8c59f-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="8c59f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c59f-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="8c59f-128">Request body</span></span>
<span data-ttu-id="8c59f-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8c59f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c59f-130">応答</span><span class="sxs-lookup"><span data-stu-id="8c59f-130">Response</span></span>

<span data-ttu-id="8c59f-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[workbookRange](../resources/workbookrange.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8c59f-131">If successful, this method returns a `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8c59f-132">例</span><span class="sxs-lookup"><span data-stu-id="8c59f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8c59f-133">要求</span><span class="sxs-lookup"><span data-stu-id="8c59f-133">Request</span></span>
<span data-ttu-id="8c59f-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8c59f-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_range"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range
```
##### <a name="response"></a><span data-ttu-id="8c59f-135">応答</span><span class="sxs-lookup"><span data-stu-id="8c59f-135">Response</span></span>
<span data-ttu-id="8c59f-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8c59f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8c59f-139">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="8c59f-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8c59f-140">C#</span><span class="sxs-lookup"><span data-stu-id="8c59f-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_range-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8c59f-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="8c59f-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_range-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8c59f-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="8c59f-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_range-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/range-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/range-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
