---
title: 'RangeSort: 適用'
description: 並べ替え操作を実行します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 06d8b8840d642cb24c002e8d02f7b0f37bd1d47c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36376081"
---
# <a name="rangesort-apply"></a><span data-ttu-id="f0a72-103">RangeSort: 適用</span><span class="sxs-lookup"><span data-stu-id="f0a72-103">RangeSort: apply</span></span>

<span data-ttu-id="f0a72-104">並べ替え操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="f0a72-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="f0a72-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f0a72-105">Permissions</span></span>
<span data-ttu-id="f0a72-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f0a72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0a72-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f0a72-108">Permission type</span></span>      | <span data-ttu-id="f0a72-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f0a72-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0a72-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f0a72-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f0a72-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0a72-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f0a72-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f0a72-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0a72-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0a72-113">Not supported.</span></span>    |
|<span data-ttu-id="f0a72-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f0a72-114">Application</span></span> | <span data-ttu-id="f0a72-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0a72-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0a72-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f0a72-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="f0a72-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f0a72-117">Request headers</span></span>
| <span data-ttu-id="f0a72-118">名前</span><span class="sxs-lookup"><span data-stu-id="f0a72-118">Name</span></span>       | <span data-ttu-id="f0a72-119">説明</span><span class="sxs-lookup"><span data-stu-id="f0a72-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f0a72-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0a72-120">Authorization</span></span>  | <span data-ttu-id="f0a72-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f0a72-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f0a72-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f0a72-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="f0a72-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="f0a72-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0a72-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f0a72-126">Request body</span></span>
<span data-ttu-id="f0a72-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="f0a72-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f0a72-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f0a72-128">Parameter</span></span>    | <span data-ttu-id="f0a72-129">型</span><span class="sxs-lookup"><span data-stu-id="f0a72-129">Type</span></span>   |<span data-ttu-id="f0a72-130">説明</span><span class="sxs-lookup"><span data-stu-id="f0a72-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0a72-131">fields</span><span class="sxs-lookup"><span data-stu-id="f0a72-131">fields</span></span>|<span data-ttu-id="f0a72-132">WorkbookSortField コレクション</span><span class="sxs-lookup"><span data-stu-id="f0a72-132">WorkbookSortField collection</span></span>|<span data-ttu-id="f0a72-133">並べ替えに使用する条件の一覧。</span><span class="sxs-lookup"><span data-stu-id="f0a72-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="f0a72-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="f0a72-134">matchCase</span></span>|<span data-ttu-id="f0a72-135">ブール値</span><span class="sxs-lookup"><span data-stu-id="f0a72-135">boolean</span></span>|<span data-ttu-id="f0a72-p104">省略可能。大文字小文字の区別が文字列の順序に影響を与えるかどうか。</span><span class="sxs-lookup"><span data-stu-id="f0a72-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="f0a72-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="f0a72-138">hasHeaders</span></span>|<span data-ttu-id="f0a72-139">boolean</span><span class="sxs-lookup"><span data-stu-id="f0a72-139">boolean</span></span>|<span data-ttu-id="f0a72-p105">省略可能。範囲にヘッダーがあるかどうか。</span><span class="sxs-lookup"><span data-stu-id="f0a72-p105">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="f0a72-142">orientation</span><span class="sxs-lookup"><span data-stu-id="f0a72-142">orientation</span></span>|<span data-ttu-id="f0a72-143">string</span><span class="sxs-lookup"><span data-stu-id="f0a72-143">string</span></span>|<span data-ttu-id="f0a72-144">省略可能。</span><span class="sxs-lookup"><span data-stu-id="f0a72-144">Optional.</span></span> <span data-ttu-id="f0a72-145">操作が行と列のどちらの並べ替えかを示します。</span><span class="sxs-lookup"><span data-stu-id="f0a72-145">Whether the operation is sorting rows or columns.</span></span>  <span data-ttu-id="f0a72-146">使用可能な値は`Rows`、 `Columns`、です。</span><span class="sxs-lookup"><span data-stu-id="f0a72-146">The possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="f0a72-147">method</span><span class="sxs-lookup"><span data-stu-id="f0a72-147">method</span></span>|<span data-ttu-id="f0a72-148">string</span><span class="sxs-lookup"><span data-stu-id="f0a72-148">string</span></span>|<span data-ttu-id="f0a72-149">省略可能。</span><span class="sxs-lookup"><span data-stu-id="f0a72-149">Optional.</span></span> <span data-ttu-id="f0a72-150">中国語文字に使用される順序付けの方法です。</span><span class="sxs-lookup"><span data-stu-id="f0a72-150">The ordering method used for Chinese characters.</span></span>  <span data-ttu-id="f0a72-151">使用可能な値は`PinYin`、 `StrokeCount`、です。</span><span class="sxs-lookup"><span data-stu-id="f0a72-151">The possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="f0a72-152">応答</span><span class="sxs-lookup"><span data-stu-id="f0a72-152">Response</span></span>

<span data-ttu-id="f0a72-p108">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f0a72-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0a72-155">例</span><span class="sxs-lookup"><span data-stu-id="f0a72-155">Example</span></span>
<span data-ttu-id="f0a72-156">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="f0a72-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f0a72-157">要求</span><span class="sxs-lookup"><span data-stu-id="f0a72-157">Request</span></span>
<span data-ttu-id="f0a72-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f0a72-158">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f0a72-159">プロトコル</span><span class="sxs-lookup"><span data-stu-id="f0a72-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort/apply
Content-type: application/json
Content-length: 358

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
  "hasHeaders": true,
  "orientation": "orientation-value",
  "method": "method-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f0a72-160">C#</span><span class="sxs-lookup"><span data-stu-id="f0a72-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rangesort-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f0a72-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0a72-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangesort-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f0a72-162">目的-C</span><span class="sxs-lookup"><span data-stu-id="f0a72-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rangesort-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f0a72-163">Java</span><span class="sxs-lookup"><span data-stu-id="f0a72-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rangesort-apply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f0a72-164">応答</span><span class="sxs-lookup"><span data-stu-id="f0a72-164">Response</span></span>
<span data-ttu-id="f0a72-165">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f0a72-165">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
