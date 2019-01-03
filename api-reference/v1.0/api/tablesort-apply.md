---
title: 'TableSort: apply　'
description: 並べ替え操作を実行します。
author: lumine2008
ms.openlocfilehash: d3e19dbd1ed77f32a215dfa165ebc796706b09a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309682"
---
# <a name="tablesort-apply"></a><span data-ttu-id="2a2b1-103">TableSort: apply　</span><span class="sxs-lookup"><span data-stu-id="2a2b1-103">TableSort: apply</span></span>

<span data-ttu-id="2a2b1-104">並べ替え操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="2a2b1-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="2a2b1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2a2b1-105">Permissions</span></span>
<span data-ttu-id="2a2b1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a2b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a2b1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2a2b1-108">Permission type</span></span>      | <span data-ttu-id="2a2b1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2a2b1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a2b1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2a2b1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2a2b1-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a2b1-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2a2b1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2a2b1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a2b1-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2a2b1-113">Not supported.</span></span>    |
|<span data-ttu-id="2a2b1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2a2b1-114">Application</span></span> | <span data-ttu-id="2a2b1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2a2b1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a2b1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2a2b1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="2a2b1-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2a2b1-117">Request headers</span></span>
| <span data-ttu-id="2a2b1-118">名前</span><span class="sxs-lookup"><span data-stu-id="2a2b1-118">Name</span></span>       | <span data-ttu-id="2a2b1-119">説明</span><span class="sxs-lookup"><span data-stu-id="2a2b1-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2a2b1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a2b1-120">Authorization</span></span>  | <span data-ttu-id="2a2b1-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2a2b1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2a2b1-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2a2b1-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="2a2b1-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="2a2b1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a2b1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2a2b1-126">Request body</span></span>
<span data-ttu-id="2a2b1-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="2a2b1-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2a2b1-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="2a2b1-128">Parameter</span></span>    | <span data-ttu-id="2a2b1-129">種類</span><span class="sxs-lookup"><span data-stu-id="2a2b1-129">Type</span></span>   |<span data-ttu-id="2a2b1-130">説明</span><span class="sxs-lookup"><span data-stu-id="2a2b1-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a2b1-131">fields</span><span class="sxs-lookup"><span data-stu-id="2a2b1-131">fields</span></span>|<span data-ttu-id="2a2b1-132">WorkbookSortField コレクション</span><span class="sxs-lookup"><span data-stu-id="2a2b1-132">WorkbookSortField collection</span></span>|<span data-ttu-id="2a2b1-133">並べ替えに使用する条件の一覧。</span><span class="sxs-lookup"><span data-stu-id="2a2b1-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="2a2b1-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="2a2b1-134">matchCase</span></span>|<span data-ttu-id="2a2b1-135">ブール値</span><span class="sxs-lookup"><span data-stu-id="2a2b1-135">boolean</span></span>|<span data-ttu-id="2a2b1-p104">省略可能。大文字小文字の区別が文字列の順序に影響を与えるかどうか。</span><span class="sxs-lookup"><span data-stu-id="2a2b1-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="2a2b1-138">method</span><span class="sxs-lookup"><span data-stu-id="2a2b1-138">method</span></span>|<span data-ttu-id="2a2b1-139">string</span><span class="sxs-lookup"><span data-stu-id="2a2b1-139">string</span></span>|<span data-ttu-id="2a2b1-140">省略可能。</span><span class="sxs-lookup"><span data-stu-id="2a2b1-140">Optional.</span></span> <span data-ttu-id="2a2b1-141">中国語の文字に使用される順序の指定方法です。</span><span class="sxs-lookup"><span data-stu-id="2a2b1-141">The ordering method used for Chinese characters.</span></span>  <span data-ttu-id="2a2b1-142">可能な値: `PinYin`、 `StrokeCount`。</span><span class="sxs-lookup"><span data-stu-id="2a2b1-142">The possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="2a2b1-143">応答</span><span class="sxs-lookup"><span data-stu-id="2a2b1-143">Response</span></span>

<span data-ttu-id="2a2b1-p106">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="2a2b1-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a2b1-146">例</span><span class="sxs-lookup"><span data-stu-id="2a2b1-146">Example</span></span>
<span data-ttu-id="2a2b1-147">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="2a2b1-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2a2b1-148">要求</span><span class="sxs-lookup"><span data-stu-id="2a2b1-148">Request</span></span>
<span data-ttu-id="2a2b1-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2a2b1-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/apply
Content-type: application/json
Content-length: 298

{
  "fields": [
    {
      "key": 99,
      "sortOn": "sortOn-value",
      "ascending": true,
      "color": "color-value",
      "dataOption": "dataOption-value",
      "icon": {
        "set": "set-value",
        "index": 99
      }
    }
  ],
  "matchCase": true,
  "method": "method-value"
}
```

##### <a name="response"></a><span data-ttu-id="2a2b1-150">応答</span><span class="sxs-lookup"><span data-stu-id="2a2b1-150">Response</span></span>
<span data-ttu-id="2a2b1-151">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="2a2b1-151">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->