---
title: 'Chart: setData'
description: グラフのソース データをリセットします。
author: lumine2008
ms.openlocfilehash: 91e46e519ab590388aad17eb30e9ca2ea19c90f8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325810"
---
# <a name="chart-setdata"></a><span data-ttu-id="a8697-103">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="a8697-103">Chart: setData</span></span>

> <span data-ttu-id="a8697-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a8697-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8697-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8697-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a8697-106">グラフのソース データをリセットします。</span><span class="sxs-lookup"><span data-stu-id="a8697-106">Resets the source data for the chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="a8697-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a8697-107">Permissions</span></span>
<span data-ttu-id="a8697-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a8697-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8697-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a8697-110">Permission type</span></span>      | <span data-ttu-id="a8697-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a8697-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8697-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a8697-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a8697-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8697-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a8697-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a8697-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8697-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8697-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a8697-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a8697-116">Application</span></span> | <span data-ttu-id="a8697-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8697-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8697-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a8697-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setData

```
## <a name="request-headers"></a><span data-ttu-id="a8697-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a8697-119">Request headers</span></span>
| <span data-ttu-id="a8697-120">名前</span><span class="sxs-lookup"><span data-stu-id="a8697-120">Name</span></span>       | <span data-ttu-id="a8697-121">説明</span><span class="sxs-lookup"><span data-stu-id="a8697-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a8697-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8697-122">Authorization</span></span>  | <span data-ttu-id="a8697-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a8697-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a8697-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a8697-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="a8697-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="a8697-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8697-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="a8697-128">Request body</span></span>
<span data-ttu-id="a8697-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="a8697-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a8697-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="a8697-130">Parameter</span></span>    | <span data-ttu-id="a8697-131">種類</span><span class="sxs-lookup"><span data-stu-id="a8697-131">Type</span></span>   |<span data-ttu-id="a8697-132">説明</span><span class="sxs-lookup"><span data-stu-id="a8697-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8697-133">sourceData</span><span class="sxs-lookup"><span data-stu-id="a8697-133">sourceData</span></span>|<span data-ttu-id="a8697-134">string</span><span class="sxs-lookup"><span data-stu-id="a8697-134">string</span></span>|<span data-ttu-id="a8697-135">データ ソースに対応する Range オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a8697-135">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="a8697-136">seriesBy</span><span class="sxs-lookup"><span data-stu-id="a8697-136">seriesBy</span></span>|<span data-ttu-id="a8697-137">文字列</span><span class="sxs-lookup"><span data-stu-id="a8697-137">string</span></span>|<span data-ttu-id="a8697-p105">省略可能。列や行がグラフのデータ系列として使用される方法を指定します。次のいずれかを指定できます。自動 (既定)、行、列。可能な値は、`Auto`、`Columns`、`Rows` です。</span><span class="sxs-lookup"><span data-stu-id="a8697-p105">Optional. Specifies the way columns or rows are used as data series on the chart. Can be one of the following: Auto (default), Rows, Columns.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="a8697-142">応答</span><span class="sxs-lookup"><span data-stu-id="a8697-142">Response</span></span>

<span data-ttu-id="a8697-p106">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="a8697-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8697-145">例</span><span class="sxs-lookup"><span data-stu-id="a8697-145">Example</span></span>
<span data-ttu-id="a8697-146">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="a8697-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a8697-147">要求</span><span class="sxs-lookup"><span data-stu-id="a8697-147">Request</span></span>
<span data-ttu-id="a8697-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a8697-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setdata"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/setData
Content-type: application/json
Content-length: 70

{
  "sourceData": "sourceData-value",
  "seriesBy": "seriesBy-value"
}
```

##### <a name="response"></a><span data-ttu-id="a8697-149">応答</span><span class="sxs-lookup"><span data-stu-id="a8697-149">Response</span></span>
<span data-ttu-id="a8697-150">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="a8697-150">Here is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "Chart: setData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->