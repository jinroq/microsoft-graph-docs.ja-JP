---
title: RangeFont を取得する
description: rangefont オブジェクトのプロパティと関係を取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5da9cb678f2067b51314f0ee9e433020ce883a97
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455785"
---
# <a name="get-rangefont"></a><span data-ttu-id="db9ec-103">RangeFont を取得する</span><span class="sxs-lookup"><span data-stu-id="db9ec-103">Get RangeFont</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db9ec-104">rangefont オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="db9ec-104">Retrieve the properties and relationships of rangefont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="db9ec-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="db9ec-105">Permissions</span></span>
<span data-ttu-id="db9ec-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="db9ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db9ec-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="db9ec-108">Permission type</span></span>      | <span data-ttu-id="db9ec-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="db9ec-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db9ec-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="db9ec-110">Delegated (work or school account)</span></span> | <span data-ttu-id="db9ec-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db9ec-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="db9ec-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="db9ec-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db9ec-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db9ec-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="db9ec-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="db9ec-114">Application</span></span> | <span data-ttu-id="db9ec-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db9ec-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="db9ec-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="db9ec-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format/font
GET /workbook/worksheets/{id|name}/range(address='<address>')/format/font
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/font
```
## <a name="optional-query-parameters"></a><span data-ttu-id="db9ec-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="db9ec-117">Optional query parameters</span></span>
<span data-ttu-id="db9ec-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="db9ec-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="db9ec-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="db9ec-119">Request headers</span></span>
| <span data-ttu-id="db9ec-120">名前</span><span class="sxs-lookup"><span data-stu-id="db9ec-120">Name</span></span>      |<span data-ttu-id="db9ec-121">説明</span><span class="sxs-lookup"><span data-stu-id="db9ec-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="db9ec-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="db9ec-122">Authorization</span></span>  | <span data-ttu-id="db9ec-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="db9ec-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="db9ec-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="db9ec-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="db9ec-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="db9ec-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="db9ec-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="db9ec-128">Request body</span></span>
<span data-ttu-id="db9ec-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="db9ec-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db9ec-130">応答</span><span class="sxs-lookup"><span data-stu-id="db9ec-130">Response</span></span>

<span data-ttu-id="db9ec-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[workbookRangeFont](../resources/workbookrangefont.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="db9ec-131">If successful, this method returns a `200 OK` response code and [workbookRangeFont](../resources/workbookrangefont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="db9ec-132">例</span><span class="sxs-lookup"><span data-stu-id="db9ec-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db9ec-133">要求</span><span class="sxs-lookup"><span data-stu-id="db9ec-133">Request</span></span>
<span data-ttu-id="db9ec-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="db9ec-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="db9ec-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="db9ec-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rangefont"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/font
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db9ec-136">C#</span><span class="sxs-lookup"><span data-stu-id="db9ec-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rangefont-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db9ec-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="db9ec-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rangefont-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db9ec-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="db9ec-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rangefont-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="db9ec-139">応答</span><span class="sxs-lookup"><span data-stu-id="db9ec-139">Response</span></span>
<span data-ttu-id="db9ec-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="db9ec-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get RangeFont",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
