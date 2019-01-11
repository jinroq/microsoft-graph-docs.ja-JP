---
title: 範囲:LastColumn
description: .
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 9ed7a58c744e316266c755f94670a3277ecd747a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885163"
---
# <a name="range-lastcolumn"></a><span data-ttu-id="00ac3-103">範囲:LastColumn</span><span class="sxs-lookup"><span data-stu-id="00ac3-103">Range: LastColumn</span></span>

<span data-ttu-id="00ac3-p101">範囲内の最後の列を取得します。たとえば、"B2:D5" の最後の列は "D2:D5" になります。</span><span class="sxs-lookup"><span data-stu-id="00ac3-p101">Gets the last column within the range. For example, the last column of "B2:D5" is "D2:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="00ac3-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="00ac3-106">Permissions</span></span>
<span data-ttu-id="00ac3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="00ac3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00ac3-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="00ac3-109">Permission type</span></span>      | <span data-ttu-id="00ac3-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="00ac3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00ac3-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="00ac3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="00ac3-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00ac3-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="00ac3-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="00ac3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00ac3-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00ac3-114">Not supported.</span></span>    |
|<span data-ttu-id="00ac3-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="00ac3-115">Application</span></span> | <span data-ttu-id="00ac3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00ac3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="00ac3-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="00ac3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/lastColumn
GET /workbook/worksheets/{id|name}/range(address='<address>')/lastColumn
GET /workbook/tables/{id|name}/columns/{id|name}/range/lastColumn

```
## <a name="request-headers"></a><span data-ttu-id="00ac3-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="00ac3-118">Request headers</span></span>
| <span data-ttu-id="00ac3-119">名前</span><span class="sxs-lookup"><span data-stu-id="00ac3-119">Name</span></span>       | <span data-ttu-id="00ac3-120">説明</span><span class="sxs-lookup"><span data-stu-id="00ac3-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="00ac3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="00ac3-121">Authorization</span></span>  | <span data-ttu-id="00ac3-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="00ac3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="00ac3-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="00ac3-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="00ac3-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="00ac3-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="00ac3-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="00ac3-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="00ac3-128">応答</span><span class="sxs-lookup"><span data-stu-id="00ac3-128">Response</span></span>

<span data-ttu-id="00ac3-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="00ac3-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00ac3-130">例</span><span class="sxs-lookup"><span data-stu-id="00ac3-130">Example</span></span>
<span data-ttu-id="00ac3-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="00ac3-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="00ac3-132">要求</span><span class="sxs-lookup"><span data-stu-id="00ac3-132">Request</span></span>
<span data-ttu-id="00ac3-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="00ac3-133">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_lastcolumn"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/lastColumn
```

##### <a name="response"></a><span data-ttu-id="00ac3-134">応答</span><span class="sxs-lookup"><span data-stu-id="00ac3-134">Response</span></span>
<span data-ttu-id="00ac3-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="00ac3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: LastColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
