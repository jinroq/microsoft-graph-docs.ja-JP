---
title: 'Chart: setData'
description: グラフのソース データをリセットします。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ef1f973cae35b2d908c060475b9c2bd04b982525
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443582"
---
# <a name="chart-setdata"></a><span data-ttu-id="d3ac9-103">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="d3ac9-103">Chart: setData</span></span>

<span data-ttu-id="d3ac9-104">グラフのソース データをリセットします。</span><span class="sxs-lookup"><span data-stu-id="d3ac9-104">Resets the source data for the chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="d3ac9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d3ac9-105">Permissions</span></span>
<span data-ttu-id="d3ac9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d3ac9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3ac9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d3ac9-108">Permission type</span></span>      | <span data-ttu-id="d3ac9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d3ac9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3ac9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d3ac9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d3ac9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3ac9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d3ac9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d3ac9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3ac9-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3ac9-113">Not supported.</span></span>    |
|<span data-ttu-id="d3ac9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d3ac9-114">Application</span></span> | <span data-ttu-id="d3ac9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3ac9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3ac9-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d3ac9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/setData

```
## <a name="request-headers"></a><span data-ttu-id="d3ac9-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d3ac9-117">Request headers</span></span>
| <span data-ttu-id="d3ac9-118">名前</span><span class="sxs-lookup"><span data-stu-id="d3ac9-118">Name</span></span>       | <span data-ttu-id="d3ac9-119">説明</span><span class="sxs-lookup"><span data-stu-id="d3ac9-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d3ac9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3ac9-120">Authorization</span></span>  | <span data-ttu-id="d3ac9-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d3ac9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d3ac9-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d3ac9-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d3ac9-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="d3ac9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3ac9-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d3ac9-126">Request body</span></span>
<span data-ttu-id="d3ac9-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="d3ac9-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d3ac9-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="d3ac9-128">Parameter</span></span>    | <span data-ttu-id="d3ac9-129">型</span><span class="sxs-lookup"><span data-stu-id="d3ac9-129">Type</span></span>   |<span data-ttu-id="d3ac9-130">説明</span><span class="sxs-lookup"><span data-stu-id="d3ac9-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3ac9-131">sourceData</span><span class="sxs-lookup"><span data-stu-id="d3ac9-131">sourceData</span></span>|<span data-ttu-id="d3ac9-132">Json</span><span class="sxs-lookup"><span data-stu-id="d3ac9-132">Json</span></span>|<span data-ttu-id="d3ac9-133">データ ソースに対応する Range オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="d3ac9-133">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="d3ac9-134">seriesBy</span><span class="sxs-lookup"><span data-stu-id="d3ac9-134">seriesBy</span></span>|<span data-ttu-id="d3ac9-135">string</span><span class="sxs-lookup"><span data-stu-id="d3ac9-135">string</span></span>|<span data-ttu-id="d3ac9-136">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d3ac9-136">Optional.</span></span> <span data-ttu-id="d3ac9-137">列や行がグラフのデータ系列として使用される方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="d3ac9-137">Specifies the way columns or rows are used as data series on the chart.</span></span> <span data-ttu-id="d3ac9-138">Auto (既定)、行、列のいずれかをすることができます。</span><span class="sxs-lookup"><span data-stu-id="d3ac9-138">Can be one of the following: Auto (default), Rows, Columns.</span></span>  <span data-ttu-id="d3ac9-139">使用可能な値: `Auto`、`Columns`、`Rows`。</span><span class="sxs-lookup"><span data-stu-id="d3ac9-139">The possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="d3ac9-140">応答</span><span class="sxs-lookup"><span data-stu-id="d3ac9-140">Response</span></span>

<span data-ttu-id="d3ac9-p105">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="d3ac9-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3ac9-143">例</span><span class="sxs-lookup"><span data-stu-id="d3ac9-143">Example</span></span>
<span data-ttu-id="d3ac9-144">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="d3ac9-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d3ac9-145">要求</span><span class="sxs-lookup"><span data-stu-id="d3ac9-145">Request</span></span>
<span data-ttu-id="d3ac9-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d3ac9-146">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d3ac9-147">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d3ac9-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chart_setdata"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setData
Content-type: application/json
Content-length: 70

{
  "sourceData": "sourceData-value",
  "seriesBy": "seriesBy-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d3ac9-148">C#</span><span class="sxs-lookup"><span data-stu-id="d3ac9-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chart-setdata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3ac9-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="d3ac9-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chart-setdata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d3ac9-150">目的-C</span><span class="sxs-lookup"><span data-stu-id="d3ac9-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chart-setdata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d3ac9-151">応答</span><span class="sxs-lookup"><span data-stu-id="d3ac9-151">Response</span></span>
<span data-ttu-id="d3ac9-152">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d3ac9-152">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: setData",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
