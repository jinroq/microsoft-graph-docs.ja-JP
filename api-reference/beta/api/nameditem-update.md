---
title: NamedItem オブジェクトを更新する
description: nameditem オブジェクトのプロパティを更新します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: f286a3ebb2ddf2973005e86ad3e52cec4607a2e2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992704"
---
# <a name="update-nameditem"></a><span data-ttu-id="2e69d-103">NamedItem オブジェクトを更新する</span><span class="sxs-lookup"><span data-stu-id="2e69d-103">Update nameditem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e69d-104">nameditem オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2e69d-104">Update the properties of nameditem object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2e69d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2e69d-105">Permissions</span></span>
<span data-ttu-id="2e69d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2e69d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e69d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2e69d-108">Permission type</span></span>      | <span data-ttu-id="2e69d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2e69d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e69d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2e69d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2e69d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e69d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2e69d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2e69d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e69d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e69d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2e69d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2e69d-114">Application</span></span> | <span data-ttu-id="2e69d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2e69d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e69d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2e69d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="2e69d-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2e69d-117">Optional request headers</span></span>
| <span data-ttu-id="2e69d-118">名前</span><span class="sxs-lookup"><span data-stu-id="2e69d-118">Name</span></span>       | <span data-ttu-id="2e69d-119">説明</span><span class="sxs-lookup"><span data-stu-id="2e69d-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2e69d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e69d-120">Authorization</span></span>  | <span data-ttu-id="2e69d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2e69d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2e69d-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2e69d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="2e69d-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="2e69d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e69d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2e69d-126">Request body</span></span>
<span data-ttu-id="2e69d-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="2e69d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2e69d-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e69d-130">Property</span></span>     | <span data-ttu-id="2e69d-131">型</span><span class="sxs-lookup"><span data-stu-id="2e69d-131">Type</span></span>   |<span data-ttu-id="2e69d-132">説明</span><span class="sxs-lookup"><span data-stu-id="2e69d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e69d-133">visible</span><span class="sxs-lookup"><span data-stu-id="2e69d-133">visible</span></span>|<span data-ttu-id="2e69d-134">ブール値</span><span class="sxs-lookup"><span data-stu-id="2e69d-134">boolean</span></span>|<span data-ttu-id="2e69d-135">オブジェクトを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="2e69d-135">Specifies whether the object is visible or not.</span></span>|
|<span data-ttu-id="2e69d-136">comment</span><span class="sxs-lookup"><span data-stu-id="2e69d-136">comment</span></span>|   <span data-ttu-id="2e69d-137">string</span><span class="sxs-lookup"><span data-stu-id="2e69d-137">string</span></span>  |<span data-ttu-id="2e69d-138">この名前に関連付けられているコメントを表します。</span><span class="sxs-lookup"><span data-stu-id="2e69d-138">Represents the comment associated with this name.</span></span>|

## <a name="response"></a><span data-ttu-id="2e69d-139">応答</span><span class="sxs-lookup"><span data-stu-id="2e69d-139">Response</span></span>

<span data-ttu-id="2e69d-140">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、更新された[workbookNamedItem](../resources/workbooknameditem.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2e69d-140">If successful, this method returns a `200 OK` response code and updated [workbookNamedItem](../resources/workbooknameditem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2e69d-141">例</span><span class="sxs-lookup"><span data-stu-id="2e69d-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e69d-142">要求</span><span class="sxs-lookup"><span data-stu-id="2e69d-142">Request</span></span>
<span data-ttu-id="2e69d-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2e69d-143">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2e69d-144">プロトコル</span><span class="sxs-lookup"><span data-stu-id="2e69d-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_nameditem"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}
Content-type: application/json
Content-length: 87

{
  "type": "type-value",
  "scope": "scope-value",
  "comment": "comment-value",
  "value": {
  },
  "visible": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2e69d-145">C#</span><span class="sxs-lookup"><span data-stu-id="2e69d-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-nameditem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2e69d-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="2e69d-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-nameditem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2e69d-147">目的-C</span><span class="sxs-lookup"><span data-stu-id="2e69d-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-nameditem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2e69d-148">Java</span><span class="sxs-lookup"><span data-stu-id="2e69d-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-nameditem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2e69d-149">応答</span><span class="sxs-lookup"><span data-stu-id="2e69d-149">Response</span></span>
<span data-ttu-id="2e69d-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2e69d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 87

{
  "name": "name-value",
  "type": "type-value",
  "value": {
  },
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update nameditem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
