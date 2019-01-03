---
title: RangeFormat を取得する
description: rangeformat オブジェクトのプロパティと関係を取得します。
author: lumine2008
ms.openlocfilehash: 180f9a0088e0c6f724e4983acdb51f87458962ee
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304789"
---
# <a name="get-rangeformat"></a><span data-ttu-id="f3088-103">RangeFormat を取得する</span><span class="sxs-lookup"><span data-stu-id="f3088-103">Get RangeFormat</span></span>

<span data-ttu-id="f3088-104">rangeformat オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="f3088-104">Retrieve the properties and relationships of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f3088-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f3088-105">Permissions</span></span>
<span data-ttu-id="f3088-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3088-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3088-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f3088-108">Permission type</span></span>      | <span data-ttu-id="f3088-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f3088-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3088-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f3088-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f3088-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3088-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f3088-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f3088-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3088-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3088-113">Not supported.</span></span>    |
|<span data-ttu-id="f3088-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f3088-114">Application</span></span> | <span data-ttu-id="f3088-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3088-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3088-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f3088-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format
GET /workbook/worksheets/{id|name}/range(address='<address>')/format
GET /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f3088-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f3088-117">Optional query parameters</span></span>
<span data-ttu-id="f3088-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f3088-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f3088-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3088-119">Request headers</span></span>
| <span data-ttu-id="f3088-120">名前</span><span class="sxs-lookup"><span data-stu-id="f3088-120">Name</span></span>      |<span data-ttu-id="f3088-121">説明</span><span class="sxs-lookup"><span data-stu-id="f3088-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f3088-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3088-122">Authorization</span></span>  | <span data-ttu-id="f3088-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f3088-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f3088-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f3088-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f3088-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="f3088-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3088-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="f3088-128">Request body</span></span>
<span data-ttu-id="f3088-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f3088-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3088-130">応答</span><span class="sxs-lookup"><span data-stu-id="f3088-130">Response</span></span>

<span data-ttu-id="f3088-131">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[WorkbookRangeFormat](../resources/rangeformat.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f3088-131">If successful, this method returns a `200 OK` response code and [WorkbookRangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f3088-132">例</span><span class="sxs-lookup"><span data-stu-id="f3088-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f3088-133">要求</span><span class="sxs-lookup"><span data-stu-id="f3088-133">Request</span></span>
<span data-ttu-id="f3088-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f3088-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rangeformat"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format
```
##### <a name="response"></a><span data-ttu-id="f3088-135">応答</span><span class="sxs-lookup"><span data-stu-id="f3088-135">Response</span></span>
<span data-ttu-id="f3088-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f3088-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 96

{
  "columnWidth": 99,
  "horizontalAlignment": "horizontalAlignment-value",
  "rowHeight": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get RangeFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->