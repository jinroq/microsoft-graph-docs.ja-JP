---
title: ワークシート:Range
description: アドレスまたは名前で指定された範囲オブジェクトを取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ec627bcdf1415fd022a25a4234371d2c5b9c6a6a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456436"
---
# <a name="worksheet-range"></a><span data-ttu-id="29c6c-103">ワークシート:Range</span><span class="sxs-lookup"><span data-stu-id="29c6c-103">Worksheet: Range</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29c6c-104">アドレスまたは名前で指定された範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="29c6c-104">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="29c6c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="29c6c-105">Permissions</span></span>
<span data-ttu-id="29c6c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="29c6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29c6c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="29c6c-108">Permission type</span></span>      | <span data-ttu-id="29c6c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="29c6c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29c6c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="29c6c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="29c6c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="29c6c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="29c6c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="29c6c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29c6c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="29c6c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="29c6c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="29c6c-114">Application</span></span> | <span data-ttu-id="29c6c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29c6c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="29c6c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="29c6c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="29c6c-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="29c6c-117">Request headers</span></span>
| <span data-ttu-id="29c6c-118">名前</span><span class="sxs-lookup"><span data-stu-id="29c6c-118">Name</span></span>       | <span data-ttu-id="29c6c-119">説明</span><span class="sxs-lookup"><span data-stu-id="29c6c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="29c6c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="29c6c-120">Authorization</span></span>  | <span data-ttu-id="29c6c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="29c6c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="29c6c-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="29c6c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="29c6c-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="29c6c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="29c6c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="29c6c-126">Request body</span></span>
<span data-ttu-id="29c6c-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="29c6c-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="29c6c-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="29c6c-128">Parameter</span></span>    | <span data-ttu-id="29c6c-129">型</span><span class="sxs-lookup"><span data-stu-id="29c6c-129">Type</span></span>   |<span data-ttu-id="29c6c-130">説明</span><span class="sxs-lookup"><span data-stu-id="29c6c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29c6c-131">address</span><span class="sxs-lookup"><span data-stu-id="29c6c-131">address</span></span>|<span data-ttu-id="29c6c-132">string</span><span class="sxs-lookup"><span data-stu-id="29c6c-132">string</span></span>|<span data-ttu-id="29c6c-p104">省略可能。範囲のアドレスまたは名前。指定されていない場合は、ワークシート全体の範囲が返されます。</span><span class="sxs-lookup"><span data-stu-id="29c6c-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="29c6c-136">応答</span><span class="sxs-lookup"><span data-stu-id="29c6c-136">Response</span></span>

<span data-ttu-id="29c6c-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/workbookrange.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="29c6c-137">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29c6c-138">例</span><span class="sxs-lookup"><span data-stu-id="29c6c-138">Example</span></span>
<span data-ttu-id="29c6c-139">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="29c6c-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="29c6c-140">要求</span><span class="sxs-lookup"><span data-stu-id="29c6c-140">Request</span></span>
<span data-ttu-id="29c6c-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="29c6c-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="29c6c-142">プロトコル</span><span class="sxs-lookup"><span data-stu-id="29c6c-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="29c6c-143">C#</span><span class="sxs-lookup"><span data-stu-id="29c6c-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="29c6c-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="29c6c-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="29c6c-145">目的-C</span><span class="sxs-lookup"><span data-stu-id="29c6c-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="29c6c-146">応答</span><span class="sxs-lookup"><span data-stu-id="29c6c-146">Response</span></span>
<span data-ttu-id="29c6c-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="29c6c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
