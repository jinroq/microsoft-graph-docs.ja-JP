---
title: 範囲:EntireRow
description: 範囲に含まれるすべての行を表すオブジェクトを取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: db5c59cd30f9687e60d4be6977b44672cc57dce0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521524"
---
# <a name="range-entirerow"></a><span data-ttu-id="ea109-103">範囲:EntireRow</span><span class="sxs-lookup"><span data-stu-id="ea109-103">Range: EntireRow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea109-104">範囲に含まれるすべての行を表すオブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="ea109-104">Gets an object that represents the entire row of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="ea109-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ea109-105">Permissions</span></span>
<span data-ttu-id="ea109-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ea109-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea109-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ea109-108">Permission type</span></span>      | <span data-ttu-id="ea109-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ea109-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea109-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ea109-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ea109-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea109-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ea109-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ea109-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea109-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea109-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ea109-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ea109-114">Application</span></span> | <span data-ttu-id="ea109-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ea109-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea109-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ea109-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/EntireRow
GET /workbook/worksheets/{id|name}/range(address='<address>')/EntireRow
GET /workbook/tables/{id|name}/columns/{id|name}/range/EntireRow

```
## <a name="request-headers"></a><span data-ttu-id="ea109-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ea109-117">Request headers</span></span>
| <span data-ttu-id="ea109-118">名前</span><span class="sxs-lookup"><span data-stu-id="ea109-118">Name</span></span>       | <span data-ttu-id="ea109-119">説明</span><span class="sxs-lookup"><span data-stu-id="ea109-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ea109-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea109-120">Authorization</span></span>  | <span data-ttu-id="ea109-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ea109-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ea109-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ea109-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="ea109-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="ea109-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea109-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ea109-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ea109-127">応答</span><span class="sxs-lookup"><span data-stu-id="ea109-127">Response</span></span>

<span data-ttu-id="ea109-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ea109-128">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea109-129">例</span><span class="sxs-lookup"><span data-stu-id="ea109-129">Example</span></span>
<span data-ttu-id="ea109-130">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="ea109-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ea109-131">要求</span><span class="sxs-lookup"><span data-stu-id="ea109-131">Request</span></span>
<span data-ttu-id="ea109-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ea109-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_entirerow"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/EntireRow
```

##### <a name="response"></a><span data-ttu-id="ea109-133">応答</span><span class="sxs-lookup"><span data-stu-id="ea109-133">Response</span></span>
<span data-ttu-id="ea109-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ea109-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: EntireRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-entirerow.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
