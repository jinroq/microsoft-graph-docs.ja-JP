---
title: 'Chart: setData'
description: グラフのソース データをリセットします。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: acde87f47f4972d2a6b84556cf2458b53158db59
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35438322"
---
# <a name="chart-setdata"></a><span data-ttu-id="b3670-103">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="b3670-103">Chart: setData</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3670-104">グラフのソース データをリセットします。</span><span class="sxs-lookup"><span data-stu-id="b3670-104">Resets the source data for the chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="b3670-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b3670-105">Permissions</span></span>
<span data-ttu-id="b3670-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b3670-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3670-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b3670-108">Permission type</span></span>      | <span data-ttu-id="b3670-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b3670-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3670-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b3670-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b3670-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b3670-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b3670-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b3670-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3670-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b3670-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b3670-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b3670-114">Application</span></span> | <span data-ttu-id="b3670-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3670-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3670-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b3670-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/setData

```
## <a name="request-headers"></a><span data-ttu-id="b3670-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b3670-117">Request headers</span></span>
| <span data-ttu-id="b3670-118">名前</span><span class="sxs-lookup"><span data-stu-id="b3670-118">Name</span></span>       | <span data-ttu-id="b3670-119">説明</span><span class="sxs-lookup"><span data-stu-id="b3670-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b3670-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3670-120">Authorization</span></span>  | <span data-ttu-id="b3670-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b3670-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b3670-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b3670-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="b3670-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="b3670-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3670-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b3670-126">Request body</span></span>
<span data-ttu-id="b3670-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b3670-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b3670-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b3670-128">Parameter</span></span>    | <span data-ttu-id="b3670-129">型</span><span class="sxs-lookup"><span data-stu-id="b3670-129">Type</span></span>   |<span data-ttu-id="b3670-130">説明</span><span class="sxs-lookup"><span data-stu-id="b3670-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b3670-131">sourceData</span><span class="sxs-lookup"><span data-stu-id="b3670-131">sourceData</span></span>|<span data-ttu-id="b3670-132">string</span><span class="sxs-lookup"><span data-stu-id="b3670-132">string</span></span>|<span data-ttu-id="b3670-133">データ ソースに対応する Range オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b3670-133">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="b3670-134">seriesBy</span><span class="sxs-lookup"><span data-stu-id="b3670-134">seriesBy</span></span>|<span data-ttu-id="b3670-135">string</span><span class="sxs-lookup"><span data-stu-id="b3670-135">string</span></span>|<span data-ttu-id="b3670-p104">省略可能。列や行がグラフのデータ系列として使用される方法を指定します。次のいずれかを指定できます。自動 (既定)、行、列。可能な値は、`Auto`、`Columns`、`Rows` です。</span><span class="sxs-lookup"><span data-stu-id="b3670-p104">Optional. Specifies the way columns or rows are used as data series on the chart. Can be one of the following: Auto (default), Rows, Columns.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="b3670-140">応答</span><span class="sxs-lookup"><span data-stu-id="b3670-140">Response</span></span>

<span data-ttu-id="b3670-p105">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b3670-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3670-143">例</span><span class="sxs-lookup"><span data-stu-id="b3670-143">Example</span></span>
<span data-ttu-id="b3670-144">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="b3670-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b3670-145">要求</span><span class="sxs-lookup"><span data-stu-id="b3670-145">Request</span></span>
<span data-ttu-id="b3670-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b3670-146">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b3670-147">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b3670-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chart_setdata"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setData
Content-type: application/json
Content-length: 70

{
  "sourceData": "sourceData-value",
  "seriesBy": "seriesBy-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b3670-148">C#</span><span class="sxs-lookup"><span data-stu-id="b3670-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chart-setdata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b3670-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="b3670-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chart-setdata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b3670-150">目的-C</span><span class="sxs-lookup"><span data-stu-id="b3670-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chart-setdata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b3670-151">応答</span><span class="sxs-lookup"><span data-stu-id="b3670-151">Response</span></span>
<span data-ttu-id="b3670-152">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b3670-152">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Chart: setData",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
