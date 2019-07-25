---
title: 名前付きアイテムの追加
description: ユーザーのロケールを数式に使用して、新しい名前を指定したスコープのコレクションに追加します。
localization_priority: Normal
ms.openlocfilehash: 2657326b774d111adbb0012f983eb99acccb15f7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879270"
---
# <a name="add-named-item"></a><span data-ttu-id="5e28e-103">名前付きアイテムの追加</span><span class="sxs-lookup"><span data-stu-id="5e28e-103">Add Named Item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e28e-104">ユーザーのロケールを数式に使用して、新しい名前を指定したスコープのコレクションに追加します。</span><span class="sxs-lookup"><span data-stu-id="5e28e-104">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e28e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5e28e-105">Permissions</span></span>
<span data-ttu-id="5e28e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5e28e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e28e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5e28e-108">Permission type</span></span>      | <span data-ttu-id="5e28e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5e28e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e28e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5e28e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5e28e-111">Files.ReadWrite、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e28e-111">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="5e28e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5e28e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e28e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e28e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5e28e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5e28e-114">Application</span></span> | <span data-ttu-id="5e28e-115">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e28e-115">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e28e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5e28e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="5e28e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5e28e-117">Request headers</span></span>
| <span data-ttu-id="5e28e-118">名前</span><span class="sxs-lookup"><span data-stu-id="5e28e-118">Name</span></span>       | <span data-ttu-id="5e28e-119">説明</span><span class="sxs-lookup"><span data-stu-id="5e28e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5e28e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e28e-120">Authorization</span></span>  | <span data-ttu-id="5e28e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5e28e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5e28e-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5e28e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="5e28e-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="5e28e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e28e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="5e28e-126">Request body</span></span>
<span data-ttu-id="5e28e-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="5e28e-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5e28e-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5e28e-128">Parameter</span></span>    | <span data-ttu-id="5e28e-129">型</span><span class="sxs-lookup"><span data-stu-id="5e28e-129">Type</span></span>   |<span data-ttu-id="5e28e-130">説明</span><span class="sxs-lookup"><span data-stu-id="5e28e-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e28e-131">name</span><span class="sxs-lookup"><span data-stu-id="5e28e-131">name</span></span>|<span data-ttu-id="5e28e-132">string</span><span class="sxs-lookup"><span data-stu-id="5e28e-132">string</span></span>|<span data-ttu-id="5e28e-133">名前付きの項目の名前。</span><span class="sxs-lookup"><span data-stu-id="5e28e-133">The name of the named item.</span></span>|
|<span data-ttu-id="5e28e-134">reference</span><span class="sxs-lookup"><span data-stu-id="5e28e-134">reference</span></span>|<span data-ttu-id="5e28e-135">string</span><span class="sxs-lookup"><span data-stu-id="5e28e-135">string</span></span>|<span data-ttu-id="5e28e-136">名前が参照する数式または範囲。</span><span class="sxs-lookup"><span data-stu-id="5e28e-136">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="5e28e-137">comment</span><span class="sxs-lookup"><span data-stu-id="5e28e-137">comment</span></span>|<span data-ttu-id="5e28e-138">string</span><span class="sxs-lookup"><span data-stu-id="5e28e-138">string</span></span>|<span data-ttu-id="5e28e-139">名前付きアイテムに関連付けられているコメント。</span><span class="sxs-lookup"><span data-stu-id="5e28e-139">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="5e28e-140">応答</span><span class="sxs-lookup"><span data-stu-id="5e28e-140">Response</span></span>

<span data-ttu-id="5e28e-141">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[workbookNamedItem](../resources/workbooknameditem.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5e28e-141">If successful, this method returns `200 OK` response code and [workbookNamedItem](../resources/workbooknameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e28e-142">例</span><span class="sxs-lookup"><span data-stu-id="5e28e-142">Example</span></span>
<span data-ttu-id="5e28e-143">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="5e28e-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="5e28e-144">要求</span><span class="sxs-lookup"><span data-stu-id="5e28e-144">Request</span></span>
<span data-ttu-id="5e28e-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5e28e-145">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5e28e-146">プロトコル</span><span class="sxs-lookup"><span data-stu-id="5e28e-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/add
Content-type: application/json
Content-length: 54

{
  "name": "test5",
  "reference": "=Sheet1!$F$15:$N$27",
  "comment": "Comment for the named item"
}


```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5e28e-147">C#</span><span class="sxs-lookup"><span data-stu-id="5e28e-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditemcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5e28e-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="5e28e-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditemcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5e28e-149">目的-C</span><span class="sxs-lookup"><span data-stu-id="5e28e-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditemcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5e28e-150">Java</span><span class="sxs-lookup"><span data-stu-id="5e28e-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/nameditemcollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5e28e-151">応答</span><span class="sxs-lookup"><span data-stu-id="5e28e-151">Response</span></span>
<span data-ttu-id="5e28e-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5e28e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookNamedItem",
    "@odata.type": "#microsoft.graph.workbookNamedItem",
    "@odata.id": "/users('ca41eb6e-5828-486b-ab52-c3bd1f7a4047')/drive/root/workbook/names(%27test5%27)",
    "comment": "Comment for the named item",
    "name": "test5",
    "scope": "Workbook",
    "type": "Range",
    "value": "Sheet1!$F$15:$N$27",
    "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "NamedItemCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
