---
title: 'ChartFill: setSolidColor'
description: グラフ要素の塗りつぶしの書式設定を均一な色に設定します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e5c0a120becc53b6b7d06fdc1e5c43130b5a414b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975919"
---
# <a name="chartfill-setsolidcolor"></a><span data-ttu-id="f03f4-103">ChartFill: setSolidColor</span><span class="sxs-lookup"><span data-stu-id="f03f4-103">ChartFill: setSolidColor</span></span>

> <span data-ttu-id="f03f4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f03f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f03f4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f03f4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f03f4-106">グラフ要素の塗りつぶしの書式設定を均一な色に設定します。</span><span class="sxs-lookup"><span data-stu-id="f03f4-106">Sets the fill formatting of a chart element to a uniform color.</span></span>
## <a name="permissions"></a><span data-ttu-id="f03f4-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f03f4-107">Permissions</span></span>
<span data-ttu-id="f03f4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f03f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f03f4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f03f4-110">Permission type</span></span>      | <span data-ttu-id="f03f4-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f03f4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f03f4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f03f4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f03f4-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f03f4-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f03f4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f03f4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f03f4-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f03f4-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f03f4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f03f4-116">Application</span></span> | <span data-ttu-id="f03f4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f03f4-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f03f4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f03f4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts(<name>)/title/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts(<name>)/legend/format/fill/setSolidColor

```
## <a name="request-headers"></a><span data-ttu-id="f03f4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f03f4-119">Request headers</span></span>
| <span data-ttu-id="f03f4-120">名前</span><span class="sxs-lookup"><span data-stu-id="f03f4-120">Name</span></span>       | <span data-ttu-id="f03f4-121">説明</span><span class="sxs-lookup"><span data-stu-id="f03f4-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f03f4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f03f4-122">Authorization</span></span>  | <span data-ttu-id="f03f4-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f03f4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f03f4-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f03f4-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f03f4-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="f03f4-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f03f4-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="f03f4-128">Request body</span></span>
<span data-ttu-id="f03f4-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="f03f4-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f03f4-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f03f4-130">Parameter</span></span>    | <span data-ttu-id="f03f4-131">Type</span><span class="sxs-lookup"><span data-stu-id="f03f4-131">Type</span></span>   |<span data-ttu-id="f03f4-132">説明</span><span class="sxs-lookup"><span data-stu-id="f03f4-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f03f4-133">color</span><span class="sxs-lookup"><span data-stu-id="f03f4-133">color</span></span>|<span data-ttu-id="f03f4-134">文字列</span><span class="sxs-lookup"><span data-stu-id="f03f4-134">string</span></span>|<span data-ttu-id="f03f4-135">枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ") です。</span><span class="sxs-lookup"><span data-stu-id="f03f4-135">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|

## <a name="response"></a><span data-ttu-id="f03f4-136">応答</span><span class="sxs-lookup"><span data-stu-id="f03f4-136">Response</span></span>

<span data-ttu-id="f03f4-p105">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f03f4-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f03f4-139">例</span><span class="sxs-lookup"><span data-stu-id="f03f4-139">Example</span></span>
<span data-ttu-id="f03f4-140">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="f03f4-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f03f4-141">要求</span><span class="sxs-lookup"><span data-stu-id="f03f4-141">Request</span></span>
<span data-ttu-id="f03f4-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f03f4-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartfill_setsolidcolor"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/format/fill/setSolidColor
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

##### <a name="response"></a><span data-ttu-id="f03f4-143">応答</span><span class="sxs-lookup"><span data-stu-id="f03f4-143">Response</span></span>
<span data-ttu-id="f03f4-144">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f03f4-144">Here is an example of the response.</span></span> 
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
  "description": "ChartFill: setSolidColor",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
