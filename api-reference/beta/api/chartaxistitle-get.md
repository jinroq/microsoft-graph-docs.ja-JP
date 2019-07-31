---
title: WorkbookChartAxisTitle を取得する
description: Workbookchartaxistitle オブジェクトのプロパティとリレーションシップを取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 3052d8249a153fd11fdf0b58c4109d0518f9f96c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944052"
---
# <a name="get-workbookchartaxistitle"></a><span data-ttu-id="0a228-103">WorkbookChartAxisTitle を取得する</span><span class="sxs-lookup"><span data-stu-id="0a228-103">Get workbookChartAxisTitle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a228-104">chartaxistitle オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="0a228-104">Retrieve the properties and relationships of chartaxistitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0a228-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0a228-105">Permissions</span></span>
<span data-ttu-id="0a228-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a228-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a228-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0a228-108">Permission type</span></span>      | <span data-ttu-id="0a228-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0a228-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a228-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0a228-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0a228-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a228-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0a228-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0a228-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a228-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a228-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0a228-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0a228-114">Application</span></span> | <span data-ttu-id="0a228-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a228-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a228-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0a228-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/title
GET /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/title
GET /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/title
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0a228-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0a228-117">Optional query parameters</span></span>
<span data-ttu-id="0a228-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0a228-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0a228-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a228-119">Request headers</span></span>
| <span data-ttu-id="0a228-120">名前</span><span class="sxs-lookup"><span data-stu-id="0a228-120">Name</span></span>      |<span data-ttu-id="0a228-121">説明</span><span class="sxs-lookup"><span data-stu-id="0a228-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0a228-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a228-122">Authorization</span></span>  | <span data-ttu-id="0a228-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0a228-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0a228-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0a228-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="0a228-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="0a228-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a228-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="0a228-128">Request body</span></span>
<span data-ttu-id="0a228-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0a228-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a228-130">応答</span><span class="sxs-lookup"><span data-stu-id="0a228-130">Response</span></span>

<span data-ttu-id="0a228-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[workbookChartAxisTitle](../resources/workbookchartaxistitle.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0a228-131">If successful, this method returns a `200 OK` response code and [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0a228-132">例</span><span class="sxs-lookup"><span data-stu-id="0a228-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0a228-133">要求</span><span class="sxs-lookup"><span data-stu-id="0a228-133">Request</span></span>
<span data-ttu-id="0a228-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0a228-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0a228-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0a228-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartaxistitle"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/title
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0a228-136">C#</span><span class="sxs-lookup"><span data-stu-id="0a228-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartaxistitle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0a228-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="0a228-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartaxistitle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0a228-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="0a228-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartaxistitle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0a228-139">Java</span><span class="sxs-lookup"><span data-stu-id="0a228-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chartaxistitle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0a228-140">応答</span><span class="sxs-lookup"><span data-stu-id="0a228-140">Response</span></span>
<span data-ttu-id="0a228-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0a228-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartAxisTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get ChartAxisTitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
