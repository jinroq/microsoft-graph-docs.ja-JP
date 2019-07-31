---
title: Get ChartSeries
description: chartseries オブジェクトのプロパティと関係を取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: daf01e855b1a652f033a99f057066da2063c3f86
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943754"
---
# <a name="get-chartseries"></a><span data-ttu-id="ea4c6-103">Get ChartSeries</span><span class="sxs-lookup"><span data-stu-id="ea4c6-103">Get ChartSeries</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea4c6-104">chartseries オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="ea4c6-104">Retrieve the properties and relationships of chartseries object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ea4c6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ea4c6-105">Permissions</span></span>
<span data-ttu-id="ea4c6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ea4c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea4c6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ea4c6-108">Permission type</span></span>      | <span data-ttu-id="ea4c6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ea4c6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea4c6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ea4c6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ea4c6-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea4c6-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ea4c6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ea4c6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea4c6-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea4c6-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ea4c6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ea4c6-114">Application</span></span> | <span data-ttu-id="ea4c6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ea4c6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea4c6-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ea4c6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/series/{undefined}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ea4c6-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ea4c6-117">Optional query parameters</span></span>
<span data-ttu-id="ea4c6-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ea4c6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ea4c6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ea4c6-119">Request headers</span></span>
| <span data-ttu-id="ea4c6-120">名前</span><span class="sxs-lookup"><span data-stu-id="ea4c6-120">Name</span></span>      |<span data-ttu-id="ea4c6-121">説明</span><span class="sxs-lookup"><span data-stu-id="ea4c6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ea4c6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea4c6-122">Authorization</span></span>  | <span data-ttu-id="ea4c6-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ea4c6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ea4c6-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ea4c6-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ea4c6-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="ea4c6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea4c6-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="ea4c6-128">Request body</span></span>
<span data-ttu-id="ea4c6-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ea4c6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea4c6-130">応答</span><span class="sxs-lookup"><span data-stu-id="ea4c6-130">Response</span></span>

<span data-ttu-id="ea4c6-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[workbookChartSeries](../resources/workbookchartseries.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ea4c6-131">If successful, this method returns a `200 OK` response code and [workbookChartSeries](../resources/workbookchartseries.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ea4c6-132">例</span><span class="sxs-lookup"><span data-stu-id="ea4c6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea4c6-133">要求</span><span class="sxs-lookup"><span data-stu-id="ea4c6-133">Request</span></span>
<span data-ttu-id="ea4c6-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ea4c6-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ea4c6-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ea4c6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartseries"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ea4c6-136">C#</span><span class="sxs-lookup"><span data-stu-id="ea4c6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartseries-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ea4c6-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="ea4c6-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartseries-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ea4c6-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="ea4c6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartseries-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ea4c6-139">Java</span><span class="sxs-lookup"><span data-stu-id="ea4c6-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chartseries-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ea4c6-140">応答</span><span class="sxs-lookup"><span data-stu-id="ea4c6-140">Response</span></span>
<span data-ttu-id="ea4c6-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ea4c6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get ChartSeries",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
