---
title: RangeFill を取得する
description: rangefill オブジェクトのプロパティと関係を取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 147e41e16e373085f9ed2cf17765b3acae1fcd35
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459763"
---
# <a name="get-rangefill"></a><span data-ttu-id="be391-103">RangeFill を取得する</span><span class="sxs-lookup"><span data-stu-id="be391-103">Get RangeFill</span></span>

<span data-ttu-id="be391-104">rangefill オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="be391-104">Retrieve the properties and relationships of rangefill object.</span></span>
## <a name="permissions"></a><span data-ttu-id="be391-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="be391-105">Permissions</span></span>
<span data-ttu-id="be391-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be391-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be391-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="be391-108">Permission type</span></span>      | <span data-ttu-id="be391-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="be391-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be391-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="be391-110">Delegated (work or school account)</span></span> | <span data-ttu-id="be391-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be391-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="be391-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="be391-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be391-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be391-113">Not supported.</span></span>    |
|<span data-ttu-id="be391-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="be391-114">Application</span></span> | <span data-ttu-id="be391-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be391-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be391-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="be391-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format/fill
GET /workbook/worksheets/{id|name}/range(address='<address>')/format/fill
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/fill
```
## <a name="optional-query-parameters"></a><span data-ttu-id="be391-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="be391-117">Optional query parameters</span></span>
<span data-ttu-id="be391-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="be391-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be391-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="be391-119">Request headers</span></span>
| <span data-ttu-id="be391-120">名前</span><span class="sxs-lookup"><span data-stu-id="be391-120">Name</span></span>      |<span data-ttu-id="be391-121">説明</span><span class="sxs-lookup"><span data-stu-id="be391-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="be391-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="be391-122">Authorization</span></span>  | <span data-ttu-id="be391-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="be391-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="be391-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="be391-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="be391-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="be391-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="be391-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="be391-128">Request body</span></span>
<span data-ttu-id="be391-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="be391-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be391-130">応答</span><span class="sxs-lookup"><span data-stu-id="be391-130">Response</span></span>

<span data-ttu-id="be391-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[WorkbookRangeFill](../resources/rangefill.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="be391-131">If successful, this method returns a `200 OK` response code and [WorkbookRangeFill](../resources/rangefill.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="be391-132">例</span><span class="sxs-lookup"><span data-stu-id="be391-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be391-133">要求</span><span class="sxs-lookup"><span data-stu-id="be391-133">Request</span></span>
<span data-ttu-id="be391-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="be391-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="be391-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="be391-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rangefill"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/fill
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="be391-136">C#</span><span class="sxs-lookup"><span data-stu-id="be391-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rangefill-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="be391-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="be391-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rangefill-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="be391-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="be391-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rangefill-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="be391-139">応答</span><span class="sxs-lookup"><span data-stu-id="be391-139">Response</span></span>
<span data-ttu-id="be391-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="be391-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get RangeFill",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
