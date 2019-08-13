---
title: Create ChartPoints
description: この API を使用して、新しい ChartPoints を作成します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 057f8be5fa646cef0a5d39fe758e8901b9e4c583
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36316747"
---
# <a name="create-chartpoint"></a><span data-ttu-id="a7c34-103">ChartPoint を作成する</span><span class="sxs-lookup"><span data-stu-id="a7c34-103">Create ChartPoint</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7c34-104">この API を使用して、新しい ChartPoint を作成します。</span><span class="sxs-lookup"><span data-stu-id="a7c34-104">Use this API to create a new ChartPoint.</span></span>
## <a name="permissions"></a><span data-ttu-id="a7c34-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a7c34-105">Permissions</span></span>
<span data-ttu-id="a7c34-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a7c34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7c34-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a7c34-108">Permission type</span></span>      | <span data-ttu-id="a7c34-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a7c34-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7c34-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a7c34-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a7c34-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7c34-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a7c34-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a7c34-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7c34-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7c34-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a7c34-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a7c34-114">Application</span></span> | <span data-ttu-id="a7c34-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7c34-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7c34-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a7c34-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points

```
## <a name="request-headers"></a><span data-ttu-id="a7c34-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a7c34-117">Request headers</span></span>
| <span data-ttu-id="a7c34-118">名前</span><span class="sxs-lookup"><span data-stu-id="a7c34-118">Name</span></span>       | <span data-ttu-id="a7c34-119">説明</span><span class="sxs-lookup"><span data-stu-id="a7c34-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a7c34-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7c34-120">Authorization</span></span>  | <span data-ttu-id="a7c34-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a7c34-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a7c34-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a7c34-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="a7c34-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="a7c34-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7c34-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a7c34-126">Request body</span></span>
<span data-ttu-id="a7c34-127">要求本文で、 [workbookChartPoint](../resources/workbookchartpoint.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a7c34-127">In the request body, supply a JSON representation of [workbookChartPoint](../resources/workbookchartpoint.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a7c34-128">応答</span><span class="sxs-lookup"><span data-stu-id="a7c34-128">Response</span></span>

<span data-ttu-id="a7c34-129">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[workbookChartPoint](../resources/workbookchartpoint.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a7c34-129">If successful, this method returns `201 Created` response code and [workbookChartPoint](../resources/workbookchartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7c34-130">例</span><span class="sxs-lookup"><span data-stu-id="a7c34-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7c34-131">要求</span><span class="sxs-lookup"><span data-stu-id="a7c34-131">Request</span></span>
<span data-ttu-id="a7c34-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a7c34-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a7c34-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a7c34-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chartpoints_from_chartseries"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points
Content-type: application/json
Content-length: 3

{
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a7c34-134">C#</span><span class="sxs-lookup"><span data-stu-id="a7c34-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chartpoints-from-chartseries-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a7c34-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7c34-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chartpoints-from-chartseries-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a7c34-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="a7c34-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chartpoints-from-chartseries-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a7c34-137">Java</span><span class="sxs-lookup"><span data-stu-id="a7c34-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chartpoints-from-chartseries-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a7c34-138">要求本文で、 [workbookChartPoint](../resources/workbookchartpoint.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a7c34-138">In the request body, supply a JSON representation of [workbookChartPoint](../resources/workbookchartpoint.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a7c34-139">応答</span><span class="sxs-lookup"><span data-stu-id="a7c34-139">Response</span></span>
<span data-ttu-id="a7c34-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a7c34-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartPoint"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 3

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create ChartPoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
