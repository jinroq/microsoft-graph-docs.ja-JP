---
title: 'workbookRange: columnsBefore'
description: 指定した範囲の左にある特定の列数を取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 136fc09801864abacd2eb7d5e1a4225e69b2418e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987335"
---
# <a name="workbookrange-columnsbefore"></a><span data-ttu-id="98aa4-103">workbookRange: columnsBefore</span><span class="sxs-lookup"><span data-stu-id="98aa4-103">workbookRange: columnsBefore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98aa4-104">指定した範囲の左にある特定の列数を取得します。</span><span class="sxs-lookup"><span data-stu-id="98aa4-104">Gets a certain number of columns to the left of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="98aa4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="98aa4-105">Permissions</span></span>
<span data-ttu-id="98aa4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="98aa4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98aa4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="98aa4-108">Permission type</span></span>      | <span data-ttu-id="98aa4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="98aa4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98aa4-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="98aa4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="98aa4-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98aa4-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="98aa4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="98aa4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98aa4-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="98aa4-113">Not supported.</span></span>    |
|<span data-ttu-id="98aa4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="98aa4-114">Application</span></span> | <span data-ttu-id="98aa4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="98aa4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="98aa4-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="98aa4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="98aa4-117">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="98aa4-117">Function parameters</span></span>

| <span data-ttu-id="98aa4-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="98aa4-118">Parameter</span></span>    | <span data-ttu-id="98aa4-119">型</span><span class="sxs-lookup"><span data-stu-id="98aa4-119">Type</span></span>   |<span data-ttu-id="98aa4-120">説明</span><span class="sxs-lookup"><span data-stu-id="98aa4-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98aa4-121">count</span><span class="sxs-lookup"><span data-stu-id="98aa4-121">count</span></span>|<span data-ttu-id="98aa4-122">Int32</span><span class="sxs-lookup"><span data-stu-id="98aa4-122">Int32</span></span>|<span data-ttu-id="98aa4-p102">結果の範囲に含める列の数です。通常、正の数値を使用して現在の範囲外に範囲を作成します。負の数値を使用して、現在の範囲内に範囲を作成することもできます。既定値は 1 です。</span><span class="sxs-lookup"><span data-stu-id="98aa4-p102">The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="98aa4-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="98aa4-127">Request headers</span></span>
| <span data-ttu-id="98aa4-128">名前</span><span class="sxs-lookup"><span data-stu-id="98aa4-128">Name</span></span>       | <span data-ttu-id="98aa4-129">説明</span><span class="sxs-lookup"><span data-stu-id="98aa4-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="98aa4-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="98aa4-130">Authorization</span></span>  | <span data-ttu-id="98aa4-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="98aa4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="98aa4-133">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="98aa4-133">Workbook-Session-Id</span></span>  | <span data-ttu-id="98aa4-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="98aa4-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="98aa4-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="98aa4-136">Request body</span></span>
<span data-ttu-id="98aa4-137">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="98aa4-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98aa4-138">応答</span><span class="sxs-lookup"><span data-stu-id="98aa4-138">Response</span></span>
<span data-ttu-id="98aa4-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/workbookrange.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="98aa4-139">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98aa4-140">例</span><span class="sxs-lookup"><span data-stu-id="98aa4-140">Example</span></span>
<span data-ttu-id="98aa4-141">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="98aa4-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="98aa4-142">要求</span><span class="sxs-lookup"><span data-stu-id="98aa4-142">Request</span></span>
<span data-ttu-id="98aa4-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="98aa4-143">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="98aa4-144">プロトコル</span><span class="sxs-lookup"><span data-stu-id="98aa4-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookrange_columnsbefore"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=2)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="98aa4-145">C#</span><span class="sxs-lookup"><span data-stu-id="98aa4-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-columnsbefore-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="98aa4-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="98aa4-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-columnsbefore-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="98aa4-147">目的-C</span><span class="sxs-lookup"><span data-stu-id="98aa4-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-columnsbefore-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="98aa4-148">Java</span><span class="sxs-lookup"><span data-stu-id="98aa4-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-columnsbefore-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="98aa4-149">応答</span><span class="sxs-lookup"><span data-stu-id="98aa4-149">Response</span></span>
<span data-ttu-id="98aa4-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="98aa4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
