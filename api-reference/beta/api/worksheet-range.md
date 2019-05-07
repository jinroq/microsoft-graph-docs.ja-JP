---
title: ワークシート:Range
description: アドレスまたは名前で指定された範囲オブジェクトを取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: bd28e251732d58fa6a65d4e79dce814543603380
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636836"
---
# <a name="worksheet-range"></a><span data-ttu-id="34c3f-103">ワークシート:Range</span><span class="sxs-lookup"><span data-stu-id="34c3f-103">Worksheet: Range</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34c3f-104">アドレスまたは名前で指定された範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="34c3f-104">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="34c3f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="34c3f-105">Permissions</span></span>
<span data-ttu-id="34c3f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="34c3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34c3f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="34c3f-108">Permission type</span></span>      | <span data-ttu-id="34c3f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="34c3f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34c3f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="34c3f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="34c3f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34c3f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="34c3f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="34c3f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34c3f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34c3f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="34c3f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="34c3f-114">Application</span></span> | <span data-ttu-id="34c3f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34c3f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="34c3f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="34c3f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="34c3f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="34c3f-117">Request headers</span></span>
| <span data-ttu-id="34c3f-118">名前</span><span class="sxs-lookup"><span data-stu-id="34c3f-118">Name</span></span>       | <span data-ttu-id="34c3f-119">説明</span><span class="sxs-lookup"><span data-stu-id="34c3f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="34c3f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="34c3f-120">Authorization</span></span>  | <span data-ttu-id="34c3f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="34c3f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="34c3f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="34c3f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="34c3f-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="34c3f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="34c3f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="34c3f-126">Request body</span></span>
<span data-ttu-id="34c3f-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="34c3f-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="34c3f-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="34c3f-128">Parameter</span></span>    | <span data-ttu-id="34c3f-129">型</span><span class="sxs-lookup"><span data-stu-id="34c3f-129">Type</span></span>   |<span data-ttu-id="34c3f-130">説明</span><span class="sxs-lookup"><span data-stu-id="34c3f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34c3f-131">address</span><span class="sxs-lookup"><span data-stu-id="34c3f-131">address</span></span>|<span data-ttu-id="34c3f-132">string</span><span class="sxs-lookup"><span data-stu-id="34c3f-132">string</span></span>|<span data-ttu-id="34c3f-p104">省略可能。範囲のアドレスまたは名前。指定されていない場合は、ワークシート全体の範囲が返されます。</span><span class="sxs-lookup"><span data-stu-id="34c3f-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="34c3f-136">応答</span><span class="sxs-lookup"><span data-stu-id="34c3f-136">Response</span></span>

<span data-ttu-id="34c3f-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/workbookrange.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="34c3f-137">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34c3f-138">例</span><span class="sxs-lookup"><span data-stu-id="34c3f-138">Example</span></span>
<span data-ttu-id="34c3f-139">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="34c3f-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="34c3f-140">要求</span><span class="sxs-lookup"><span data-stu-id="34c3f-140">Request</span></span>
<span data-ttu-id="34c3f-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="34c3f-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/Range
Content-type: application/json
Content-length: 32

{
  "address": "address-value"
}
```

##### <a name="response"></a><span data-ttu-id="34c3f-142">応答</span><span class="sxs-lookup"><span data-stu-id="34c3f-142">Response</span></span>
<span data-ttu-id="34c3f-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="34c3f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="34c3f-146">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="34c3f-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="34c3f-147">Visual</span><span class="sxs-lookup"><span data-stu-id="34c3f-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/worksheet_range-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="34c3f-148">Java</span><span class="sxs-lookup"><span data-stu-id="34c3f-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/worksheet_range-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheet-range.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/worksheet-range.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
