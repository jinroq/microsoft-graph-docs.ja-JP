---
title: 名前付きアイテム FormulaLocal の追加
description: ユーザーのロケールを数式に使用して、新しい名前を指定したスコープのコレクションに追加します。
localization_priority: Normal
ms.openlocfilehash: 24232699220a025c19a4e2141d15ac76f0ad807f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814176"
---
# <a name="add-named-item-formulalocal"></a><span data-ttu-id="60412-103">名前付きアイテム FormulaLocal の追加</span><span class="sxs-lookup"><span data-stu-id="60412-103">Add Named Item FormulaLocal</span></span>
<span data-ttu-id="60412-104">ユーザーのロケールを数式に使用して、新しい名前を指定したスコープのコレクションに追加します。</span><span class="sxs-lookup"><span data-stu-id="60412-104">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="60412-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="60412-105">Permissions</span></span>
<span data-ttu-id="60412-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60412-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60412-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="60412-108">Permission type</span></span>      | <span data-ttu-id="60412-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="60412-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60412-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="60412-110">Delegated (work or school account)</span></span> | <span data-ttu-id="60412-111">Files.ReadWrite、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="60412-111">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="60412-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="60412-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60412-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60412-113">Not supported.</span></span>    |
|<span data-ttu-id="60412-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="60412-114">Application</span></span> | <span data-ttu-id="60412-115">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="60412-115">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60412-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="60412-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="60412-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60412-117">Request headers</span></span>
| <span data-ttu-id="60412-118">名前</span><span class="sxs-lookup"><span data-stu-id="60412-118">Name</span></span>       | <span data-ttu-id="60412-119">説明</span><span class="sxs-lookup"><span data-stu-id="60412-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="60412-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="60412-120">Authorization</span></span>  | <span data-ttu-id="60412-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="60412-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="60412-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="60412-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="60412-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="60412-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="60412-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="60412-126">Request body</span></span>
<span data-ttu-id="60412-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="60412-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="60412-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="60412-128">Parameter</span></span>    | <span data-ttu-id="60412-129">Type</span><span class="sxs-lookup"><span data-stu-id="60412-129">Type</span></span>   |<span data-ttu-id="60412-130">説明</span><span class="sxs-lookup"><span data-stu-id="60412-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60412-131">name</span><span class="sxs-lookup"><span data-stu-id="60412-131">name</span></span>|<span data-ttu-id="60412-132">文字列</span><span class="sxs-lookup"><span data-stu-id="60412-132">string</span></span>|<span data-ttu-id="60412-133">名前付きのアイテムの名前。</span><span class="sxs-lookup"><span data-stu-id="60412-133">The name of the named item.</span></span>|
|<span data-ttu-id="60412-134">formula</span><span class="sxs-lookup"><span data-stu-id="60412-134">formula</span></span>|<span data-ttu-id="60412-135">文字列</span><span class="sxs-lookup"><span data-stu-id="60412-135">string</span></span>|<span data-ttu-id="60412-136">名前が参照する数式または範囲。</span><span class="sxs-lookup"><span data-stu-id="60412-136">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="60412-137">comment</span><span class="sxs-lookup"><span data-stu-id="60412-137">comment</span></span>|<span data-ttu-id="60412-138">文字列</span><span class="sxs-lookup"><span data-stu-id="60412-138">string</span></span>|<span data-ttu-id="60412-139">名前付きアイテムに関連付けられているコメント。</span><span class="sxs-lookup"><span data-stu-id="60412-139">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="60412-140">応答</span><span class="sxs-lookup"><span data-stu-id="60412-140">Response</span></span>

<span data-ttu-id="60412-141">かどうかは成功すると、このメソッドを返します`200 OK`応答コードおよび応答の本文に[WorkbookNamedItem](../resources/nameditem.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="60412-141">If successful, this method returns `200 OK` response code and [WorkbookNamedItem](../resources/nameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60412-142">例</span><span class="sxs-lookup"><span data-stu-id="60412-142">Example</span></span>
<span data-ttu-id="60412-143">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="60412-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="60412-144">要求</span><span class="sxs-lookup"><span data-stu-id="60412-144">Request</span></span>
<span data-ttu-id="60412-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="60412-145">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/addFormulaLocal
Content-type: application/json
Content-length: 54

{
  "name": "test7",
  "formula": "=SUM(Sheet2!$A$1+Sheet2!$A$2)",
  "comment": "Comment for the named item"
}
```

##### <a name="response"></a><span data-ttu-id="60412-146">応答</span><span class="sxs-lookup"><span data-stu-id="60412-146">Response</span></span>
<span data-ttu-id="60412-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="60412-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
