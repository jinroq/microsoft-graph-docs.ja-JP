---
title: 'ChartPointsCollection: ItemAt'
description: データ系列内の位置に基づくポイントを取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c5ba2e5e0a65aa6c05771b084ed395a016622206
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943765"
---
# <a name="chartpointscollection-itemat"></a><span data-ttu-id="40c21-103">ChartPointsCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="40c21-103">ChartPointsCollection: ItemAt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40c21-104">データ系列内の位置に基づくポイントを取得します。</span><span class="sxs-lookup"><span data-stu-id="40c21-104">Retrieve a point based on its position within the series.</span></span>
## <a name="permissions"></a><span data-ttu-id="40c21-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="40c21-105">Permissions</span></span>
<span data-ttu-id="40c21-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="40c21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40c21-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="40c21-108">Permission type</span></span>      | <span data-ttu-id="40c21-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="40c21-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40c21-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="40c21-110">Delegated (work or school account)</span></span> | <span data-ttu-id="40c21-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40c21-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="40c21-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="40c21-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40c21-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40c21-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="40c21-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="40c21-114">Application</span></span> | <span data-ttu-id="40c21-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40c21-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="40c21-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="40c21-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="40c21-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40c21-117">Request headers</span></span>
| <span data-ttu-id="40c21-118">名前</span><span class="sxs-lookup"><span data-stu-id="40c21-118">Name</span></span>       | <span data-ttu-id="40c21-119">説明</span><span class="sxs-lookup"><span data-stu-id="40c21-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="40c21-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="40c21-120">Authorization</span></span>  | <span data-ttu-id="40c21-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="40c21-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="40c21-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="40c21-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="40c21-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="40c21-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="40c21-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="40c21-126">Request body</span></span>
<span data-ttu-id="40c21-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="40c21-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="40c21-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="40c21-128">Parameter</span></span>    | <span data-ttu-id="40c21-129">型</span><span class="sxs-lookup"><span data-stu-id="40c21-129">Type</span></span>   |<span data-ttu-id="40c21-130">説明</span><span class="sxs-lookup"><span data-stu-id="40c21-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40c21-131">index</span><span class="sxs-lookup"><span data-stu-id="40c21-131">index</span></span>|<span data-ttu-id="40c21-132">number</span><span class="sxs-lookup"><span data-stu-id="40c21-132">number</span></span>|<span data-ttu-id="40c21-p104">取得するオブジェクトのインデックス値。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="40c21-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="40c21-135">応答</span><span class="sxs-lookup"><span data-stu-id="40c21-135">Response</span></span>

<span data-ttu-id="40c21-136">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[workbookChartPoint](../resources/workbookchartpoint.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="40c21-136">If successful, this method returns `200 OK` response code and [workbookChartPoint](../resources/workbookchartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40c21-137">例</span><span class="sxs-lookup"><span data-stu-id="40c21-137">Example</span></span>
<span data-ttu-id="40c21-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="40c21-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="40c21-139">要求</span><span class="sxs-lookup"><span data-stu-id="40c21-139">Request</span></span>
<span data-ttu-id="40c21-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="40c21-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="40c21-141">プロトコル</span><span class="sxs-lookup"><span data-stu-id="40c21-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartpointscollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="40c21-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="40c21-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartpointscollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="40c21-143">応答</span><span class="sxs-lookup"><span data-stu-id="40c21-143">Response</span></span>
<span data-ttu-id="40c21-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="40c21-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartPoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 20

{
  "value": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartPointsCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
