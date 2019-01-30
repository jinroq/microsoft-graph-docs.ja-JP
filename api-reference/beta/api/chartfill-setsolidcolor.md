---
title: 'ChartFill: setSolidColor'
description: グラフ要素の塗りつぶしの書式設定を均一な色に設定します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e841ee13719b7d19f1ca306ad3a555b447cb9cb6
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642332"
---
# <a name="chartfill-setsolidcolor"></a><span data-ttu-id="c6090-103">ChartFill: setSolidColor</span><span class="sxs-lookup"><span data-stu-id="c6090-103">ChartFill: setSolidColor</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6090-104">グラフ要素の塗りつぶしの書式設定を均一な色に設定します。</span><span class="sxs-lookup"><span data-stu-id="c6090-104">Sets the fill formatting of a chart element to a uniform color.</span></span>
## <a name="permissions"></a><span data-ttu-id="c6090-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c6090-105">Permissions</span></span>
<span data-ttu-id="c6090-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c6090-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6090-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c6090-108">Permission type</span></span>      | <span data-ttu-id="c6090-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c6090-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6090-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c6090-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c6090-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6090-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c6090-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c6090-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6090-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6090-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c6090-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c6090-114">Application</span></span> | <span data-ttu-id="c6090-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c6090-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6090-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c6090-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts(<name>)/title/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts(<name>)/legend/format/fill/setSolidColor

```
## <a name="request-headers"></a><span data-ttu-id="c6090-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c6090-117">Request headers</span></span>
| <span data-ttu-id="c6090-118">名前</span><span class="sxs-lookup"><span data-stu-id="c6090-118">Name</span></span>       | <span data-ttu-id="c6090-119">説明</span><span class="sxs-lookup"><span data-stu-id="c6090-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c6090-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6090-120">Authorization</span></span>  | <span data-ttu-id="c6090-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c6090-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c6090-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c6090-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c6090-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="c6090-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6090-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c6090-126">Request body</span></span>
<span data-ttu-id="c6090-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="c6090-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c6090-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c6090-128">Parameter</span></span>    | <span data-ttu-id="c6090-129">型</span><span class="sxs-lookup"><span data-stu-id="c6090-129">Type</span></span>   |<span data-ttu-id="c6090-130">説明</span><span class="sxs-lookup"><span data-stu-id="c6090-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6090-131">color</span><span class="sxs-lookup"><span data-stu-id="c6090-131">color</span></span>|<span data-ttu-id="c6090-132">文字列</span><span class="sxs-lookup"><span data-stu-id="c6090-132">string</span></span>|<span data-ttu-id="c6090-133">枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ") です。</span><span class="sxs-lookup"><span data-stu-id="c6090-133">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|

## <a name="response"></a><span data-ttu-id="c6090-134">応答</span><span class="sxs-lookup"><span data-stu-id="c6090-134">Response</span></span>

<span data-ttu-id="c6090-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="c6090-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6090-137">例</span><span class="sxs-lookup"><span data-stu-id="c6090-137">Example</span></span>
<span data-ttu-id="c6090-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="c6090-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c6090-139">要求</span><span class="sxs-lookup"><span data-stu-id="c6090-139">Request</span></span>
<span data-ttu-id="c6090-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c6090-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c6090-141">応答</span><span class="sxs-lookup"><span data-stu-id="c6090-141">Response</span></span>
<span data-ttu-id="c6090-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c6090-142">Here is an example of the response.</span></span> 
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
  "description": "ChartFill: setSolidColor",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartfill-setsolidcolor.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
