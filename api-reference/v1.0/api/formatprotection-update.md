---
title: FormatProtection オブジェクトの更新
description: formatprotection オブジェクトのプロパティを更新します。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: a4550b0092a53af077e7475b1cb8b0a9febb1b62
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369442"
---
# <a name="update-formatprotection"></a><span data-ttu-id="4c72f-103">FormatProtection オブジェクトの更新</span><span class="sxs-lookup"><span data-stu-id="4c72f-103">Update formatprotection</span></span>

<span data-ttu-id="4c72f-104">formatprotection オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4c72f-104">Update the properties of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4c72f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4c72f-105">Permissions</span></span>
<span data-ttu-id="4c72f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c72f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c72f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4c72f-108">Permission type</span></span>      | <span data-ttu-id="4c72f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4c72f-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="4c72f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4c72f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4c72f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4c72f-111">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="4c72f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4c72f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c72f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c72f-113">Not supported.</span></span>    | 
|<span data-ttu-id="4c72f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4c72f-114">Application</span></span> | <span data-ttu-id="4c72f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c72f-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4c72f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4c72f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/protection
PATCH /workbook/worksheets/{id|name}/range(<address>)/format/protection
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-request-headers"></a><span data-ttu-id="4c72f-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c72f-117">Optional request headers</span></span>
| <span data-ttu-id="4c72f-118">名前</span><span class="sxs-lookup"><span data-stu-id="4c72f-118">Name</span></span>       | <span data-ttu-id="4c72f-119">説明</span><span class="sxs-lookup"><span data-stu-id="4c72f-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4c72f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c72f-120">Authorization</span></span>  | <span data-ttu-id="4c72f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4c72f-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="4c72f-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="4c72f-123">Request body</span></span>
<span data-ttu-id="4c72f-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="4c72f-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4c72f-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c72f-127">Property</span></span>     | <span data-ttu-id="4c72f-128">型</span><span class="sxs-lookup"><span data-stu-id="4c72f-128">Type</span></span>   |<span data-ttu-id="4c72f-129">説明</span><span class="sxs-lookup"><span data-stu-id="4c72f-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c72f-130">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="4c72f-130">formulaHidden</span></span>|<span data-ttu-id="4c72f-131">boolean</span><span class="sxs-lookup"><span data-stu-id="4c72f-131">boolean</span></span>|<span data-ttu-id="4c72f-p104">Excel が範囲内のセルの数式を非表示にするかどうかを示します。null 値は、範囲全体に一様な数式非表示設定がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="4c72f-p104">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="4c72f-134">locked</span><span class="sxs-lookup"><span data-stu-id="4c72f-134">locked</span></span>|<span data-ttu-id="4c72f-135">ブール値</span><span class="sxs-lookup"><span data-stu-id="4c72f-135">boolean</span></span>|<span data-ttu-id="4c72f-p105">Excel がオブジェクト内のセルをロックするかどうかを示します。null 値は、範囲全体に一様なロック設定がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="4c72f-p105">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="response"></a><span data-ttu-id="4c72f-138">応答</span><span class="sxs-lookup"><span data-stu-id="4c72f-138">Response</span></span>

<span data-ttu-id="4c72f-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [FormatProtection](../resources/formatprotection.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4c72f-139">If successful, this method returns a `200 OK` response code and updated [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4c72f-140">例</span><span class="sxs-lookup"><span data-stu-id="4c72f-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c72f-141">要求</span><span class="sxs-lookup"><span data-stu-id="4c72f-141">Request</span></span>
<span data-ttu-id="4c72f-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4c72f-142">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4c72f-143">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4c72f-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_formatprotection"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/protection
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4c72f-144">C#</span><span class="sxs-lookup"><span data-stu-id="4c72f-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-formatprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4c72f-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c72f-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-formatprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4c72f-146">目的-C</span><span class="sxs-lookup"><span data-stu-id="4c72f-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-formatprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4c72f-147">Java</span><span class="sxs-lookup"><span data-stu-id="4c72f-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-formatprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4c72f-148">応答</span><span class="sxs-lookup"><span data-stu-id="4c72f-148">Response</span></span>
<span data-ttu-id="4c72f-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4c72f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookFormatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update formatprotection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
