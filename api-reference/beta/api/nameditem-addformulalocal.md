---
title: 名前付きアイテム FormulaLocal の追加
description: ユーザーのロケールを数式に使用して、新しい名前を指定したスコープのコレクションに追加します。
localization_priority: Normal
ms.openlocfilehash: 406ca086f29cb6bcd8f1e309e5bd35d1f19c3299
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879261"
---
# <a name="add-named-item-formulalocal"></a><span data-ttu-id="71c1f-103">名前付きアイテム FormulaLocal の追加</span><span class="sxs-lookup"><span data-stu-id="71c1f-103">Add Named Item FormulaLocal</span></span>
<span data-ttu-id="71c1f-104">ユーザーのロケールを数式に使用して、新しい名前を指定したスコープのコレクションに追加します。</span><span class="sxs-lookup"><span data-stu-id="71c1f-104">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="71c1f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="71c1f-105">Permissions</span></span>
<span data-ttu-id="71c1f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="71c1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71c1f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="71c1f-108">Permission type</span></span>      | <span data-ttu-id="71c1f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="71c1f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71c1f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="71c1f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="71c1f-111">Files.ReadWrite、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="71c1f-111">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="71c1f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="71c1f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71c1f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71c1f-113">Not supported.</span></span>    |
|<span data-ttu-id="71c1f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="71c1f-114">Application</span></span> | <span data-ttu-id="71c1f-115">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="71c1f-115">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71c1f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="71c1f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="71c1f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71c1f-117">Request headers</span></span>
| <span data-ttu-id="71c1f-118">名前</span><span class="sxs-lookup"><span data-stu-id="71c1f-118">Name</span></span>       | <span data-ttu-id="71c1f-119">説明</span><span class="sxs-lookup"><span data-stu-id="71c1f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="71c1f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="71c1f-120">Authorization</span></span>  | <span data-ttu-id="71c1f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="71c1f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="71c1f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="71c1f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="71c1f-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="71c1f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="71c1f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="71c1f-126">Request body</span></span>
<span data-ttu-id="71c1f-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="71c1f-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="71c1f-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="71c1f-128">Parameter</span></span>    | <span data-ttu-id="71c1f-129">型</span><span class="sxs-lookup"><span data-stu-id="71c1f-129">Type</span></span>   |<span data-ttu-id="71c1f-130">説明</span><span class="sxs-lookup"><span data-stu-id="71c1f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71c1f-131">name</span><span class="sxs-lookup"><span data-stu-id="71c1f-131">name</span></span>|<span data-ttu-id="71c1f-132">string</span><span class="sxs-lookup"><span data-stu-id="71c1f-132">string</span></span>|<span data-ttu-id="71c1f-133">名前付きのアイテムの名前。</span><span class="sxs-lookup"><span data-stu-id="71c1f-133">The name of the named item.</span></span>|
|<span data-ttu-id="71c1f-134">formula</span><span class="sxs-lookup"><span data-stu-id="71c1f-134">formula</span></span>|<span data-ttu-id="71c1f-135">string</span><span class="sxs-lookup"><span data-stu-id="71c1f-135">string</span></span>|<span data-ttu-id="71c1f-136">名前が参照する数式または範囲。</span><span class="sxs-lookup"><span data-stu-id="71c1f-136">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="71c1f-137">comment</span><span class="sxs-lookup"><span data-stu-id="71c1f-137">comment</span></span>|<span data-ttu-id="71c1f-138">string</span><span class="sxs-lookup"><span data-stu-id="71c1f-138">string</span></span>|<span data-ttu-id="71c1f-139">名前付きアイテムに関連付けられているコメント。</span><span class="sxs-lookup"><span data-stu-id="71c1f-139">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="71c1f-140">応答</span><span class="sxs-lookup"><span data-stu-id="71c1f-140">Response</span></span>

<span data-ttu-id="71c1f-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [NamedItem](../resources/workbooknameditem.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="71c1f-141">If successful, this method returns `200 OK` response code and [NamedItem](../resources/workbooknameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71c1f-142">例</span><span class="sxs-lookup"><span data-stu-id="71c1f-142">Example</span></span>
<span data-ttu-id="71c1f-143">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="71c1f-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="71c1f-144">要求</span><span class="sxs-lookup"><span data-stu-id="71c1f-144">Request</span></span>
<span data-ttu-id="71c1f-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="71c1f-145">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="71c1f-146">プロトコル</span><span class="sxs-lookup"><span data-stu-id="71c1f-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/addFormulaLocal
Content-type: application/json
Content-length: 54

{
  "name": "test7",
  "formula": "=SUM(Sheet2!$A$1+Sheet2!$A$2)",
  "comment": "Comment for the named item"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="71c1f-147">C#</span><span class="sxs-lookup"><span data-stu-id="71c1f-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditemcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="71c1f-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="71c1f-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditemcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="71c1f-149">目的-C</span><span class="sxs-lookup"><span data-stu-id="71c1f-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditemcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="71c1f-150">Java</span><span class="sxs-lookup"><span data-stu-id="71c1f-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/nameditemcollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="71c1f-151">応答</span><span class="sxs-lookup"><span data-stu-id="71c1f-151">Response</span></span>
<span data-ttu-id="71c1f-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="71c1f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.id": "/users('ca41eb6e-5828-486b-ab52-c3bd1f7a4047')/drive/root/workbook/names(%27test7%27)",
    "comment": "Comment for the named item",
    "name": "test7",
    "scope": "Workbook",
    "type": "String",
    "value": "0",
    "visible": true
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItemCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
