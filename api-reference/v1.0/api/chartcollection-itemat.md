---
title: 'ChartCollection: ItemAt'
description: コレクション内での位置を基にグラフを取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b1e5986871d553e9daa58b3064657d20091cc52b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580008"
---
# <a name="chartcollection-itemat"></a><span data-ttu-id="bd320-103">ChartCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="bd320-103">ChartCollection: ItemAt</span></span>

<span data-ttu-id="bd320-104">コレクション内での位置を基にグラフを取得します。</span><span class="sxs-lookup"><span data-stu-id="bd320-104">Gets a chart based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="bd320-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bd320-105">Permissions</span></span>
<span data-ttu-id="bd320-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bd320-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd320-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bd320-108">Permission type</span></span>      | <span data-ttu-id="bd320-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bd320-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd320-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bd320-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bd320-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd320-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bd320-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bd320-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd320-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd320-113">Not supported.</span></span>    |
|<span data-ttu-id="bd320-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bd320-114">Application</span></span> | <span data-ttu-id="bd320-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd320-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd320-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bd320-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="bd320-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bd320-117">Request headers</span></span>
| <span data-ttu-id="bd320-118">名前</span><span class="sxs-lookup"><span data-stu-id="bd320-118">Name</span></span>       | <span data-ttu-id="bd320-119">説明</span><span class="sxs-lookup"><span data-stu-id="bd320-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bd320-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd320-120">Authorization</span></span>  | <span data-ttu-id="bd320-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bd320-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bd320-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bd320-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="bd320-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="bd320-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd320-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="bd320-126">Request body</span></span>
<span data-ttu-id="bd320-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="bd320-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bd320-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="bd320-128">Parameter</span></span>    | <span data-ttu-id="bd320-129">型</span><span class="sxs-lookup"><span data-stu-id="bd320-129">Type</span></span>   |<span data-ttu-id="bd320-130">説明</span><span class="sxs-lookup"><span data-stu-id="bd320-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd320-131">index</span><span class="sxs-lookup"><span data-stu-id="bd320-131">index</span></span>|<span data-ttu-id="bd320-132">Int32</span><span class="sxs-lookup"><span data-stu-id="bd320-132">Int32</span></span>|<span data-ttu-id="bd320-p104">取得するオブジェクトのインデックス値。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="bd320-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="bd320-135">応答</span><span class="sxs-lookup"><span data-stu-id="bd320-135">Response</span></span>

<span data-ttu-id="bd320-136">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[WorkbookChart](../resources/chart.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bd320-136">If successful, this method returns `200 OK` response code and [WorkbookChart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd320-137">例</span><span class="sxs-lookup"><span data-stu-id="bd320-137">Example</span></span>
<span data-ttu-id="bd320-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="bd320-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bd320-139">要求</span><span class="sxs-lookup"><span data-stu-id="bd320-139">Request</span></span>
<span data-ttu-id="bd320-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bd320-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "chartcollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.chartcollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 8
}
```

##### <a name="response"></a><span data-ttu-id="bd320-141">応答</span><span class="sxs-lookup"><span data-stu-id="bd320-141">Response</span></span>
<span data-ttu-id="bd320-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bd320-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
