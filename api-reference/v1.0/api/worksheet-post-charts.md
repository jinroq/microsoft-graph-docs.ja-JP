---
title: グラフを作成します。
description: この API を使用して、新しいグラフを作成します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 562d1b347fc0ddb2abfa89e44831b32cca2a57e3
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33601355"
---
# <a name="create-chart"></a><span data-ttu-id="8f011-103">グラフを作成します。</span><span class="sxs-lookup"><span data-stu-id="8f011-103">Create Chart</span></span>

<span data-ttu-id="8f011-104">この API を使用して、新しいグラフを作成します。</span><span class="sxs-lookup"><span data-stu-id="8f011-104">Use this API to create a new Chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="8f011-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8f011-105">Permissions</span></span>
<span data-ttu-id="8f011-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8f011-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f011-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8f011-108">Permission type</span></span>      | <span data-ttu-id="8f011-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8f011-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f011-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8f011-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8f011-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f011-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8f011-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8f011-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f011-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8f011-113">Not supported.</span></span>    |
|<span data-ttu-id="8f011-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8f011-114">Application</span></span> | <span data-ttu-id="8f011-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8f011-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f011-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8f011-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/

```
## <a name="request-headers"></a><span data-ttu-id="8f011-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8f011-117">Request headers</span></span>
| <span data-ttu-id="8f011-118">名前</span><span class="sxs-lookup"><span data-stu-id="8f011-118">Name</span></span>       | <span data-ttu-id="8f011-119">説明</span><span class="sxs-lookup"><span data-stu-id="8f011-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8f011-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f011-120">Authorization</span></span>  | <span data-ttu-id="8f011-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8f011-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f011-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8f011-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8f011-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="8f011-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f011-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8f011-126">Request body</span></span>
<span data-ttu-id="8f011-127">要求本文で、 [WorkbookChart](../resources/chart.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8f011-127">In the request body, supply a JSON representation of [WorkbookChart](../resources/chart.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8f011-128">応答</span><span class="sxs-lookup"><span data-stu-id="8f011-128">Response</span></span>

<span data-ttu-id="8f011-129">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[WorkbookChart](../resources/chart.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8f011-129">If successful, this method returns `201 Created` response code and [WorkbookChart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f011-130">例</span><span class="sxs-lookup"><span data-stu-id="8f011-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8f011-131">要求</span><span class="sxs-lookup"><span data-stu-id="8f011-131">Request</span></span>
<span data-ttu-id="8f011-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8f011-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chart_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```
<span data-ttu-id="8f011-133">要求本文で、 [WorkbookChart](../resources/chart.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8f011-133">In the request body, supply a JSON representation of [WorkbookChart](../resources/chart.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8f011-134">応答</span><span class="sxs-lookup"><span data-stu-id="8f011-134">Response</span></span>
<span data-ttu-id="8f011-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8f011-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8f011-138">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="8f011-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8f011-139">Visual</span><span class="sxs-lookup"><span data-stu-id="8f011-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_chart_from_worksheet-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f011-140">Java</span><span class="sxs-lookup"><span data-stu-id="8f011-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_chart_from_worksheet-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/worksheet-post-charts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/worksheet-post-charts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
