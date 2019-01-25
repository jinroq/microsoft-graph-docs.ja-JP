---
title: 範囲:LastRow
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8f6ed391f1158b6b9253827c52c50a0b197e31a5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510254"
---
# <a name="range-lastrow"></a><span data-ttu-id="c7e83-103">範囲:LastRow</span><span class="sxs-lookup"><span data-stu-id="c7e83-103">Range: LastRow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7e83-p101">範囲内の最後の行を取得します。たとえば、"B2:D5" の最後の行は "B5:D5" になります。</span><span class="sxs-lookup"><span data-stu-id="c7e83-p101">Gets the last row within the range. For example, the last row of "B2:D5" is "B5:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="c7e83-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c7e83-106">Permissions</span></span>
<span data-ttu-id="c7e83-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c7e83-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7e83-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c7e83-109">Permission type</span></span>      | <span data-ttu-id="c7e83-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c7e83-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7e83-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c7e83-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c7e83-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7e83-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c7e83-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c7e83-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7e83-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7e83-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c7e83-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c7e83-115">Application</span></span> | <span data-ttu-id="c7e83-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7e83-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7e83-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c7e83-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/LastRow
GET /workbook/worksheets/{id|name}/range(address='<address>')/LastRow
GET /workbook/tables/{id|name}/columns/{id|name}/range/LastRow

```
## <a name="request-headers"></a><span data-ttu-id="c7e83-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c7e83-118">Request headers</span></span>
| <span data-ttu-id="c7e83-119">名前</span><span class="sxs-lookup"><span data-stu-id="c7e83-119">Name</span></span>       | <span data-ttu-id="c7e83-120">説明</span><span class="sxs-lookup"><span data-stu-id="c7e83-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c7e83-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7e83-121">Authorization</span></span>  | <span data-ttu-id="c7e83-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c7e83-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c7e83-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c7e83-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="c7e83-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="c7e83-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7e83-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c7e83-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c7e83-128">応答</span><span class="sxs-lookup"><span data-stu-id="c7e83-128">Response</span></span>

<span data-ttu-id="c7e83-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c7e83-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7e83-130">例</span><span class="sxs-lookup"><span data-stu-id="c7e83-130">Example</span></span>
<span data-ttu-id="c7e83-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="c7e83-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c7e83-132">要求</span><span class="sxs-lookup"><span data-stu-id="c7e83-132">Request</span></span>
<span data-ttu-id="c7e83-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c7e83-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_lastrow"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/LastRow
```

##### <a name="response"></a><span data-ttu-id="c7e83-134">応答</span><span class="sxs-lookup"><span data-stu-id="c7e83-134">Response</span></span>
<span data-ttu-id="c7e83-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c7e83-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
<!--
{
  "type": "#page.annotation",
  "description": "Range: LastRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-lastrow.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
