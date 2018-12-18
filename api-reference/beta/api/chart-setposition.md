---
title: 'Chart: setPosition'
description: ワークシート上のセルを基準にしてグラフを配置します。
author: lumine2008
ms.openlocfilehash: 8d5a5f2b599d9d3b3902c8bbb5feec2d8178a6e6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314925"
---
# <a name="chart-setposition"></a><span data-ttu-id="6cff3-103">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="6cff3-103">Chart: setPosition</span></span>

> <span data-ttu-id="6cff3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6cff3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6cff3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6cff3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6cff3-106">ワークシート上のセルを基準にしてグラフを配置します。</span><span class="sxs-lookup"><span data-stu-id="6cff3-106">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="6cff3-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6cff3-107">Permissions</span></span>
<span data-ttu-id="6cff3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6cff3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cff3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6cff3-110">Permission type</span></span>      | <span data-ttu-id="6cff3-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6cff3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6cff3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6cff3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6cff3-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6cff3-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6cff3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6cff3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cff3-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6cff3-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6cff3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6cff3-116">Application</span></span> | <span data-ttu-id="6cff3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6cff3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6cff3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6cff3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="6cff3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6cff3-119">Request headers</span></span>
| <span data-ttu-id="6cff3-120">名前</span><span class="sxs-lookup"><span data-stu-id="6cff3-120">Name</span></span>       | <span data-ttu-id="6cff3-121">説明</span><span class="sxs-lookup"><span data-stu-id="6cff3-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6cff3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cff3-122">Authorization</span></span>  | <span data-ttu-id="6cff3-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6cff3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6cff3-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6cff3-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="6cff3-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="6cff3-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cff3-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="6cff3-128">Request body</span></span>
<span data-ttu-id="6cff3-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="6cff3-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6cff3-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="6cff3-130">Parameter</span></span>    | <span data-ttu-id="6cff3-131">種類</span><span class="sxs-lookup"><span data-stu-id="6cff3-131">Type</span></span>   |<span data-ttu-id="6cff3-132">説明</span><span class="sxs-lookup"><span data-stu-id="6cff3-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6cff3-133">startCell</span><span class="sxs-lookup"><span data-stu-id="6cff3-133">startCell</span></span>|<span data-ttu-id="6cff3-134">string</span><span class="sxs-lookup"><span data-stu-id="6cff3-134">string</span></span>|<span data-ttu-id="6cff3-p105">開始セル。これは、グラフの移動先です。開始セルは、ユーザーの右から左への表示の設定に応じて、左上のセルか、右上のセルとなります。</span><span class="sxs-lookup"><span data-stu-id="6cff3-p105">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="6cff3-138">endCell</span><span class="sxs-lookup"><span data-stu-id="6cff3-138">endCell</span></span>|<span data-ttu-id="6cff3-139">string</span><span class="sxs-lookup"><span data-stu-id="6cff3-139">string</span></span>|<span data-ttu-id="6cff3-p106">省略可能。終了セル。指定されている場合、グラフの幅と高さは、このセルまたは範囲を完全にカバーするように設定されます。</span><span class="sxs-lookup"><span data-stu-id="6cff3-p106">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="6cff3-143">応答</span><span class="sxs-lookup"><span data-stu-id="6cff3-143">Response</span></span>

<span data-ttu-id="6cff3-p107">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="6cff3-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cff3-146">例</span><span class="sxs-lookup"><span data-stu-id="6cff3-146">Example</span></span>
<span data-ttu-id="6cff3-147">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="6cff3-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6cff3-148">要求</span><span class="sxs-lookup"><span data-stu-id="6cff3-148">Request</span></span>
<span data-ttu-id="6cff3-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6cff3-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setposition"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/setPosition
Content-type: application/json
Content-length: 66

{
  "startCell": "startCell-value",
  "endCell": "endCell-value"
}
```

##### <a name="response"></a><span data-ttu-id="6cff3-150">応答</span><span class="sxs-lookup"><span data-stu-id="6cff3-150">Response</span></span>
<span data-ttu-id="6cff3-151">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6cff3-151">Here is an example of the response.</span></span> 
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
  "description": "Chart: setPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->