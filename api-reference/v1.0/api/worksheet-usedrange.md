---
title: ワークシート:UsedRange
description: 使用範囲とは、値または書式設定が割り当たっているすべてのセルを包含する最小の範囲です。ワークシートが空白の場合、この関数は左上のセルを返します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 756fccce62bab54296e5aa4ba44291ab903e24bf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36026111"
---
# <a name="worksheet-usedrange"></a><span data-ttu-id="08daf-104">ワークシート:UsedRange</span><span class="sxs-lookup"><span data-stu-id="08daf-104">Worksheet: UsedRange</span></span>

<span data-ttu-id="08daf-p102">使用範囲とは、値または書式設定が割り当たっているすべてのセルを包含する最小の範囲です。ワークシートが空白の場合、この関数は左上のセルを返します。</span><span class="sxs-lookup"><span data-stu-id="08daf-p102">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="08daf-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="08daf-107">Permissions</span></span>
<span data-ttu-id="08daf-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="08daf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08daf-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="08daf-110">Permission type</span></span>      | <span data-ttu-id="08daf-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="08daf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08daf-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="08daf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="08daf-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08daf-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="08daf-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="08daf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08daf-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08daf-115">Not supported.</span></span>    |
|<span data-ttu-id="08daf-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="08daf-116">Application</span></span> | <span data-ttu-id="08daf-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08daf-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="08daf-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="08daf-118">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="08daf-119">プロトコル</span><span class="sxs-lookup"><span data-stu-id="08daf-119">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/usedRange

```

## <a name="function-parameters"></a><span data-ttu-id="08daf-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="08daf-120">Function parameters</span></span>
<span data-ttu-id="08daf-121">要求 URL には、オプションのパラメーターを指定できます。</span><span class="sxs-lookup"><span data-stu-id="08daf-121">In the request URL you may provide optional parameters.</span></span>

| <span data-ttu-id="08daf-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="08daf-122">Parameter</span></span>    | <span data-ttu-id="08daf-123">型</span><span class="sxs-lookup"><span data-stu-id="08daf-123">Type</span></span>   |<span data-ttu-id="08daf-124">説明</span><span class="sxs-lookup"><span data-stu-id="08daf-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08daf-125">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="08daf-125">valuesOnly</span></span>|<span data-ttu-id="08daf-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="08daf-126">Boolean</span></span>|<span data-ttu-id="08daf-p104">省略可能。値の入っているセルのみを使用セルと見なします (書式設定は無視されます)。</span><span class="sxs-lookup"><span data-stu-id="08daf-p104">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="08daf-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="08daf-129">Request headers</span></span>
| <span data-ttu-id="08daf-130">名前</span><span class="sxs-lookup"><span data-stu-id="08daf-130">Name</span></span>       | <span data-ttu-id="08daf-131">説明</span><span class="sxs-lookup"><span data-stu-id="08daf-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="08daf-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="08daf-132">Authorization</span></span>  | <span data-ttu-id="08daf-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="08daf-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="08daf-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="08daf-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="08daf-p106">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="08daf-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="08daf-138">要求本文</span><span class="sxs-lookup"><span data-stu-id="08daf-138">Request body</span></span>
<span data-ttu-id="08daf-139">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="08daf-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08daf-140">応答</span><span class="sxs-lookup"><span data-stu-id="08daf-140">Response</span></span>

<span data-ttu-id="08daf-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="08daf-141">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08daf-142">例</span><span class="sxs-lookup"><span data-stu-id="08daf-142">Example</span></span>
<span data-ttu-id="08daf-143">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="08daf-143">Here is an example that shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="08daf-144">要求</span><span class="sxs-lookup"><span data-stu-id="08daf-144">Request</span></span>
<span data-ttu-id="08daf-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="08daf-145">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="08daf-146">C#</span><span class="sxs-lookup"><span data-stu-id="08daf-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="08daf-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="08daf-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="08daf-148">目的-C</span><span class="sxs-lookup"><span data-stu-id="08daf-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="08daf-149">Java</span><span class="sxs-lookup"><span data-stu-id="08daf-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-usedrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="08daf-150">応答</span><span class="sxs-lookup"><span data-stu-id="08daf-150">Response</span></span>
<span data-ttu-id="08daf-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="08daf-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="08daf-154">プロトコル</span><span class="sxs-lookup"><span data-stu-id="08daf-154">HTTP</span></span>](#tab/http)
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
  "addressLocal": "addressLocal-value"
}
```

<span data-ttu-id="08daf-155">また、この関数は、省略可能`valuesOnly`なパラメーターを指定して呼び出すこともできます。</span><span class="sxs-lookup"><span data-stu-id="08daf-155">Alternatively, this function can be called with the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="08daf-156">要求</span><span class="sxs-lookup"><span data-stu-id="08daf-156">Request</span></span>
<span data-ttu-id="08daf-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="08daf-157">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange(valuesOnly=true)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="08daf-158">C#</span><span class="sxs-lookup"><span data-stu-id="08daf-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-usedrange-valuesonly-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="08daf-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="08daf-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-usedrange-valuesonly-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="08daf-160">目的-C</span><span class="sxs-lookup"><span data-stu-id="08daf-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-usedrange-valuesonly-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="08daf-161">Java</span><span class="sxs-lookup"><span data-stu-id="08daf-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-usedrange-valuesonly-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="08daf-162">応答</span><span class="sxs-lookup"><span data-stu-id="08daf-162">Response</span></span>
<span data-ttu-id="08daf-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="08daf-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "addressLocal": "addressLocal-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
