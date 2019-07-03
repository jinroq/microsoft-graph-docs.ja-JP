---
title: Create ChartSeries
description: この API を使用して、新しい ChartSeries を作成します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 95b734e5fa77b5700752e43b3964ae0dba73c680
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443596"
---
# <a name="create-chartseries"></a><span data-ttu-id="e1ada-103">Create ChartSeries</span><span class="sxs-lookup"><span data-stu-id="e1ada-103">Create ChartSeries</span></span>

<span data-ttu-id="e1ada-104">この API を使用して、新しい ChartSeries を作成します。</span><span class="sxs-lookup"><span data-stu-id="e1ada-104">Use this API to create a new ChartSeries.</span></span>
## <a name="permissions"></a><span data-ttu-id="e1ada-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e1ada-105">Permissions</span></span>
<span data-ttu-id="e1ada-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e1ada-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1ada-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e1ada-108">Permission type</span></span>      | <span data-ttu-id="e1ada-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e1ada-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1ada-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e1ada-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e1ada-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1ada-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e1ada-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e1ada-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1ada-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1ada-113">Not supported.</span></span>    |
|<span data-ttu-id="e1ada-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e1ada-114">Application</span></span> | <span data-ttu-id="e1ada-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1ada-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1ada-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e1ada-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series

```
## <a name="request-headers"></a><span data-ttu-id="e1ada-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e1ada-117">Request headers</span></span>
| <span data-ttu-id="e1ada-118">名前</span><span class="sxs-lookup"><span data-stu-id="e1ada-118">Name</span></span>       | <span data-ttu-id="e1ada-119">説明</span><span class="sxs-lookup"><span data-stu-id="e1ada-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e1ada-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1ada-120">Authorization</span></span>  | <span data-ttu-id="e1ada-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e1ada-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e1ada-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e1ada-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e1ada-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="e1ada-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1ada-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e1ada-126">Request body</span></span>
<span data-ttu-id="e1ada-127">要求本文で、 [WorkbookChartSeries](../resources/chartseries.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e1ada-127">In the request body, supply a JSON representation of [WorkbookChartSeries](../resources/chartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e1ada-128">応答</span><span class="sxs-lookup"><span data-stu-id="e1ada-128">Response</span></span>

<span data-ttu-id="e1ada-129">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[WorkbookChartSeries](../resources/chartseries.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e1ada-129">If successful, this method returns `201 Created` response code and [WorkbookChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1ada-130">例</span><span class="sxs-lookup"><span data-stu-id="e1ada-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1ada-131">要求</span><span class="sxs-lookup"><span data-stu-id="e1ada-131">Request</span></span>
<span data-ttu-id="e1ada-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e1ada-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e1ada-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e1ada-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chartseries_from_chart"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e1ada-134">C#</span><span class="sxs-lookup"><span data-stu-id="e1ada-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chartseries-from-chart-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1ada-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="e1ada-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chartseries-from-chart-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e1ada-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="e1ada-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chartseries-from-chart-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="e1ada-137">要求本文で、 [WorkbookChartSeries](../resources/chartseries.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e1ada-137">In the request body, supply a JSON representation of [WorkbookChartSeries](../resources/chartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e1ada-138">応答</span><span class="sxs-lookup"><span data-stu-id="e1ada-138">Response</span></span>
<span data-ttu-id="e1ada-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e1ada-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ChartSeries",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
