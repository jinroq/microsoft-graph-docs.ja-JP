---
title: List ChartPointsCollection
description: chartpoint オブジェクトのリストを取得します。
ms.openlocfilehash: 3d44c7fa816b1c1e9789f19e62ff1df6ada37158
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023344"
---
# <a name="list-chartpointscollection"></a><span data-ttu-id="6724c-103">List ChartPointsCollection</span><span class="sxs-lookup"><span data-stu-id="6724c-103">List ChartPointsCollection</span></span>

<span data-ttu-id="6724c-104">chartpoint オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="6724c-104">Retrieve a list of chartpoint objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="6724c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6724c-105">Permissions</span></span>
<span data-ttu-id="6724c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6724c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6724c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6724c-108">Permission type</span></span>      | <span data-ttu-id="6724c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6724c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6724c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6724c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6724c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6724c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6724c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6724c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6724c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6724c-113">Not supported.</span></span>    |
|<span data-ttu-id="6724c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6724c-114">Application</span></span> | <span data-ttu-id="6724c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6724c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6724c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6724c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6724c-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6724c-117">Optional query parameters</span></span>
<span data-ttu-id="6724c-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6724c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6724c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6724c-119">Request headers</span></span>
| <span data-ttu-id="6724c-120">名前</span><span class="sxs-lookup"><span data-stu-id="6724c-120">Name</span></span>      |<span data-ttu-id="6724c-121">説明</span><span class="sxs-lookup"><span data-stu-id="6724c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6724c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6724c-122">Authorization</span></span>  | <span data-ttu-id="6724c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6724c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6724c-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6724c-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="6724c-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="6724c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6724c-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="6724c-128">Request body</span></span>
<span data-ttu-id="6724c-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6724c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6724c-130">応答</span><span class="sxs-lookup"><span data-stu-id="6724c-130">Response</span></span>

<span data-ttu-id="6724c-131">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[WorkbookChartPoint](../resources/chartpoint.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="6724c-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookChartPoint](../resources/chartpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6724c-132">例</span><span class="sxs-lookup"><span data-stu-id="6724c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6724c-133">要求</span><span class="sxs-lookup"><span data-stu-id="6724c-133">Request</span></span>
<span data-ttu-id="6724c-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6724c-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartpointscollection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points
```
##### <a name="response"></a><span data-ttu-id="6724c-135">応答</span><span class="sxs-lookup"><span data-stu-id="6724c-135">Response</span></span>
<span data-ttu-id="6724c-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6724c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List ChartPointsCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->