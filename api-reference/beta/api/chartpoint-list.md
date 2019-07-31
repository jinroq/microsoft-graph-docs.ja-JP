---
title: List ChartPointsCollection
description: chartpoint オブジェクトのリストを取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 171ffbe4fefebd1e7a465b1ebb83a9a03c1e4f0d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943779"
---
# <a name="list-chartpointscollection"></a><span data-ttu-id="a564e-103">List ChartPointsCollection</span><span class="sxs-lookup"><span data-stu-id="a564e-103">List ChartPointsCollection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a564e-104">chartpoint オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="a564e-104">Retrieve a list of chartpoint objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="a564e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a564e-105">Permissions</span></span>
<span data-ttu-id="a564e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a564e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a564e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a564e-108">Permission type</span></span>      | <span data-ttu-id="a564e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a564e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a564e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a564e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a564e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a564e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a564e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a564e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a564e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a564e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a564e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a564e-114">Application</span></span> | <span data-ttu-id="a564e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a564e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a564e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a564e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a564e-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a564e-117">Optional query parameters</span></span>
<span data-ttu-id="a564e-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a564e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a564e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a564e-119">Request headers</span></span>
| <span data-ttu-id="a564e-120">名前</span><span class="sxs-lookup"><span data-stu-id="a564e-120">Name</span></span>      |<span data-ttu-id="a564e-121">説明</span><span class="sxs-lookup"><span data-stu-id="a564e-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a564e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a564e-122">Authorization</span></span>  | <span data-ttu-id="a564e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a564e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a564e-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a564e-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="a564e-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="a564e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a564e-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="a564e-128">Request body</span></span>
<span data-ttu-id="a564e-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a564e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a564e-130">応答</span><span class="sxs-lookup"><span data-stu-id="a564e-130">Response</span></span>

<span data-ttu-id="a564e-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[workbookChartPoint](../resources/workbookchartpoint.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a564e-131">If successful, this method returns a `200 OK` response code and collection of [workbookChartPoint](../resources/workbookchartpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a564e-132">例</span><span class="sxs-lookup"><span data-stu-id="a564e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a564e-133">要求</span><span class="sxs-lookup"><span data-stu-id="a564e-133">Request</span></span>
<span data-ttu-id="a564e-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a564e-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a564e-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a564e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartpointscollection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a564e-136">C#</span><span class="sxs-lookup"><span data-stu-id="a564e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartpointscollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a564e-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="a564e-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartpointscollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a564e-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="a564e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartpointscollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a564e-139">Java</span><span class="sxs-lookup"><span data-stu-id="a564e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chartpointscollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a564e-140">応答</span><span class="sxs-lookup"><span data-stu-id="a564e-140">Response</span></span>
<span data-ttu-id="a564e-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a564e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartPoint",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 57

{
  "value": [
    {
      "value": {
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List ChartPointsCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
