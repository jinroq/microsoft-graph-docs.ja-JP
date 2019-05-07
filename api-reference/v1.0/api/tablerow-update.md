---
title: tablerow を更新する　
description: tablerow オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 05f3df038767cee1138b26808e7a818b508bda46
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33602474"
---
# <a name="update-tablerow"></a><span data-ttu-id="e5884-103">tablerow を更新する　</span><span class="sxs-lookup"><span data-stu-id="e5884-103">Update tablerow</span></span>

<span data-ttu-id="e5884-104">tablerow オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e5884-104">Update the properties of tablerow object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e5884-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e5884-105">Permissions</span></span>
<span data-ttu-id="e5884-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e5884-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5884-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e5884-108">Permission type</span></span>      | <span data-ttu-id="e5884-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e5884-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5884-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e5884-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e5884-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5884-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e5884-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e5884-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5884-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5884-113">Not supported.</span></span>    |
|<span data-ttu-id="e5884-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e5884-114">Application</span></span> | <span data-ttu-id="e5884-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5884-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5884-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e5884-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/rows/{index}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}
```
## <a name="optional-request-headers"></a><span data-ttu-id="e5884-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e5884-117">Optional request headers</span></span>
| <span data-ttu-id="e5884-118">名前</span><span class="sxs-lookup"><span data-stu-id="e5884-118">Name</span></span>       | <span data-ttu-id="e5884-119">説明</span><span class="sxs-lookup"><span data-stu-id="e5884-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e5884-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5884-120">Authorization</span></span>  | <span data-ttu-id="e5884-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e5884-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e5884-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e5884-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e5884-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="e5884-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5884-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e5884-126">Request body</span></span>
<span data-ttu-id="e5884-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="e5884-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e5884-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5884-130">Property</span></span>     | <span data-ttu-id="e5884-131">型</span><span class="sxs-lookup"><span data-stu-id="e5884-131">Type</span></span>   |<span data-ttu-id="e5884-132">説明</span><span class="sxs-lookup"><span data-stu-id="e5884-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5884-133">values</span><span class="sxs-lookup"><span data-stu-id="e5884-133">values</span></span>|<span data-ttu-id="e5884-134">Json</span><span class="sxs-lookup"><span data-stu-id="e5884-134">Json</span></span>|<span data-ttu-id="e5884-p105">指定した範囲の Raw 値を表します。返されるデータの型は、文字列、数値、またはブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="e5884-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="e5884-138">応答</span><span class="sxs-lookup"><span data-stu-id="e5884-138">Response</span></span>

<span data-ttu-id="e5884-139">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、更新された[WorkbookTableRow](../resources/tablerow.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e5884-139">If successful, this method returns a `200 OK` response code and updated [WorkbookTableRow](../resources/tablerow.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e5884-140">例</span><span class="sxs-lookup"><span data-stu-id="e5884-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5884-141">要求</span><span class="sxs-lookup"><span data-stu-id="e5884-141">Request</span></span>
<span data-ttu-id="e5884-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e5884-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tablerow"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```
##### <a name="response"></a><span data-ttu-id="e5884-143">応答</span><span class="sxs-lookup"><span data-stu-id="e5884-143">Response</span></span>
<span data-ttu-id="e5884-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e5884-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e5884-147">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="e5884-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e5884-148">Visual</span><span class="sxs-lookup"><span data-stu-id="e5884-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_tablerow-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e5884-149">Java</span><span class="sxs-lookup"><span data-stu-id="e5884-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_tablerow-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tablerow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/tablerow-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/tablerow-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
