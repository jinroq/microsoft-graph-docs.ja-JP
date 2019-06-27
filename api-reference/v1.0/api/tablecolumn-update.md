---
title: tablecolumn を更新する
description: tablecolumn オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: dd7b663847d121ce84359b0253a4bfcdc18a2817
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278821"
---
# <a name="update-tablecolumn"></a><span data-ttu-id="638ac-103">tablecolumn を更新する</span><span class="sxs-lookup"><span data-stu-id="638ac-103">Update tablecolumn</span></span>

<span data-ttu-id="638ac-104">tablecolumn オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="638ac-104">Update the properties of tablecolumn object.</span></span>
## <a name="permissions"></a><span data-ttu-id="638ac-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="638ac-105">Permissions</span></span>
<span data-ttu-id="638ac-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="638ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="638ac-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="638ac-108">Permission type</span></span>      | <span data-ttu-id="638ac-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="638ac-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="638ac-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="638ac-110">Delegated (work or school account)</span></span> | <span data-ttu-id="638ac-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="638ac-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="638ac-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="638ac-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="638ac-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="638ac-113">Not supported.</span></span>    |
|<span data-ttu-id="638ac-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="638ac-114">Application</span></span> | <span data-ttu-id="638ac-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="638ac-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="638ac-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="638ac-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/columns/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="638ac-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="638ac-117">Optional request headers</span></span>
| <span data-ttu-id="638ac-118">名前</span><span class="sxs-lookup"><span data-stu-id="638ac-118">Name</span></span>       | <span data-ttu-id="638ac-119">説明</span><span class="sxs-lookup"><span data-stu-id="638ac-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="638ac-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="638ac-120">Authorization</span></span>  | <span data-ttu-id="638ac-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="638ac-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="638ac-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="638ac-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="638ac-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="638ac-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="638ac-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="638ac-126">Request body</span></span>
<span data-ttu-id="638ac-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="638ac-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="638ac-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="638ac-130">Property</span></span>     | <span data-ttu-id="638ac-131">型</span><span class="sxs-lookup"><span data-stu-id="638ac-131">Type</span></span>   |<span data-ttu-id="638ac-132">説明</span><span class="sxs-lookup"><span data-stu-id="638ac-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="638ac-133">values</span><span class="sxs-lookup"><span data-stu-id="638ac-133">values</span></span>|<span data-ttu-id="638ac-134">Json</span><span class="sxs-lookup"><span data-stu-id="638ac-134">Json</span></span>|<span data-ttu-id="638ac-p105">指定した範囲の Raw 値を表します。返されるデータの型は、文字列、数値、またはブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="638ac-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="638ac-138">応答</span><span class="sxs-lookup"><span data-stu-id="638ac-138">Response</span></span>

<span data-ttu-id="638ac-139">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、更新された[WorkbookTableColumn](../resources/tablecolumn.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="638ac-139">If successful, this method returns a `200 OK` response code and updated [WorkbookTableColumn](../resources/tablecolumn.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="638ac-140">例</span><span class="sxs-lookup"><span data-stu-id="638ac-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="638ac-141">要求</span><span class="sxs-lookup"><span data-stu-id="638ac-141">Request</span></span>
<span data-ttu-id="638ac-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="638ac-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tablecolumn"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
Content-type: application/json
Content-length: 81

{
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
##### <a name="response"></a><span data-ttu-id="638ac-143">応答</span><span class="sxs-lookup"><span data-stu-id="638ac-143">Response</span></span>
<span data-ttu-id="638ac-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="638ac-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="638ac-147">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="638ac-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="638ac-148">C#</span><span class="sxs-lookup"><span data-stu-id="638ac-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_tablecolumn-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="638ac-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="638ac-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_tablecolumn-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="638ac-150">目的-C</span><span class="sxs-lookup"><span data-stu-id="638ac-150">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_tablecolumn-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tablecolumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/tablecolumn-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/tablecolumn-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/tablecolumn-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
