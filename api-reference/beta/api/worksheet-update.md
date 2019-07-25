---
title: ワークシートを更新する
description: ワークシート オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f7120ebb7dfd199ad478a1160c30b5fd000a6ca8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866136"
---
# <a name="update-worksheet"></a><span data-ttu-id="c211c-103">ワークシートを更新する</span><span class="sxs-lookup"><span data-stu-id="c211c-103">Update worksheet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c211c-104">ワークシート オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c211c-104">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c211c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c211c-105">Permissions</span></span>
<span data-ttu-id="c211c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c211c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c211c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c211c-108">Permission type</span></span>      | <span data-ttu-id="c211c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c211c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c211c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c211c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c211c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c211c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c211c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c211c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c211c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c211c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c211c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c211c-114">Application</span></span> | <span data-ttu-id="c211c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c211c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c211c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c211c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="c211c-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c211c-117">Optional request headers</span></span>
| <span data-ttu-id="c211c-118">名前</span><span class="sxs-lookup"><span data-stu-id="c211c-118">Name</span></span>       | <span data-ttu-id="c211c-119">説明</span><span class="sxs-lookup"><span data-stu-id="c211c-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c211c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c211c-120">Authorization</span></span>  | <span data-ttu-id="c211c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c211c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c211c-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c211c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c211c-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="c211c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c211c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c211c-126">Request body</span></span>
<span data-ttu-id="c211c-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="c211c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c211c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c211c-130">Property</span></span>     | <span data-ttu-id="c211c-131">型</span><span class="sxs-lookup"><span data-stu-id="c211c-131">Type</span></span>   |<span data-ttu-id="c211c-132">説明</span><span class="sxs-lookup"><span data-stu-id="c211c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c211c-133">name</span><span class="sxs-lookup"><span data-stu-id="c211c-133">name</span></span>|<span data-ttu-id="c211c-134">string</span><span class="sxs-lookup"><span data-stu-id="c211c-134">string</span></span>|<span data-ttu-id="c211c-135">ワークシートの表示名。</span><span class="sxs-lookup"><span data-stu-id="c211c-135">The display name of the worksheet.</span></span>|
|<span data-ttu-id="c211c-136">position</span><span class="sxs-lookup"><span data-stu-id="c211c-136">position</span></span>|<span data-ttu-id="c211c-137">int</span><span class="sxs-lookup"><span data-stu-id="c211c-137">int</span></span>|<span data-ttu-id="c211c-138">0 を起点とした、ブック内のワークシートの位置。</span><span class="sxs-lookup"><span data-stu-id="c211c-138">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="c211c-139">visibility</span><span class="sxs-lookup"><span data-stu-id="c211c-139">visibility</span></span>|<span data-ttu-id="c211c-140">string</span><span class="sxs-lookup"><span data-stu-id="c211c-140">string</span></span>|<span data-ttu-id="c211c-p105">ワークシートの可視性。可能な値は、`Visible`、`Hidden`、`VeryHidden` です。</span><span class="sxs-lookup"><span data-stu-id="c211c-p105">The Visibility of the worksheet. Possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="c211c-143">応答</span><span class="sxs-lookup"><span data-stu-id="c211c-143">Response</span></span>

<span data-ttu-id="c211c-144">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、更新された[workbookWorksheet](../resources/workbookworksheet.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c211c-144">If successful, this method returns a `200 OK` response code and updated [workbookWorksheet](../resources/workbookworksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c211c-145">例</span><span class="sxs-lookup"><span data-stu-id="c211c-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c211c-146">要求</span><span class="sxs-lookup"><span data-stu-id="c211c-146">Request</span></span>
<span data-ttu-id="c211c-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c211c-147">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c211c-148">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c211c-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_worksheet"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}
Content-type: application/json
Content-length: 100

{
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c211c-149">C#</span><span class="sxs-lookup"><span data-stu-id="c211c-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c211c-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="c211c-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c211c-151">目的-C</span><span class="sxs-lookup"><span data-stu-id="c211c-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c211c-152">Java</span><span class="sxs-lookup"><span data-stu-id="c211c-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-worksheet-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c211c-153">応答</span><span class="sxs-lookup"><span data-stu-id="c211c-153">Response</span></span>
<span data-ttu-id="c211c-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c211c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update worksheet",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
