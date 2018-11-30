---
title: 'ChartFill: setSolidColor'
description: グラフ要素の塗りつぶしの書式設定を均一な色に設定します。
ms.openlocfilehash: bcb8397217ee6cc574fe08f585d51a6243d83ca9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020793"
---
# <a name="chartfill-setsolidcolor"></a><span data-ttu-id="074ae-103">ChartFill: setSolidColor</span><span class="sxs-lookup"><span data-stu-id="074ae-103">ChartFill: setSolidColor</span></span>

<span data-ttu-id="074ae-104">グラフ要素の塗りつぶしの書式設定を均一な色に設定します。</span><span class="sxs-lookup"><span data-stu-id="074ae-104">Sets the fill formatting of a chart element to a uniform color.</span></span>
## <a name="permissions"></a><span data-ttu-id="074ae-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="074ae-105">Permissions</span></span>
<span data-ttu-id="074ae-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="074ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="074ae-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="074ae-108">Permission type</span></span>      | <span data-ttu-id="074ae-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="074ae-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="074ae-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="074ae-110">Delegated (work or school account)</span></span> | <span data-ttu-id="074ae-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="074ae-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="074ae-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="074ae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="074ae-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="074ae-113">Not supported.</span></span>    |
|<span data-ttu-id="074ae-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="074ae-114">Application</span></span> | <span data-ttu-id="074ae-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="074ae-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="074ae-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="074ae-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts/{name}/title/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/setSolidColor

```
## <a name="request-headers"></a><span data-ttu-id="074ae-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="074ae-117">Request headers</span></span>
| <span data-ttu-id="074ae-118">名前</span><span class="sxs-lookup"><span data-stu-id="074ae-118">Name</span></span>       | <span data-ttu-id="074ae-119">説明</span><span class="sxs-lookup"><span data-stu-id="074ae-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="074ae-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="074ae-120">Authorization</span></span>  | <span data-ttu-id="074ae-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="074ae-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="074ae-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="074ae-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="074ae-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="074ae-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="074ae-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="074ae-126">Request body</span></span>
<span data-ttu-id="074ae-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="074ae-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="074ae-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="074ae-128">Parameter</span></span>    | <span data-ttu-id="074ae-129">型</span><span class="sxs-lookup"><span data-stu-id="074ae-129">Type</span></span>   |<span data-ttu-id="074ae-130">説明</span><span class="sxs-lookup"><span data-stu-id="074ae-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="074ae-131">color</span><span class="sxs-lookup"><span data-stu-id="074ae-131">color</span></span>|<span data-ttu-id="074ae-132">文字列</span><span class="sxs-lookup"><span data-stu-id="074ae-132">string</span></span>|<span data-ttu-id="074ae-133">枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ") です。</span><span class="sxs-lookup"><span data-stu-id="074ae-133">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|

## <a name="response"></a><span data-ttu-id="074ae-134">応答</span><span class="sxs-lookup"><span data-stu-id="074ae-134">Response</span></span>

<span data-ttu-id="074ae-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="074ae-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="074ae-137">例</span><span class="sxs-lookup"><span data-stu-id="074ae-137">Example</span></span>
<span data-ttu-id="074ae-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="074ae-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="074ae-139">要求</span><span class="sxs-lookup"><span data-stu-id="074ae-139">Request</span></span>
<span data-ttu-id="074ae-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="074ae-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartfill_setsolidcolor"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

##### <a name="response"></a><span data-ttu-id="074ae-141">応答</span><span class="sxs-lookup"><span data-stu-id="074ae-141">Response</span></span>
<span data-ttu-id="074ae-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="074ae-142">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartFill: setSolidColor",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->