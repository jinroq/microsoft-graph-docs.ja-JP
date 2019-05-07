---
title: WorkbookChartDataLabels を取得する
description: Workbookchartdatalabels オブジェクトのプロパティとリレーションシップを取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 97ea5fac73e055a2f10967b0dd4e98235b9b33a7
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635541"
---
# <a name="get-chartdatalabels"></a><span data-ttu-id="eaaf3-103">Get ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="eaaf3-103">Get ChartDataLabels</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eaaf3-104">chartdatalabels オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="eaaf3-104">Retrieve the properties and relationships of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="eaaf3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="eaaf3-105">Permissions</span></span>
<span data-ttu-id="eaaf3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eaaf3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eaaf3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eaaf3-108">Permission type</span></span>      | <span data-ttu-id="eaaf3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="eaaf3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eaaf3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eaaf3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="eaaf3-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eaaf3-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="eaaf3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eaaf3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eaaf3-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eaaf3-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="eaaf3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eaaf3-114">Application</span></span> | <span data-ttu-id="eaaf3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eaaf3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eaaf3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eaaf3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/datalabels
```
## <a name="optional-query-parameters"></a><span data-ttu-id="eaaf3-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="eaaf3-117">Optional query parameters</span></span>
<span data-ttu-id="eaaf3-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="eaaf3-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eaaf3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eaaf3-119">Request headers</span></span>
| <span data-ttu-id="eaaf3-120">名前</span><span class="sxs-lookup"><span data-stu-id="eaaf3-120">Name</span></span>      |<span data-ttu-id="eaaf3-121">説明</span><span class="sxs-lookup"><span data-stu-id="eaaf3-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eaaf3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eaaf3-122">Authorization</span></span>  | <span data-ttu-id="eaaf3-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="eaaf3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eaaf3-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="eaaf3-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="eaaf3-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="eaaf3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eaaf3-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="eaaf3-128">Request body</span></span>
<span data-ttu-id="eaaf3-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="eaaf3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eaaf3-130">応答</span><span class="sxs-lookup"><span data-stu-id="eaaf3-130">Response</span></span>

<span data-ttu-id="eaaf3-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[workbookChartDataLabels](../resources/workbookchartdatalabels.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="eaaf3-131">If successful, this method returns a `200 OK` response code and [workbookChartDataLabels](../resources/workbookchartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eaaf3-132">例</span><span class="sxs-lookup"><span data-stu-id="eaaf3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eaaf3-133">要求</span><span class="sxs-lookup"><span data-stu-id="eaaf3-133">Request</span></span>
<span data-ttu-id="eaaf3-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="eaaf3-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartdatalabels"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/datalabels
```
##### <a name="response"></a><span data-ttu-id="eaaf3-135">応答</span><span class="sxs-lookup"><span data-stu-id="eaaf3-135">Response</span></span>
<span data-ttu-id="eaaf3-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="eaaf3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartDataLabels"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "position": "position-value",
  "showValue": true,
  "showSeriesName": true,
  "showCategoryName": true,
  "showLegendKey": true
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="eaaf3-139">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="eaaf3-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="eaaf3-140">Visual</span><span class="sxs-lookup"><span data-stu-id="eaaf3-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_chartdatalabels-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eaaf3-141">Java</span><span class="sxs-lookup"><span data-stu-id="eaaf3-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_chartdatalabels-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get ChartDataLabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartdatalabels-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/chartdatalabels-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
