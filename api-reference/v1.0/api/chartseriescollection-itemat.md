---
title: 'ChartSeriesCollection: ItemAt'
description: コレクション内の位置に基づいてデータ系列を取得します。
author: lumine2008
ms.openlocfilehash: 9a61617fff9322452698761696a5f5a4f2d110ef
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331753"
---
# <a name="chartseriescollection-itemat"></a><span data-ttu-id="37a2e-103">ChartSeriesCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="37a2e-103">ChartSeriesCollection: ItemAt</span></span>

<span data-ttu-id="37a2e-104">コレクション内の位置に基づいてデータ系列を取得します。</span><span class="sxs-lookup"><span data-stu-id="37a2e-104">Retrieves a series based on its position in the collection</span></span>
## <a name="permissions"></a><span data-ttu-id="37a2e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="37a2e-105">Permissions</span></span>
<span data-ttu-id="37a2e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="37a2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37a2e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="37a2e-108">Permission type</span></span>      | <span data-ttu-id="37a2e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="37a2e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37a2e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="37a2e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="37a2e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37a2e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="37a2e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="37a2e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37a2e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37a2e-113">Not supported.</span></span>    |
|<span data-ttu-id="37a2e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="37a2e-114">Application</span></span> | <span data-ttu-id="37a2e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37a2e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="37a2e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="37a2e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="37a2e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="37a2e-117">Request headers</span></span>
| <span data-ttu-id="37a2e-118">名前</span><span class="sxs-lookup"><span data-stu-id="37a2e-118">Name</span></span>       | <span data-ttu-id="37a2e-119">説明</span><span class="sxs-lookup"><span data-stu-id="37a2e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="37a2e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="37a2e-120">Authorization</span></span>  | <span data-ttu-id="37a2e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="37a2e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="37a2e-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="37a2e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="37a2e-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="37a2e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="37a2e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="37a2e-126">Request body</span></span>
<span data-ttu-id="37a2e-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="37a2e-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="37a2e-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="37a2e-128">Parameter</span></span>    | <span data-ttu-id="37a2e-129">種類</span><span class="sxs-lookup"><span data-stu-id="37a2e-129">Type</span></span>   |<span data-ttu-id="37a2e-130">説明</span><span class="sxs-lookup"><span data-stu-id="37a2e-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37a2e-131">index</span><span class="sxs-lookup"><span data-stu-id="37a2e-131">index</span></span>|<span data-ttu-id="37a2e-132">Int32</span><span class="sxs-lookup"><span data-stu-id="37a2e-132">Int32</span></span>|<span data-ttu-id="37a2e-p104">取得するオブジェクトのインデックス値。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="37a2e-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="37a2e-135">応答</span><span class="sxs-lookup"><span data-stu-id="37a2e-135">Response</span></span>

<span data-ttu-id="37a2e-136">かどうかは成功すると、このメソッドを返します`200 OK`応答コードおよび応答の本文に[WorkbookChartSeries](../resources/chartseries.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="37a2e-136">If successful, this method returns `200 OK` response code and [WorkbookChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37a2e-137">例</span><span class="sxs-lookup"><span data-stu-id="37a2e-137">Example</span></span>
<span data-ttu-id="37a2e-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="37a2e-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="37a2e-139">要求</span><span class="sxs-lookup"><span data-stu-id="37a2e-139">Request</span></span>
<span data-ttu-id="37a2e-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="37a2e-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "chartseriescollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.chartseriescollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 2
}
```

##### <a name="response"></a><span data-ttu-id="37a2e-141">応答</span><span class="sxs-lookup"><span data-stu-id="37a2e-141">Response</span></span>
<span data-ttu-id="37a2e-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="37a2e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "ChartSeriesCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->