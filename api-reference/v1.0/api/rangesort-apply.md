---
title: 'RangeSort: 適用'
description: 並べ替え操作を実行します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: be024f3eacbb4e2d1178ec7b82a8e8ca604aff60
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967106"
---
# <a name="rangesort-apply"></a><span data-ttu-id="b7d6b-103">RangeSort: 適用</span><span class="sxs-lookup"><span data-stu-id="b7d6b-103">RangeSort: apply</span></span>

<span data-ttu-id="b7d6b-104">並べ替え操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="b7d6b-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="b7d6b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b7d6b-105">Permissions</span></span>
<span data-ttu-id="b7d6b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7d6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7d6b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b7d6b-108">Permission type</span></span>      | <span data-ttu-id="b7d6b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b7d6b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7d6b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b7d6b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b7d6b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7d6b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b7d6b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b7d6b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7d6b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7d6b-113">Not supported.</span></span>    |
|<span data-ttu-id="b7d6b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b7d6b-114">Application</span></span> | <span data-ttu-id="b7d6b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7d6b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7d6b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b7d6b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="b7d6b-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b7d6b-117">Request headers</span></span>
| <span data-ttu-id="b7d6b-118">名前</span><span class="sxs-lookup"><span data-stu-id="b7d6b-118">Name</span></span>       | <span data-ttu-id="b7d6b-119">説明</span><span class="sxs-lookup"><span data-stu-id="b7d6b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b7d6b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7d6b-120">Authorization</span></span>  | <span data-ttu-id="b7d6b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b7d6b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b7d6b-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b7d6b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="b7d6b-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="b7d6b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7d6b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b7d6b-126">Request body</span></span>
<span data-ttu-id="b7d6b-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b7d6b-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b7d6b-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b7d6b-128">Parameter</span></span>    | <span data-ttu-id="b7d6b-129">Type</span><span class="sxs-lookup"><span data-stu-id="b7d6b-129">Type</span></span>   |<span data-ttu-id="b7d6b-130">説明</span><span class="sxs-lookup"><span data-stu-id="b7d6b-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7d6b-131">fields</span><span class="sxs-lookup"><span data-stu-id="b7d6b-131">fields</span></span>|<span data-ttu-id="b7d6b-132">WorkbookSortField コレクション</span><span class="sxs-lookup"><span data-stu-id="b7d6b-132">WorkbookSortField collection</span></span>|<span data-ttu-id="b7d6b-133">並べ替えに使用する条件の一覧。</span><span class="sxs-lookup"><span data-stu-id="b7d6b-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="b7d6b-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="b7d6b-134">matchCase</span></span>|<span data-ttu-id="b7d6b-135">ブール値</span><span class="sxs-lookup"><span data-stu-id="b7d6b-135">boolean</span></span>|<span data-ttu-id="b7d6b-p104">省略可能。大文字小文字の区別が文字列の順序に影響を与えるかどうか。</span><span class="sxs-lookup"><span data-stu-id="b7d6b-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="b7d6b-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="b7d6b-138">hasHeaders</span></span>|<span data-ttu-id="b7d6b-139">ブール値</span><span class="sxs-lookup"><span data-stu-id="b7d6b-139">boolean</span></span>|<span data-ttu-id="b7d6b-p105">省略可能。範囲にヘッダーがあるかどうか。</span><span class="sxs-lookup"><span data-stu-id="b7d6b-p105">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="b7d6b-142">orientation</span><span class="sxs-lookup"><span data-stu-id="b7d6b-142">orientation</span></span>|<span data-ttu-id="b7d6b-143">文字列</span><span class="sxs-lookup"><span data-stu-id="b7d6b-143">string</span></span>|<span data-ttu-id="b7d6b-144">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b7d6b-144">Optional.</span></span> <span data-ttu-id="b7d6b-145">かどうか操作が行または列を並べ替え。</span><span class="sxs-lookup"><span data-stu-id="b7d6b-145">Whether the operation is sorting rows or columns.</span></span>  <span data-ttu-id="b7d6b-146">可能な値: `Rows`、 `Columns`。</span><span class="sxs-lookup"><span data-stu-id="b7d6b-146">The possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="b7d6b-147">method</span><span class="sxs-lookup"><span data-stu-id="b7d6b-147">method</span></span>|<span data-ttu-id="b7d6b-148">文字列</span><span class="sxs-lookup"><span data-stu-id="b7d6b-148">string</span></span>|<span data-ttu-id="b7d6b-149">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b7d6b-149">Optional.</span></span> <span data-ttu-id="b7d6b-150">中国語の文字に使用される順序の指定方法です。</span><span class="sxs-lookup"><span data-stu-id="b7d6b-150">The ordering method used for Chinese characters.</span></span>  <span data-ttu-id="b7d6b-151">可能な値: `PinYin`、 `StrokeCount`。</span><span class="sxs-lookup"><span data-stu-id="b7d6b-151">The possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="b7d6b-152">応答</span><span class="sxs-lookup"><span data-stu-id="b7d6b-152">Response</span></span>

<span data-ttu-id="b7d6b-p108">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b7d6b-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7d6b-155">例</span><span class="sxs-lookup"><span data-stu-id="b7d6b-155">Example</span></span>
<span data-ttu-id="b7d6b-156">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="b7d6b-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b7d6b-157">要求</span><span class="sxs-lookup"><span data-stu-id="b7d6b-157">Request</span></span>
<span data-ttu-id="b7d6b-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b7d6b-158">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="b7d6b-159">応答</span><span class="sxs-lookup"><span data-stu-id="b7d6b-159">Response</span></span>
<span data-ttu-id="b7d6b-160">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b7d6b-160">Here is an example of the response.</span></span> 
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
  "tocPath": ""
}-->
