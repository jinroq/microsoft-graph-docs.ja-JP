---
title: RangeBorder を取得する
description: rangeborder オブジェクトのプロパティと関係を取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: edbe018188f04c107cfccd86705eb260a89d70e0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455575"
---
# <a name="get-rangeborder"></a><span data-ttu-id="f0cfd-103">RangeBorder を取得する</span><span class="sxs-lookup"><span data-stu-id="f0cfd-103">Get RangeBorder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0cfd-104">rangeborder オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="f0cfd-104">Retrieve the properties and relationships of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f0cfd-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f0cfd-105">Permissions</span></span>
<span data-ttu-id="f0cfd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f0cfd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0cfd-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f0cfd-108">Permission type</span></span>      | <span data-ttu-id="f0cfd-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f0cfd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0cfd-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f0cfd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f0cfd-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0cfd-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f0cfd-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f0cfd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0cfd-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0cfd-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f0cfd-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f0cfd-114">Application</span></span> | <span data-ttu-id="f0cfd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0cfd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0cfd-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f0cfd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format/borders(<sideIndex>)
GET /workbook/worksheets/{id|name}/range(address='<address>')/format/borders(<sideIndex>)
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/borders(<sideIndex>)
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f0cfd-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f0cfd-117">Optional query parameters</span></span>
<span data-ttu-id="f0cfd-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f0cfd-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f0cfd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f0cfd-119">Request headers</span></span>
| <span data-ttu-id="f0cfd-120">名前</span><span class="sxs-lookup"><span data-stu-id="f0cfd-120">Name</span></span>      |<span data-ttu-id="f0cfd-121">説明</span><span class="sxs-lookup"><span data-stu-id="f0cfd-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f0cfd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0cfd-122">Authorization</span></span>  | <span data-ttu-id="f0cfd-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f0cfd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f0cfd-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f0cfd-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f0cfd-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="f0cfd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0cfd-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="f0cfd-128">Request body</span></span>
<span data-ttu-id="f0cfd-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f0cfd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0cfd-130">応答</span><span class="sxs-lookup"><span data-stu-id="f0cfd-130">Response</span></span>

<span data-ttu-id="f0cfd-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[workbookRangeBorder](../resources/workbookrangeborder.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f0cfd-131">If successful, this method returns a `200 OK` response code and [workbookRangeBorder](../resources/workbookrangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f0cfd-132">例</span><span class="sxs-lookup"><span data-stu-id="f0cfd-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0cfd-133">要求</span><span class="sxs-lookup"><span data-stu-id="f0cfd-133">Request</span></span>
<span data-ttu-id="f0cfd-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f0cfd-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f0cfd-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="f0cfd-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rangeborder"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/borders/{sideIndex}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f0cfd-136">C#</span><span class="sxs-lookup"><span data-stu-id="f0cfd-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rangeborder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f0cfd-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="f0cfd-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rangeborder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f0cfd-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="f0cfd-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rangeborder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f0cfd-139">応答</span><span class="sxs-lookup"><span data-stu-id="f0cfd-139">Response</span></span>
<span data-ttu-id="f0cfd-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f0cfd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "Get RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
