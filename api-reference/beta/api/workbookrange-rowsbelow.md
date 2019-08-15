---
title: 'workbookRange: rowsBelow'
description: 指定した範囲の下にある特定の行数を取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 70f76ca82da365d6780364f7c5fa4c390b5bd062
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421548"
---
# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="ee61a-103">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="ee61a-103">workbookRange: rowsBelow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee61a-104">指定した範囲の下にある特定の行数を取得します。</span><span class="sxs-lookup"><span data-stu-id="ee61a-104">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee61a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ee61a-105">Permissions</span></span>
<span data-ttu-id="ee61a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee61a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee61a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ee61a-108">Permission type</span></span>      | <span data-ttu-id="ee61a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ee61a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee61a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ee61a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ee61a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee61a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ee61a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ee61a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee61a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee61a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ee61a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ee61a-114">Application</span></span> | <span data-ttu-id="ee61a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee61a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee61a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ee61a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="ee61a-117">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="ee61a-117">Function parameters</span></span>

| <span data-ttu-id="ee61a-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ee61a-118">Parameter</span></span>    | <span data-ttu-id="ee61a-119">型</span><span class="sxs-lookup"><span data-stu-id="ee61a-119">Type</span></span>   |<span data-ttu-id="ee61a-120">説明</span><span class="sxs-lookup"><span data-stu-id="ee61a-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee61a-121">count</span><span class="sxs-lookup"><span data-stu-id="ee61a-121">count</span></span>|<span data-ttu-id="ee61a-122">Int32</span><span class="sxs-lookup"><span data-stu-id="ee61a-122">Int32</span></span>|<span data-ttu-id="ee61a-p102">省略可能。結果の範囲に含める行の数です。通常、正の数値を使用して現在の範囲外に範囲を作成します。負の数値を使用して、現在の範囲内に範囲を作成することもできます。既定値は 1 です。</span><span class="sxs-lookup"><span data-stu-id="ee61a-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="ee61a-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee61a-128">Request headers</span></span>
| <span data-ttu-id="ee61a-129">名前</span><span class="sxs-lookup"><span data-stu-id="ee61a-129">Name</span></span>       | <span data-ttu-id="ee61a-130">説明</span><span class="sxs-lookup"><span data-stu-id="ee61a-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ee61a-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee61a-131">Authorization</span></span>  | <span data-ttu-id="ee61a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ee61a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ee61a-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ee61a-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="ee61a-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="ee61a-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee61a-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="ee61a-137">Request body</span></span>
<span data-ttu-id="ee61a-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ee61a-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee61a-139">応答</span><span class="sxs-lookup"><span data-stu-id="ee61a-139">Response</span></span>

<span data-ttu-id="ee61a-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/workbookrange.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ee61a-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee61a-141">例</span><span class="sxs-lookup"><span data-stu-id="ee61a-141">Example</span></span>
<span data-ttu-id="ee61a-142">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="ee61a-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ee61a-143">要求</span><span class="sxs-lookup"><span data-stu-id="ee61a-143">Request</span></span>
<span data-ttu-id="ee61a-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ee61a-144">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ee61a-145">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ee61a-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookrange_rowsBelow"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ee61a-146">C#</span><span class="sxs-lookup"><span data-stu-id="ee61a-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-rowsbelow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ee61a-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee61a-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-rowsbelow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ee61a-148">目的-C</span><span class="sxs-lookup"><span data-stu-id="ee61a-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-rowsbelow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ee61a-149">応答</span><span class="sxs-lookup"><span data-stu-id="ee61a-149">Response</span></span>
<span data-ttu-id="ee61a-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ee61a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
